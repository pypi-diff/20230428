# Comparing `tmp/primap2-0.9.5.tar.gz` & `tmp/primap2-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primap2-0.9.5.tar", last modified: Tue Dec 13 17:12:02 2022, max compression
+gzip compressed data, was "primap2-0.9.6.tar", last modified: Fri Apr 28 09:39:42 2023, max compression
```

## Comparing `primap2-0.9.5.tar` & `primap2-0.9.6.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.700827 primap2-0.9.5/
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.688827 primap2-0.9.5/.github/
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.688827 primap2-0.9.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      671 2021-01-04 18:40:51.000000 primap2-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      548 2021-01-04 18:42:27.000000 primap2-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      364 2021-05-11 10:50:46.000000 primap2-0.9.5/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.688827 primap2-0.9.5/.github/workflows/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      950 2022-12-13 12:39:23.000000 primap2-0.9.5/.github/workflows/ci.yml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1320 2022-01-14 16:46:00.000000 primap2-0.9.5/.gitignore
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1348 2022-12-13 10:01:12.000000 primap2-0.9.5/.pre-commit-config.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      420 2022-05-09 18:22:07.000000 primap2-0.9.5/.readthedocs.yml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      175 2022-08-02 07:19:03.000000 primap2-0.9.5/AUTHORS.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5339 2022-12-13 17:11:10.000000 primap2-0.9.5/CHANGELOG.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1608 2022-08-02 07:19:03.000000 primap2-0.9.5/CONTRIBUTING.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    11357 2021-01-04 14:40:34.000000 primap2-0.9.5/LICENSE
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2860 2022-01-14 16:58:11.000000 primap2-0.9.5/Makefile
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8580 2022-12-13 17:12:02.700827 primap2-0.9.5/PKG-INFO
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2242 2022-12-13 17:11:38.000000 primap2-0.9.5/README.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      167 2022-08-02 07:19:03.000000 primap2-0.9.5/TODO.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      130 2021-03-08 13:18:42.000000 primap2-0.9.5/codecov.yml
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.688827 primap2-0.9.5/docs/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      620 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/Makefile
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.688827 primap2-0.9.5/docs/_static/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       28 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/_static/custom.css
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1796 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/api.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       30 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/changelog.rst
--rwxrwxr-x   0 pflueger  (1000) pflueger  (1000)     5210 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/conf.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      356 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/credits.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8297 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/data_format_details.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    14060 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_format_examples.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3891 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/data_reading.rst
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.692827 primap2-0.9.5/docs/data_reading_writing_examples/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      105 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/.gitignore
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    33106 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/FAOstat.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    44497 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/PRIMAP-hist.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      199 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/test_csv_data_long.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      432 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/test_csv_data_sec_cat.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1201 2022-11-02 13:15:33.000000 primap2-0.9.5/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      332 2022-11-02 13:15:33.000000 primap2-0.9.5/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5669 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/test_data_long.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5774 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/data_reading_writing_examples/test_data_wide.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1538 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/datalad.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    19137 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/development.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      436 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/index.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1106 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/installation.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     4579 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/interchange_format_details.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    11376 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/interchange_format_examples.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      769 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/make.bat
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    15032 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/minimal_ds.nc
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   543680 2022-05-09 17:51:11.000000 primap2-0.9.5/docs/opulent_ds.nc
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      292 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/pm2io.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       27 2022-08-02 07:19:03.000000 primap2-0.9.5/docs/readme.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      111 2022-05-09 18:22:07.000000 primap2-0.9.5/docs/requirements.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    28635 2022-07-26 17:09:05.000000 primap2-0.9.5/docs/usage.ipynb
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.692827 primap2-0.9.5/licenses/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      565 2021-01-15 15:18:07.000000 primap2-0.9.5/licenses/pint_xarray_license
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      565 2021-01-15 13:20:39.000000 primap2-0.9.5/licenses/xarray_license
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       64 2021-03-04 10:07:15.000000 primap2-0.9.5/mypy.ini
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2261 2022-05-09 18:22:07.000000 primap2-0.9.5/primap-stubs.patch
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.692827 primap2-0.9.5/primap2/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      304 2022-12-13 17:10:54.000000 primap2-0.9.5/primap2/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      327 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_accessor_base.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    21831 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_aggregate.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     9222 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_alias_selection.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    18224 2022-11-02 13:42:53.000000 primap2-0.9.5/primap2/_data_format.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    12267 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_downscale.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     9215 2022-11-02 13:42:53.000000 primap2-0.9.5/primap2/_merge.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2720 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_metadata.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5740 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_overview.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    23883 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_setters.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      423 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/_types.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    11462 2022-11-02 13:13:51.000000 primap2-0.9.5/primap2/_units.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1508 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/accessors.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.692827 primap2-0.9.5/primap2/pm2io/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     6343 2022-11-02 13:42:53.000000 primap2-0.9.5/primap2/pm2io/_GHG_inventory_reading.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      728 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/pm2io/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    13487 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/pm2io/_conversion.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    61107 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/pm2io/_data_reading.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    13974 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/pm2io/_interchange_format.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.696827 primap2-0.9.5/primap2/tests/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       79 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1640 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/conftest.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.696827 primap2-0.9.5/primap2/tests/data/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2999 2021-06-11 16:53:46.000000 primap2-0.9.5/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    21056 2021-06-11 16:53:46.000000 primap2-0.9.5/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      701 2021-06-11 16:53:46.000000 primap2-0.9.5/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        0 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/data/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      199 2021-04-14 15:51:03.000000 primap2-0.9.5/primap2/tests/data/long.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       84 2021-04-14 15:51:03.000000 primap2-0.9.5/primap2/tests/data/long_no_time.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       87 2021-04-14 15:51:03.000000 primap2-0.9.5/primap2/tests/data/test_csv_data.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      113 2021-06-07 09:00:48.000000 primap2-0.9.5/primap2/tests/data/test_csv_data_category_name.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      109 2021-06-07 09:00:48.000000 primap2-0.9.5/primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      231 2021-06-07 09:00:48.000000 primap2-0.9.5/primap2/tests/data/test_csv_data_category_name_long.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      432 2021-03-08 13:23:28.000000 primap2-0.9.5/primap2/tests/data/test_csv_data_sec_cat.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      434 2022-01-14 16:46:00.000000 primap2-0.9.5/primap2/tests/data/test_csv_data_sec_cat_strings.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    14880 2021-03-08 13:23:28.000000 primap2-0.9.5/primap2/tests/data/test_from_interchange_format_output.nc
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      198 2021-04-14 15:51:03.000000 primap2-0.9.5/primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      224 2021-06-07 09:00:48.000000 primap2-0.9.5/primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      446 2022-01-14 16:46:00.000000 primap2-0.9.5/primap2/tests/data/test_read_wide_csv_file_output.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      492 2022-01-14 16:46:00.000000 primap2-0.9.5/primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      328 2021-04-14 15:51:03.000000 primap2-0.9.5/primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    90672 2021-07-14 10:48:25.000000 primap2-0.9.5/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     6126 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/examples.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    11711 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_aggregate.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2988 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_alias_selection.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5501 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_conversion.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    11752 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_data_format.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    37510 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_data_reading.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     6827 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_downscale.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1737 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_interchange_format.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3597 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_merge.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1384 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_metadata.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     6107 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_overview.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    17673 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_setters.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2621 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/test_units.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1939 2022-08-02 07:19:03.000000 primap2-0.9.5/primap2/tests/utils.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.692827 primap2-0.9.5/primap2.egg-info/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8580 2022-12-13 17:12:02.000000 primap2-0.9.5/primap2.egg-info/PKG-INFO
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3607 2022-12-13 17:12:02.000000 primap2-0.9.5/primap2.egg-info/SOURCES.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        1 2022-12-13 17:12:02.000000 primap2-0.9.5/primap2.egg-info/dependency_links.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      413 2022-12-13 17:12:02.000000 primap2-0.9.5/primap2.egg-info/requires.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        8 2022-12-13 17:12:02.000000 primap2-0.9.5/primap2.egg-info/top_level.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      191 2021-03-18 18:20:05.000000 primap2-0.9.5/pyproject.toml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        2 2021-06-01 12:28:37.000000 primap2-0.9.5/requirements.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        7 2021-03-18 18:20:05.000000 primap2-0.9.5/requirements_dev.txt
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 17:12:02.700827 primap2-0.9.5/rosetta/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     4711 2021-04-13 15:09:35.000000 primap2-0.9.5/rosetta/combine_rows-set.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1843 2022-12-13 17:12:02.700827 primap2-0.9.5/setup.cfg
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       61 2022-08-02 07:19:03.000000 primap2-0.9.5/setup.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1315 2022-12-13 17:10:54.000000 primap2-0.9.5/tbump.toml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      385 2022-12-13 09:58:47.000000 primap2-0.9.5/tox.ini
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      706 2022-08-02 07:19:03.000000 primap2-0.9.5/update_changelog.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1147 2022-08-02 07:19:03.000000 primap2-0.9.5/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-03-31 17:51:36.000000 primap2-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-03-31 17:51:36.000000 primap2-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      364 2023-03-31 17:51:36.000000 primap2-0.9.6/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      955 2023-04-24 13:56:22.000000 primap2-0.9.6/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1340 2023-04-28 09:36:40.000000 primap2-0.9.6/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1197 2023-04-28 09:36:40.000000 primap2-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      406 2023-04-28 09:36:40.000000 primap2-0.9.6/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      173 2023-04-28 09:36:40.000000 primap2-0.9.6/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5612 2023-04-28 09:37:40.000000 primap2-0.9.6/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1608 2023-03-31 17:51:36.000000 primap2-0.9.6/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11357 2023-03-31 17:51:36.000000 primap2-0.9.6/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2860 2023-03-31 17:51:36.000000 primap2-0.9.6/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8851 2023-04-28 09:39:42.022160 primap2-0.9.6/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2284 2023-04-28 09:39:18.000000 primap2-0.9.6/README.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      167 2023-03-31 17:51:36.000000 primap2-0.9.6/TODO.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-03-31 17:51:36.000000 primap2-0.9.6/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      620 2023-04-04 07:09:04.000000 primap2-0.9.6/docs/Makefile
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/docs/_static/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       28 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/_static/custom.css
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1796 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5210 2023-04-24 13:56:22.000000 primap2-0.9.6/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      356 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8297 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_format_details.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14060 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_format_examples.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3891 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/docs/data_reading_writing_examples/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      105 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    33106 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/FAOstat.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    44497 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/PRIMAP-hist.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1201 2023-04-28 07:59:57.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      332 2023-04-28 07:59:57.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5669 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_data_long.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5774 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_data_wide.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1538 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/datalad.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    19051 2023-04-28 09:36:09.000000 primap2-0.9.6/docs/development.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      436 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1106 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4579 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/interchange_format_details.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11376 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/interchange_format_examples.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    15032 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/minimal_ds.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   543680 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/opulent_ds.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      292 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/pm2io.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      111 2023-04-04 07:21:47.000000 primap2-0.9.6/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    28635 2023-04-04 07:21:47.000000 primap2-0.9.6/docs/usage.ipynb
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/licenses/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.6/licenses/pint_xarray_license
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.6/licenses/xarray_license
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       64 2023-03-31 17:51:36.000000 primap2-0.9.6/mypy.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2261 2023-04-04 07:21:47.000000 primap2-0.9.6/primap-stubs.patch
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/primap2/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-28 09:37:24.000000 primap2-0.9.6/primap2/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      327 2023-04-25 14:13:52.000000 primap2-0.9.6/primap2/_accessor_base.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21858 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_aggregate.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9076 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_alias_selection.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18227 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_data_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    12288 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_downscale.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9246 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_merge.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2720 2023-04-25 13:24:13.000000 primap2-0.9.6/primap2/_metadata.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5656 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_overview.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23888 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_setters.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      423 2023-04-25 13:05:58.000000 primap2-0.9.6/primap2/_types.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11482 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_units.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1508 2023-04-25 13:14:07.000000 primap2-0.9.6/primap2/accessors.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/primap2/pm2io/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6332 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/pm2io/_GHG_inventory_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      728 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/pm2io/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13487 2023-04-25 15:48:53.000000 primap2-0.9.6/primap2/pm2io/_conversion.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    61245 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/pm2io/_data_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13953 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/pm2io/_interchange_format.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/primap2/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       79 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1640 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/primap2/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2999 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21056 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      701 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       84 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/long_no_time.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       87 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      113 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_category_name.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      109 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      231 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_category_name_long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_sec_cat.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      434 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_sec_cat_strings.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14880 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_from_interchange_format_output.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      198 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      224 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      446 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_output.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      492 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    90672 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6126 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11711 2023-04-04 07:21:47.000000 primap2-0.9.6/primap2/tests/test_aggregate.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2988 2023-04-28 08:57:53.000000 primap2-0.9.6/primap2/tests/test_alias_selection.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5501 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_conversion.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11752 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_data_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    37510 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/tests/test_data_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6827 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_downscale.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1737 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_interchange_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3597 2023-04-04 07:21:47.000000 primap2-0.9.6/primap2/tests/test_merge.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1384 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_metadata.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6107 2023-04-28 08:58:51.000000 primap2-0.9.6/primap2/tests/test_overview.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17597 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/tests/test_setters.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2621 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_units.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1911 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/tests/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/primap2.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8851 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3607 2023-04-28 09:39:42.000000 primap2-0.9.6/primap2.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      415 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        8 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      322 2023-04-28 09:36:40.000000 primap2-0.9.6/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-03-31 17:51:36.000000 primap2-0.9.6/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-03-31 17:51:36.000000 primap2-0.9.6/requirements_dev.txt
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/rosetta/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4711 2023-03-31 17:51:36.000000 primap2-0.9.6/rosetta/combine_rows-set.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1695 2023-04-28 09:39:42.022160 primap2-0.9.6/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-03-31 17:51:36.000000 primap2-0.9.6/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1315 2023-04-28 09:37:24.000000 primap2-0.9.6/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-24 13:56:22.000000 primap2-0.9.6/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      706 2023-03-31 17:51:36.000000 primap2-0.9.6/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1147 2023-03-31 17:51:36.000000 primap2-0.9.6/update_citation_info.py
```

### Comparing `primap2-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md` & `primap2-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md` & `primap2-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/.github/workflows/ci.yml` & `primap2-0.9.6/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest, windows-latest ]
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: [ 3.9, "3.10", "3.11" ]
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `primap2-0.9.5/.gitignore` & `primap2-0.9.6/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 parts/
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
 *.egg
+html/
+.mutmut-cache
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `primap2-0.9.5/CHANGELOG.rst` & `primap2-0.9.6/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+0.9.6
+-----
+* Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
+* stop building pdf output documentation, it doesn't support SVG and isn't used much.
+* Drop support for Python version 3.8 to prepare for it being dropped
+  in Numpy on April 14.
+
 0.9.5
 -----
 * pr.merge: use xarray's combine_first instead of own algorithm for better performance.
 * Fix in nan handling of to_interchange_format
 * made regexp_unit optional in nir_add_unit_information as intended already before
 * Add support for Python 3.11
```

### Comparing `primap2-0.9.5/CONTRIBUTING.rst` & `primap2-0.9.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/LICENSE` & `primap2-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/Makefile` & `primap2-0.9.6/Makefile`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/PKG-INFO` & `primap2-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: primap2
-Version: 0.9.5
+Version: 0.9.6
 Summary: The next generation of the PRIMAP climate policy analysis suite.
 Home-page: https://github.com/pik-primap/primap2
 Author: Mika Pflüger
-Author-email: mika.pflueger@pik-potsdam.de
+Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://primap2.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: datalad
 License-File: LICENSE
 
 =======
@@ -58,15 +57,17 @@
 ------
 
 PRIMAP2 is in active development, and not everything promised above is built
 yet.
 
 License
 -------
-Copyright 2020-2021, Potsdam-Institut für Klimafolgenforschung e.V.
+Copyright 2020-2022, Potsdam-Institut für Klimafolgenforschung e.V.
+
+Copyright 2023, Climate Resource Pty Ltd
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this
 file except in compliance with the License. You may obtain a copy of the License at
 
 https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under
@@ -78,22 +79,29 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2022-12-13).
-pik-primap/primap2: PRIMAP2 Version 0.9.5.
-Zenodo. https://doi.org/10.5281/zenodo.7434154
+Mika Pflüger and Johannes Gütschow. (2023-04-28).
+pik-primap/primap2: PRIMAP2 Version 0.9.6.
+Zenodo. https://doi.org/10.5281/zenodo.7875234
 
 =========
 Changelog
 =========
 
+0.9.6
+-----
+* Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
+* stop building pdf output documentation, it doesn't support SVG and isn't used much.
+* Drop support for Python version 3.8 to prepare for it being dropped
+  in Numpy on April 14.
+
 0.9.5
 -----
 * pr.merge: use xarray's combine_first instead of own algorithm for better performance.
 * Fix in nan handling of to_interchange_format
 * made regexp_unit optional in nir_add_unit_information as intended already before
 * Add support for Python 3.11
```

### Comparing `primap2-0.9.5/README.rst` & `primap2-0.9.6/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 ------
 
 PRIMAP2 is in active development, and not everything promised above is built
 yet.
 
 License
 -------
-Copyright 2020-2021, Potsdam-Institut für Klimafolgenforschung e.V.
+Copyright 2020-2022, Potsdam-Institut für Klimafolgenforschung e.V.
+
+Copyright 2023, Climate Resource Pty Ltd
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this
 file except in compliance with the License. You may obtain a copy of the License at
 
 https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under
@@ -52,10 +54,10 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2022-12-13).
-pik-primap/primap2: PRIMAP2 Version 0.9.5.
-Zenodo. https://doi.org/10.5281/zenodo.7434154
+Mika Pflüger and Johannes Gütschow. (2023-04-28).
+pik-primap/primap2: PRIMAP2 Version 0.9.6.
+Zenodo. https://doi.org/10.5281/zenodo.7875234
```

### Comparing `primap2-0.9.5/docs/Makefile` & `primap2-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/api.rst` & `primap2-0.9.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/conf.py` & `primap2-0.9.6/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 release = primap2.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `primap2-0.9.5/docs/data_format_details.rst` & `primap2-0.9.6/docs/data_format_details.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_format_examples.ipynb` & `primap2-0.9.6/docs/data_format_examples.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_reading.rst` & `primap2-0.9.6/docs/data_reading.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_reading_writing_examples/FAOstat.ipynb` & `primap2-0.9.6/docs/data_reading_writing_examples/FAOstat.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_reading_writing_examples/PRIMAP-hist.ipynb` & `primap2-0.9.6/docs/data_reading_writing_examples/PRIMAP-hist.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv` & `primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_reading_writing_examples/test_data_long.ipynb` & `primap2-0.9.6/docs/data_reading_writing_examples/test_data_long.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/data_reading_writing_examples/test_data_wide.ipynb` & `primap2-0.9.6/docs/data_reading_writing_examples/test_data_wide.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/datalad.rst` & `primap2-0.9.6/docs/datalad.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/development.rst` & `primap2-0.9.6/docs/development.rst`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 (yet) meant to be part of the public API using a leading ``_``, etc.
 
 If a part of the code should *not* follow our usual code style (because you are somewhat
 dubiously building ASCII art in Python or whatever), use
 `the fmt on/off directive <https://github.com/psf/black#the-black-code-style>`_ so black
 will ignore that part.
 
-We target Python version 3.6 and later, so using
+We target Python version 3.9 and later, so using
 `f-strings <https://docs.python.org/3/tutorial/inputoutput.html#tut-f-strings>`_ is fine
 and generally preferable to old-style format strings.
 
 Please use `type annotations <https://realpython.com/lessons/type-hinting/>`_ where
 appropriate to facilitate static type checking and state your expectations explicitly
 for other developers and users. Please also document your code, see the section below.
 
@@ -145,19 +145,18 @@
 We use `pre-commit <https://pre-commit.com/>`_ to catch smaller and larger errors before
 they are committed. All the configured checks and fixes are listed in the
 ``.pre-commit-config.yaml`` file, the most interesting ones in daily development are:
 
 - ``check-ast``: parses all python files and errors if the syntax is not valid.
 - ``check-merge-conflict``: emits an error if it finds unresolved merge conflicts.
 - ``black``: formats all python files using black.
-- ``flake8`` and ``doc8``: static analysis for unused imports and variables etc.
+- ``ruff`` and ``doc8``: static analysis for unused imports and variables etc.
   Sometimes, it is unavoidable to trigger flake8 errors, in that case add a comment of
   the form ``# noqa: E501`` at the end of the offending line (using the error code that
-  flake8 reports).
-- ``isort``: automatically sorts imports according to PEP8, so you don't have to.
+  ruff reports).
 
 At any time, you can run all the checks using::
 
    $ make lint
 
 Checks are also automatically run when you commit your changes, and the commit is
 aborted if errors are found or files are modified so you can review the changes. Since
```

### Comparing `primap2-0.9.5/docs/installation.rst` & `primap2-0.9.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/interchange_format_details.rst` & `primap2-0.9.6/docs/interchange_format_details.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/interchange_format_examples.ipynb` & `primap2-0.9.6/docs/interchange_format_examples.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/make.bat` & `primap2-0.9.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/minimal_ds.nc` & `primap2-0.9.6/docs/minimal_ds.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/opulent_ds.nc` & `primap2-0.9.6/docs/opulent_ds.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/docs/usage.ipynb` & `primap2-0.9.6/docs/usage.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/licenses/pint_xarray_license` & `primap2-0.9.6/licenses/pint_xarray_license`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/licenses/xarray_license` & `primap2-0.9.6/licenses/xarray_license`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap-stubs.patch` & `primap2-0.9.6/primap-stubs.patch`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/_aggregate.py` & `primap2-0.9.6/primap2/_aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Hashable, Iterable, Mapping, Optional, Sequence, Union
+from collections.abc import Hashable, Iterable, Mapping, Sequence
+from typing import Any, Optional, Union
 
 import numpy as np
 import xarray as xr
 
 from ._accessor_base import BaseDataArrayAccessor, BaseDatasetAccessor
 from ._alias_selection import alias_dims
 from ._types import DatasetOrDataArray, DimOrDimsT
```

### Comparing `primap2-0.9.5/primap2/_alias_selection.py` & `primap2-0.9.6/primap2/_alias_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 def translate(item: KeyT, translations: typing.Mapping[typing.Hashable, str]) -> KeyT:
     if isinstance(item, str):
         if item in translations:
             return translations[item]
         else:
             return item
     else:
-        sel: typing.Dict[typing.Hashable, typing.Hashable] = {}
+        sel: dict[typing.Hashable, typing.Hashable] = {}
         for key in item:
             if key in translations:
                 sel[translations[key]] = item[key]
             else:
                 sel[key] = item[key]
         return sel
 
 
 def translations_from_attrs(
-    attrs: typing.Dict[typing.Hashable, typing.Any], include_entity=False
-) -> typing.Dict[typing.Hashable, str]:
-    ret: typing.Dict[typing.Hashable, str] = {}
+    attrs: dict[typing.Hashable, typing.Any], include_entity=False
+) -> dict[typing.Hashable, str]:
+    ret: dict[typing.Hashable, str] = {}
     for key, abbrev in [("category", "cat"), ("scenario", "scen"), ("area", "area")]:
         if abbrev in attrs:
             ret[key] = attrs[abbrev]
             ret[abbrev] = attrs[abbrev]
     if "sec_cats" in attrs:
         for full_name in attrs["sec_cats"]:
             key = full_name.split("(")[0][:-1]
@@ -47,54 +47,50 @@
     if include_entity and "entity_terminology" in attrs:
         ret["entity"] = f"entity ({attrs['entity_terminology']})"
     return ret
 
 
 def translations_from_dims(
     dims: typing.Iterable[typing.Hashable],
-) -> typing.Dict[typing.Hashable, str]:
-    ret: typing.Dict[typing.Hashable, str] = {}
+) -> dict[typing.Hashable, str]:
+    ret: dict[typing.Hashable, str] = {}
     for dim in dims:
-        if isinstance(dim, str):
-            if " (" in dim:
-                key: str = dim.split("(")[0][:-1]
-                ret[key] = dim
+        if isinstance(dim, str) and " (" in dim:
+            key: str = dim.split("(")[0][:-1]
+            ret[key] = dim
     if "scenario" in ret:
         ret["scen"] = ret["scenario"]
     if "category" in ret:
         ret["cat"] = ret["category"]
     return ret
 
 
 def alias(
     dim: DimOrDimsT,
-    translations: typing.Dict[typing.Hashable, str],
+    translations: dict[typing.Hashable, str],
     dims: typing.Iterable[typing.Hashable],
 ) -> DimOrDimsT:
     if isinstance(dim, str):
         dim = translations.get(dim, dim)
         if dim not in dims:
             raise DimensionNotExistingError(dim)
         return dim
     else:
         try:
-            rdim = []
-            for idim in dim:
-                rdim.append(alias(idim, translations, dims))
-            return rdim
+            return [alias(idim, translations, dims) for idim in dim]
         except TypeError:  # not iterable, so some other hashable like int
             if dim not in dims:
-                raise DimensionNotExistingError(dim)
+                raise DimensionNotExistingError(dim) from None
             return dim
 
 
 def alias_dims(
     args_to_alias: typing.Iterable[str],
     wraps: typing.Optional[typing.Callable] = None,
-    additional_allowed_values: typing.Iterable[str] = tuple(),
+    additional_allowed_values: typing.Iterable[str] = (),
 ) -> typing.Callable[[FunctionT], FunctionT]:
     """Method decorator to automatically translate dimension aliases in parameters.
 
     Use like this:
     @alias_dims(["dim"])
     def sum(self, dim):
         return self._da.sum(dim)
@@ -102,15 +98,14 @@
     To copy the documentation etc. from an xarray function, use the wraps parameter:
     @alias_dims(["dim"], wraps=xr.DataArray.sum)
     def sum(self, *args, **kwargs):
         return self._da.sum(*args, **kwargs)
     """
 
     def decorator(func: FunctionT) -> FunctionT:
-
         if wraps is not None:
             wrap_func = wraps
         else:
             wrap_func = func
 
         # the parameters of the wrapped function without self
         func_args_list = list(inspect.signature(wrap_func).parameters.values())[1:]
@@ -176,15 +171,15 @@
         self._da.loc.__setitem__(
             translate(key, self._da.pr.dim_alias_translations), value
         )
 
 
 class DataArrayAliasSelectionAccessor(_accessor_base.BaseDataArrayAccessor):
     @property
-    def dim_alias_translations(self) -> typing.Dict[typing.Hashable, str]:
+    def dim_alias_translations(self) -> dict[typing.Hashable, str]:
         """Translate a shortened dimension alias to a full dimension name.
 
         For example, if the full dimension name is ``area (ISO3)``, the alias ``area``
         is mapped to ``area (ISO3)``.
 
         Returns
         -------
@@ -222,15 +217,15 @@
         self, item: typing.Mapping[typing.Hashable, typing.Any]
     ) -> xr.Dataset:
         return self._ds.loc[translate(item, self._ds.pr.dim_alias_translations)]
 
 
 class DatasetAliasSelectionAccessor(_accessor_base.BaseDatasetAccessor):
     @property
-    def dim_alias_translations(self) -> typing.Dict[typing.Hashable, str]:
+    def dim_alias_translations(self) -> dict[typing.Hashable, str]:
         """Translate a shortened dimension alias to a full dimension name.
 
         For example, if the full dimension name is ``area (ISO3)``, the alias ``area``
         is mapped to ``area (ISO3)``.
 
         Returns
         -------
```

### Comparing `primap2-0.9.5/primap2/_data_format.py` & `primap2-0.9.6/primap2/_data_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import contextlib
 import datetime
 import pathlib
-from typing import IO, Hashable, Iterable, Mapping, Optional, Tuple, Union
+from collections.abc import Hashable, Iterable, Mapping
+from typing import IO, Optional, Union
 
 import pandas as pd
 import pint
 import xarray as xr
 from loguru import logger
 
 from . import _accessor_base, pm2io
@@ -198,15 +200,15 @@
         return df
 
     def to_netcdf(
         self,
         path: Union[pathlib.Path, str],
         mode: str = "w",
         group: Optional[str] = None,
-        encoding: Mapping = None,
+        encoding: Union[Mapping, None] = None,
     ) -> Union[bytes, None]:
         """Write dataset contents to a netCDF file.
 
         Parameters
         ----------
         path : str or Path
             File path to which to save this dataset.
@@ -238,22 +240,24 @@
             group=group,
             encoding=encoding,
             engine="h5netcdf",
             format="NETCDF4",
         )
 
 
-def split_dim_name(dim_name: str) -> Tuple[str, str]:
+def split_dim_name(dim_name: str) -> tuple[str, str]:
     """Split a dimension name composed of the dimension, and the category set in
     parentheses into its parts."""
     try:
         dim, category_set = dim_name.split("(", 1)
     except ValueError:
         logger.error(f"{dim_name!r} not in the format 'dim (category_set)'.")
-        raise ValueError(f"{dim_name!r} not in the format 'dim (category_set)'")
+        raise ValueError(
+            f"{dim_name!r} not in the format 'dim (category_set)'"
+        ) from None
     return dim, category_set[:-1]
 
 
 def ensure_no_dimension_without_coordinates(ds: xr.Dataset):
     for dim in ds.dims:
         if dim not in ds.coords:
             logger.error(f"No coord found for dimension {dim!r}.")
@@ -278,38 +282,29 @@
                     f"Additional coordinate name {coord!r} contains a space, "
                     f"replace it with an underscore."
                 )
                 raise ValueError(f"Coord key {coord!r} contains a space")
 
 
 def ensure_valid_attributes(ds: xr.Dataset):
-    try:
+    with contextlib.suppress(KeyError):
         reference = ds.attrs["references"]
         if not reference.startswith("doi:"):
             logger.info(f"Reference information is not a DOI: {reference!r}")
-    except KeyError:
-        pass
-
-    try:
+    with contextlib.suppress(KeyError):
         contact = ds.attrs["contact"]
         if "@" not in contact:
             logger.info(f"Contact information is not an email address: {contact!r}.")
-    except KeyError:
-        pass
-
-    try:
+    with contextlib.suppress(KeyError):
         publication_date = ds.attrs["publication_date"]
         if not isinstance(publication_date, datetime.date):
             logger.error(
                 f"Publication date is not a datetime.date object: {publication_date!r}."
             )
             raise ValueError("Publication date is not a date object.")
-    except KeyError:
-        pass
-
     valid_attr_keys = {
         "references",
         "rights",
         "contact",
         "title",
         "comment",
         "institution",
@@ -359,27 +354,25 @@
         logger.error("'units' in variable attrs, but data is quantified already.")
         raise
 
 
 def ensure_entity_and_units_valid(key: Hashable, da: xr.DataArray):
     entity = da.attrs["entity"]
     units = da.pint.units
-    try:
+    with contextlib.suppress(pint.UndefinedUnitError):
         # if the entity is a gas and it is not converted to a gwp, the dimensions
         # should be compatible with an emission rate
         unit_entity = ureg(entity)
         if "gwp_context" not in da.attrs and not units.is_compatible_with(
             unit_entity * ureg.Gg / ureg.year
         ):
             logger.warning(
                 f"{key!r} has a unit of {units}, which is not "
                 f"compatible with an emission rate."
             )
-    except pint.UndefinedUnitError:
-        pass  # if the entity is something else, we can't directly check the dimensions
 
 
 def ensure_gwp_context_valid(key: str, da: xr.DataArray):
     units = da.pint.units
     gwp_context = da.attrs["gwp_context"]
 
     if units.dimensionality != {"[carbon]": 1, "[mass]": 1, "[time]": -1}:
@@ -390,15 +383,15 @@
         raise ValueError(f"{key} has wrong dimensionality for gwp_context.")
 
     try:
         with ureg.context(gwp_context):
             pass
     except KeyError:
         logger.error(f"gwp_context {gwp_context!r} for {key!r} is not valid.")
-        raise ValueError(f"Invalid gwp_context {gwp_context!r} for {key!r}")
+        raise ValueError(f"Invalid gwp_context {gwp_context!r} for {key!r}") from None
 
     if "(" not in key or not key.endswith(")"):
         logger.warning(f"{key!r} has a gwp_context in attrs, but not in its " f"name.")
 
 
 def ensure_not_gwp(key: Hashable, da: xr.DataArray):
     if (
```

### Comparing `primap2-0.9.5/primap2/_downscale.py` & `primap2-0.9.6/primap2/_downscale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Dict, Hashable, Optional, Sequence
+from collections.abc import Hashable, Sequence
+from typing import Optional
 
 import xarray as xr
 
 from ._accessor_base import BaseDataArrayAccessor, BaseDatasetAccessor
 from ._aggregate import select_no_scalar_dimension
 from ._units import ureg
 
@@ -11,15 +12,15 @@
     def downscale_timeseries(
         self,
         *,
         dim: Hashable,
         basket: Hashable,
         basket_contents: Sequence[Hashable],
         check_consistency: bool = True,
-        sel: Optional[Dict[Hashable, Sequence]] = None,
+        sel: Optional[dict[Hashable, Sequence]] = None,
         skipna_evaluation_dims: Sequence[Hashable] = tuple(),
     ) -> xr.DataArray:
         """Downscale timeseries along a dimension using a basket defined on a
         broader timeseries.
 
         This is useful if you have data for many points in time for a total, for example
         the entire Energy sector, and higher-resolution data (e.g. fossil and non-fossil
@@ -98,15 +99,15 @@
     def downscale_timeseries(
         self,
         *,
         dim: Hashable,
         basket: Hashable,
         basket_contents: Sequence[Hashable],
         check_consistency: bool = True,
-        sel: Optional[Dict[Hashable, Sequence]] = None,
+        sel: Optional[dict[Hashable, Sequence]] = None,
         skipna_evaluation_dims: Sequence[Hashable] = tuple(),
     ) -> xr.Dataset:
         """Downscale timeseries along a dimension using a basket defined on a
         broader timeseries.
 
         This is useful if you have data for many points in time for a total, for example
         the entire Energy sector, and higher-resolution data (e.g. fossil and non-fossil
@@ -188,15 +189,15 @@
 
     def downscale_gas_timeseries(
         self,
         *,
         basket: Hashable,
         basket_contents: Sequence[Hashable],
         check_consistency: bool = True,
-        sel: Optional[Dict[Hashable, Sequence]] = None,
+        sel: Optional[dict[Hashable, Sequence]] = None,
         skipna_evaluation_dims: Sequence[Hashable] = tuple(),
     ) -> xr.Dataset:
         """Downscale a gas basket defined on a broader timeseries to its contents
         known on fewer time points.
 
         This is useful if you have data for many points in time for a gas basket, for
         example KYOTOGHG, and higher-resolution data (e.g. the individual green house
```

### Comparing `primap2-0.9.5/primap2/_merge.py` & `primap2-0.9.6/primap2/_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Merge arrays and datasets with optional tolerances."""
 
+
+import contextlib
 import typing
 
 import numpy as np
 import xarray as xr
 from loguru import logger
 
 from ._accessor_base import BaseDataArrayAccessor, BaseDatasetAccessor
@@ -46,26 +48,23 @@
         If true throw an exception if false a warning and return values from
         the calling object in cases of conflict.
 
     Returns
     -------
         xr.DataArray: DataArray with data from da_merge merged into da_start
     """
-    try:
+    with contextlib.suppress(xr.MergeError):
         da_result = xr.merge(
             [da_start, da_merge],
             compat="no_conflicts",
             join="outer",
         )
         # all done as no errors occurred and thus no duplicates were present
         # make sure we have a DataArray not a Dataset
         return da_result[da_start.name]
-    except xr.MergeError:
-        pass
-
     # there are conflicts (overlapping coordinates) between da_start and da_merge
 
     # calculate the deviation between da_start and da_merge
     da_comp = abs(da_start - da_merge) / da_start
     da_error = da_comp.where(da_comp > tolerance, drop=True)
 
     if np.logical_not(da_error.isnull()).any():
@@ -171,15 +170,15 @@
 
 class DatasetMergeAccessor(BaseDatasetAccessor):
     def merge(
         self,
         ds_merge: xr.Dataset,
         tolerance: float = 0.01,
         error_on_discrepancy: bool = True,
-        combine_attrs: str = "drop_conflicts",
+        combine_attrs: xr.core.types.CombineAttrsOptions = "drop_conflicts",
     ) -> xr.Dataset:
         """
         Merge two Datasets with a given tolerance for discrepancies in values
         present in both Datasets. If values from the data to merge are already
         present in the calling object they are treated as equal if the relative
         difference is below the tolerance threshold. The result will use the values
         of the calling object.
@@ -201,25 +200,22 @@
 
         Returns
         -------
             xr.Dataset: Dataset with data from da_merge merged into the calling object
         """
         ds_start = self._ds
 
-        try:
+        with contextlib.suppress(xr.MergeError, ValueError):
             # if there are no conflicts just merge using xr.merge
             return xr.merge(
                 [ds_start, ds_merge],
                 compat="no_conflicts",
                 join="outer",
                 combine_attrs=combine_attrs,
             )
-        except (xr.MergeError, ValueError):
-            pass
-
         # merge by hand
         ensure_compatible_coords_dims(ds_merge, ds_start)
 
         vars_start = set(ds_start.data_vars)
         vars_merge = set(ds_merge.data_vars)
         vars_common = vars_start & vars_merge
         vars_only_start = vars_start - vars_common
```

### Comparing `primap2-0.9.5/primap2/_metadata.py` & `primap2-0.9.6/primap2/_metadata.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/_overview.py` & `primap2-0.9.6/primap2/_overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,20 +140,15 @@
         ds = self._ds
 
         for dim in dims:
             if dim == "entity":
                 continue
             ds = ds.drop_vars([x for x in ds if dim not in ds[x].dims])
 
-        all_boolean = True
-        for var in ds:
-            if ds[var].dtype != bool:
-                all_boolean = False
-                break
-
+        all_boolean = all(ds[var].dtype == bool for var in ds)
         if not all_boolean:  # Convert into boolean coverage array
             ds = ds.notnull()
 
         da = ds.pr.sum(reduce_to_dim=dims)
         if "entity" in dims:
             da = da.to_array("entity")
```

### Comparing `primap2-0.9.5/primap2/_setters.py` & `primap2-0.9.6/primap2/_setters.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
         try:
             return da.loc[{dim: key}]
         except KeyError:
             missing = set(key).difference(set(da[dim].values))
             raise KeyError(
                 f"Values {missing!r} not in {dim!r}, use new='extend' to "
                 f"automatically insert new values into dim."
-            )
+            ) from None
 
     @alias_dims(["dim", "value_dims"])
     def set(
         self,
         dim: typing.Hashable,
         key: typing.Any,
         value: typing.Union[xr.DataArray, np.ndarray],
         *,
-        value_dims: typing.Optional[typing.List[typing.Hashable]] = None,
+        value_dims: typing.Optional[list[typing.Hashable]] = None,
         existing: str = "fillna_empty",
         new: str = "extend",
     ) -> xr.DataArray:
         """Set values, optionally expanding the given dimension as necessary.
 
         The handling of already existing key values can be selected using the
         ``existing`` parameter.
@@ -263,15 +263,15 @@
         if isinstance(value, xr.DataArray):
             if value_dims is not None:
                 raise ValueError("value_dims given, but value is already a DataArray.")
 
             # conform value to given dim: key
             if dim not in value.dims:
                 if dim in value.coords:
-                    value = value.reset_coords(dim, drop=True)
+                    value = value.reset_coords([dim], drop=True)
                 value = value.expand_dims({dim: key})  # type: ignore
             else:
                 value = value.loc[{dim: key}]
 
             # we broadcast value to full self._da, a possible optimization would be
             # to broadcast value only to sel, but would need more careful handling
             # later.
```

### Comparing `primap2-0.9.5/primap2/_units.py` & `primap2-0.9.6/primap2/_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,22 +188,22 @@
         """
         if gwp_context is None:
             try:
                 gwp_context = self._da.attrs["gwp_context"]
             except KeyError:
                 raise ValueError(
                     "No gwp_context given and no gwp_context available in the attrs."
-                )
+                ) from None
         if entity is None:
             try:
                 entity = self._da.attrs["entity"]
             except KeyError:
                 raise ValueError(
                     "No entity given and no entity available in the attrs."
-                )
+                ) from None
 
         if isinstance(entity, str):
             entity = ureg.parse_units(entity)
 
         with ureg.context(gwp_context):
             da = self._da.pint.to(
                 self._da.pint.units / ureg.parse_units("CO2") * entity
```

### Comparing `primap2-0.9.5/primap2/accessors.py` & `primap2-0.9.6/primap2/accessors.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/pm2io/_GHG_inventory_reading.py` & `primap2-0.9.6/primap2/pm2io/_GHG_inventory_reading.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 and other official country emissions inventories
 Most of the functions in this file are exposed to the outside yet they
 currently do not undergo the strict testing applied to the rest of PRIMAP2 as
 they are added during the process of reading an preparing data for the PRIMAP-hist
 update. Testing will be added in the future."""
 
 import re
-from typing import Dict, List, Optional, Union
+from typing import Optional, Union
 
 import pandas as pd
 
 
 def nir_add_unit_information(
     df_nir: pd.DataFrame,
     *,
     unit_row: Union[str, int],
     entity_row: Optional[Union[str, int]] = None,
     regexp_entity: str,
     regexp_unit: Optional[str] = None,
-    manual_repl_unit: Optional[Dict[str, str]] = None,
-    manual_repl_entity: Optional[Dict[str, str]] = None,
+    manual_repl_unit: Optional[dict[str, str]] = None,
+    manual_repl_entity: Optional[dict[str, str]] = None,
     default_unit: str,
 ) -> pd.DataFrame:
     """Add unit information to a National Inventory Report (NIR) style DataFrame.
 
     Add unit information to the header of an "entity-wide" file as
     present in the standard table format of National Inventory Reports (NIRs). The
     unit and entity information is extracted from combined unit and entity information
@@ -131,15 +131,15 @@
     if cols_to_drop:
         df_out = df_out.drop(df_out.index[cols_to_drop])
 
     return df_out
 
 
 def nir_convert_df_to_long(
-    df_nir: pd.DataFrame, year: int, header_long: Optional[List[str]] = None
+    df_nir: pd.DataFrame, year: int, header_long: Optional[list[str]] = None
 ) -> pd.DataFrame:
     """Convert an entity-wide NIR table for a single year to a long format
     DataFrame.
 
     The input DataFrame is required to have the following structure:
     * Columns for category, original category name, and data in this order, where
     category and original category name form a multiindex.
@@ -162,10 +162,10 @@
         converted DataFrame
     """
     if header_long is None:
         header_long = ["category", "orig_cat_name", "entity", "unit", "time", "data"]
 
     df_stacked = df_nir.stack([0, 1], dropna=True).to_frame()
     df_stacked.insert(0, "year", str(year))
-    df_stacked.reset_index(inplace=True)
+    df_stacked = df_stacked.reset_index()
     df_stacked.columns = header_long
     return df_stacked
```

### Comparing `primap2-0.9.5/primap2/pm2io/__init__.py` & `primap2-0.9.6/primap2/pm2io/__init__.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/pm2io/_conversion.py` & `primap2-0.9.6/primap2/pm2io/_conversion.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/pm2io/_data_reading.py` & `primap2-0.9.6/primap2/pm2io/_data_reading.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import datetime
 import itertools
 import re
+from collections.abc import Iterable
 from pathlib import Path
-from typing import (
-    IO,
-    Any,
-    Callable,
-    Dict,
-    Hashable,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Union,
-)
+from typing import IO, Any, Callable, Union
 
 import numpy as np
 import pandas as pd
 import pint
 from loguru import logger
 
 from .. import _alias_selection
@@ -40,34 +30,35 @@
     "OTHERPFCS",
 ]
 
 
 def convert_long_dataframe_if(
     data_long: pd.DataFrame,
     *,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]] = None,
-    coords_defaults: Optional[Dict[str, Any]] = None,
-    coords_terminologies: Dict[str, str],
-    coords_value_mapping: Optional[Dict[str, Any]] = None,
-    coords_value_filling: Optional[Dict[str, Dict[str, Dict]]] = None,
-    filter_keep: Optional[Dict[str, Dict[str, Any]]] = None,
-    filter_remove: Optional[Dict[str, Dict[str, Any]]] = None,
-    meta_data: Optional[Dict[str, Any]] = None,
+    coords_cols: dict[str, str],
+    add_coords_cols: Union[None, dict[str, list[str]]] = None,
+    coords_defaults: Union[None, dict[str, Any]] = None,
+    coords_terminologies: dict[str, str],
+    coords_value_mapping: Union[None, dict[str, Any]] = None,
+    coords_value_filling: Union[None, dict[str, dict[str, dict]]] = None,
+    filter_keep: Union[None, dict[str, dict[str, Any]]] = None,
+    filter_remove: Union[None, dict[str, dict[str, Any]]] = None,
+    meta_data: Union[None, dict[str, Any]] = None,
     time_format: str = "%Y-%m-%d",
-    convert_str: Union[bool, Dict[str, float]] = True,
+    convert_str: Union[bool, dict[str, float]] = True,
     copy_df: bool = True,
 ) -> pd.DataFrame:
     """convert a DataFrame in long (tidy) format into the PRIMAP2 interchange format.
 
-    Columns can be renamed or filled with default values to match the PRIMAP2 structure.
-    Where we refer to "dimensions" in the parameter description below we mean the basic
-    dimension names without the added terminology (e.g. "area" not "area (ISO3)"). The
-    terminology information will be added by this function. You can not use the short
-    dimension names in the attributes (e.g. "cat" instead of "category").
+    Columns can be renamed or filled with default values to match the PRIMAP2
+    structure. Where we refer to "dimensions" in the parameter description below we
+    mean the basic dimension names without the added terminology (e.g. "area" not
+    "area (ISO3)"). The terminology information will be added by this function. You can
+    not use the short dimension names in the attributes (e.g. "cat" instead of
+    "category").
 
     Parameters
     ----------
     data_long: str, pd.DataFrame
         Long format DataFrame file which will be converted.
 
     coords_cols : dict
@@ -75,48 +66,48 @@
         the dimension in PRIMAP2. To specify the data column containing the observable,
         use the "data" key. For secondary categories use a ``sec_cats__`` prefix.
 
     add_coords_cols : dict, optional
         Dict where the keys are PRIMAP2 additional coordinate names and the values are
         lists with two elements where the first is the column in the dataframe to be
         converted and the second is the primap2 dimension for the coordinate (e.g.
-        ``category`` for a ``category_name`` coordinate.
+        ``category`` for a ``category_name`` coordinate).
 
     coords_defaults : dict, optional
         Dict for default values of coordinates / dimensions not given in the csv files.
         The keys are the dimension names and the values are the values for
         the dimensions. For secondary categories use a ``sec_cats__`` prefix.
 
     coords_terminologies : dict
         Dict defining the terminologies used for the different coordinates (e.g. ISO3
         for area). Only possible coordinates here are: area, category, scenario,
         entity, and secondary categories. For secondary categories use a ``sec_cats__``
-        prefix. All entries different from "area", "category", "scenario", "entity", and
-        ``sec_cats__<name>`` will raise a ValueError.
+        prefix. All entries different from "area", "category", "scenario", "entity",
+        and ``sec_cats__<name>`` will raise a ValueError.
 
     coords_value_mapping : dict, optional
         A dict with primap2 dimension names as keys. Values are dicts with input values
         as keys and output values as values. A standard use case is to map gas names
         from input data to the standardized names used in primap2.
         Alternatively a value can also be a function which transforms one CSV metadata
         value into the new metadata value.
         A third possibility is to give a string as a value, which defines a rule for
         translating metadata values. For the "category", "entity", and "unit" columns,
         the rule "PRIMAP1" is available, which translates from PRIMAP1 metadata to
         PRIMAP2 metadata.
 
     coords_value_filling : dict, optional
         A dict with primap2 dimension names as keys. These are the target columns where
-        values will be filled (or replaced). Vales are dicts with primap2 dimension names
-        as keys. These are the source columns. The values are dicts with source value -
-        target value mappings.
-        The value filling can do everything that the value mapping can, but while mapping
-        can only replace values within a column using information from that column, the
-        filing function can also fill or replace data based on values from a different
-        column.
+        values will be filled (or replaced). Vales are dicts with primap2 dimension
+        names as keys. These are the source columns. The values are dicts with source
+        value - target value mappings.
+        The value filling can do everything that the value mapping can, but while
+        mapping can only replace values within a column using information from that
+        column, the filing function can also fill or replace data based on values from
+        a different column.
         This can be used to e.g. fill missing category codes based on category names or
         to replace category codes which do not meet the terminology using the category
         names.
 
     filter_keep : dict, optional
         Dict defining filters of data to keep. Filtering is done before metadata
         mapping, so use original metadata values to define the filter. Column names are
@@ -130,15 +121,16 @@
         The names of the filters have no relevance.
 
     meta_data : dict, optional
         Meta data for the whole dataset. Will end up in the dataset-wide attrs. Allowed
         keys are "references", "rights", "contact", "title", "comment", "institution",
         and "history". Documentation about the format and meaning of the meta data can
         be found in the
-        `data format documentation <https://primap2.readthedocs.io/en/stable/data_format_details.html#dataset-attributes>`_.  # noqa: E501
+        `data format documentation <https://primap2.readthedocs.io/en/stable/\
+data_format_details.html#dataset-attributes>`_.
 
     time_format : str, optional (default: "%Y-%m-%d")
         strftime style format used to format the time information for the data columns
         in the interchange format.
         Default: "%F", i.e. the ISO 8601 date format.
 
     convert_str : bool or dict, optional (default: True)
@@ -264,33 +256,34 @@
 
     return data
 
 
 def read_long_csv_file_if(
     filepath_or_buffer: Union[str, Path, IO],
     *,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]] = None,
-    coords_defaults: Optional[Dict[str, Any]] = None,
-    coords_terminologies: Dict[str, str],
-    coords_value_mapping: Optional[Dict[str, Any]] = None,
-    coords_value_filling: Optional[Dict[str, Dict[str, Dict]]] = None,
-    filter_keep: Optional[Dict[str, Dict[str, Any]]] = None,
-    filter_remove: Optional[Dict[str, Dict[str, Any]]] = None,
-    meta_data: Optional[Dict[str, Any]] = None,
+    coords_cols: dict[str, str],
+    add_coords_cols: Union[None, dict[str, list[str]]] = None,
+    coords_defaults: Union[None, dict[str, Any]] = None,
+    coords_terminologies: dict[str, str],
+    coords_value_mapping: Union[None, dict[str, Any]] = None,
+    coords_value_filling: Union[None, dict[str, dict[str, dict]]] = None,
+    filter_keep: Union[None, dict[str, dict[str, Any]]] = None,
+    filter_remove: Union[None, dict[str, dict[str, Any]]] = None,
+    meta_data: Union[None, dict[str, Any]] = None,
     time_format: str = "%Y-%m-%d",
-    convert_str: Union[bool, Dict[str, float]] = True,
+    convert_str: Union[bool, dict[str, float]] = True,
 ) -> pd.DataFrame:
     """Read a CSV file in long (tidy) format into the PRIMAP2 interchange format.
 
-    Columns can be renamed or filled with default values to match the PRIMAP2 structure.
-    Where we refer to "dimensions" in the parameter description below we mean the basic
-    dimension names without the added terminology (e.g. "area" not "area (ISO3)"). The
-    terminology information will be added by this function. You can not use the short
-    dimension names in the attributes (e.g. "cat" instead of "category").
+    Columns can be renamed or filled with default values to match the PRIMAP2
+    structure. Where we refer to "dimensions" in the parameter description below we
+    mean the basic dimension names without the added terminology (e.g. "area" not
+    "area (ISO3)"). The terminology information will be added by this function. You can
+    not use the short dimension names in the attributes (e.g. "cat" instead of
+    "category").
 
     Parameters
     ----------
     filepath_or_buffer: str, pathlib.Path, or file-like
         Long CSV file which will be read.
 
     coords_cols : dict
@@ -298,48 +291,48 @@
         the dimension in PRIMAP2. To specify the data column containing the observable,
         use the "data" key. For secondary categories use a ``sec_cats__`` prefix.
 
     add_coords_cols : dict, optional
         Dict where the keys are PRIMAP2 additional coordinate names and the values are
         lists with two elements where the first is the column in the csv file to be
         read and the second is the primap2 dimension for the coordinate (e.g.
-        ``category`` for a ``category_name`` coordinate.
+        ``category`` for a ``category_name`` coordinate).
 
     coords_defaults : dict, optional
         Dict for default values of coordinates / dimensions not given in the csv files.
         The keys are the dimension names and the values are the values for
         the dimensions. For secondary categories use a ``sec_cats__`` prefix.
 
     coords_terminologies : dict
         Dict defining the terminologies used for the different coordinates (e.g. ISO3
         for area). Only possible coordinates here are: area, category, scenario,
         entity, and secondary categories. For secondary categories use a ``sec_cats__``
-        prefix. All entries different from "area", "category", "scenario", "entity", and
-        ``sec_cats__<name>`` will raise a ValueError.
+        prefix. All entries different from "area", "category", "scenario", "entity",
+        and ``sec_cats__<name>`` will raise a ValueError.
 
     coords_value_mapping : dict, optional
         A dict with primap2 dimension names as keys. Values are dicts with input values
         as keys and output values as values. A standard use case is to map gas names
         from input data to the standardized names used in primap2.
         Alternatively a value can also be a function which transforms one CSV metadata
         value into the new metadata value.
         A third possibility is to give a string as a value, which defines a rule for
         translating metadata values. For the "category", "entity", and "unit" columns,
         the rule "PRIMAP1" is available, which translates from PRIMAP1 metadata to
         PRIMAP2 metadata.
 
     coords_value_filling : dict, optional
         A dict with primap2 dimension names as keys. These are the target columns where
-        values will be filled (or replaced). Vales are dicts with primap2 dimension names
-        as keys. These are the source columns. The values are dicts with source value -
-        target value mappings.
-        The value filling can do everything that the value mapping can, but while mapping
-        can only replace values within a column using information from that column, the
-        filing function can also fill or replace data based on values from a different
-        column.
+        values will be filled (or replaced). Vales are dicts with primap2 dimension
+        names as keys. These are the source columns. The values are dicts with source
+        value - target value mappings.
+        The value filling can do everything that the value mapping can, but while
+        mapping can only replace values within a column using information from that
+        column, the filing function can also fill or replace data based on values from
+        a different column.
         This can be used to e.g. fill missing category codes based on category names or
         to replace category codes which do not meet the terminology using the category
         names.
 
     filter_keep : dict, optional
         Dict defining filters of data to keep. Filtering is done before metadata
         mapping, so use original metadata values to define the filter. Column names are
@@ -353,15 +346,16 @@
         The names of the filters have no relevance.
 
     meta_data : dict, optional
         Meta data for the whole dataset. Will end up in the dataset-wide attrs. Allowed
         keys are "references", "rights", "contact", "title", "comment", "institution",
         and "history". Documentation about the format and meaning of the meta data can
         be found in the
-        `data format documentation <https://primap2.readthedocs.io/en/stable/data_format_details.html#dataset-attributes>`_.  # noqa: E501
+        `data format documentation <https://primap2.readthedocs.io/en/stable/\
+data_format_details.html#dataset-attributes>`_.
 
     time_format : str, optional
         strftime style format used to format the time information for the data columns
         in the interchange format.
         Default: "%F", i.e. the ISO 8601 date format.
 
     convert_str : bool or dict, optional (default: True)
@@ -429,61 +423,62 @@
         convert_str=convert_str,
         copy_df=False,
     )
 
 
 def long_to_wide(
     data_long: pd.DataFrame, *, time_format: str
-) -> (pd.DataFrame, Set[str]):
+) -> tuple[pd.DataFrame, list[str]]:
     data_long["time"] = data_long["time"].dt.strftime(time_format)
 
     coords = list(set(data_long.columns.values) - {"data", "time"})
 
     # unit is neither a coordinate nor a data column, so has to be handled separately
     unit = data_long[coords].drop_duplicates()
     coords.remove("unit")
     unit.index = pd.MultiIndex.from_frame(unit[coords])
 
     series = data_long["data"]
-    series.index = pd.MultiIndex.from_frame(data_long[coords + ["time"]])
+    series.index = pd.MultiIndex.from_frame(data_long[[*coords, "time"]])
     data = series.unstack("time")
 
     data["unit"] = unit["unit"]
 
     data.reset_index(inplace=True)
     data.columns.name = None
 
-    return data, coords + ["unit"]
+    return data, [*coords, "unit"]
 
 
 def convert_wide_dataframe_if(
     data_wide: pd.DataFrame,
     *,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]] = None,
-    coords_defaults: Optional[Dict[str, Any]] = None,
-    coords_terminologies: Dict[str, str],
-    coords_value_mapping: Optional[Dict[str, Any]] = None,
-    coords_value_filling: Optional[Dict[str, Dict[str, Dict]]] = None,
-    filter_keep: Optional[Dict[str, Dict[str, Any]]] = None,
-    filter_remove: Optional[Dict[str, Dict[str, Any]]] = None,
-    meta_data: Optional[Dict[str, Any]] = None,
+    coords_cols: dict[str, str],
+    add_coords_cols: Union[None, dict[str, list[str]]] = None,
+    coords_defaults: Union[None, dict[str, Any]] = None,
+    coords_terminologies: dict[str, str],
+    coords_value_mapping: Union[None, dict[str, Any]] = None,
+    coords_value_filling: Union[None, dict[str, dict[str, dict]]] = None,
+    filter_keep: Union[None, dict[str, dict[str, Any]]] = None,
+    filter_remove: Union[None, dict[str, dict[str, Any]]] = None,
+    meta_data: Union[None, dict[str, Any]] = None,
     time_format: str = "%Y",
-    time_cols: Optional[List] = None,
-    convert_str: Union[bool, Dict[str, float]] = True,
+    time_cols: Union[None, list] = None,
+    convert_str: Union[bool, dict[str, float]] = True,
     copy_df: bool = False,
 ) -> pd.DataFrame:
     """
     Convert a DataFrame in wide format into the PRIMAP2 interchange format.
 
-    Columns can be renamed or filled with default values to match the PRIMAP2 structure.
-    Where we refer to "dimensions" in the parameter description below we mean the basic
-    dimension names without the added terminology (e.g. "area" not "area (ISO3)"). The
-    terminology information will be added by this function. You can not use the short
-    dimension names in the attributes (e.g. "cat" instead of "category").
+    Columns can be renamed or filled with default values to match the PRIMAP2
+    structure. Where we refer to "dimensions" in the parameter description below we
+    mean the basic dimension names without the added terminology (e.g. "area" not
+    "area (ISO3)"). The terminology information will be added by this function. You can
+    not use the short dimension names in the attributes (e.g. "cat" instead of
+    "category").
 
     TODO: Currently duplicate data points will not be detected.
 
     TODO: enable filtering through query strings
 
     TODO: enable specification of the entity terminology
 
@@ -508,37 +503,37 @@
         The keys are the dimension names and the values are the values for
         the dimensions. For secondary categories use a ``sec_cats__`` prefix.
 
     coords_terminologies : dict
         Dict defining the terminologies used for the different coordinates (e.g. ISO3
         for area). Only possible coordinates here are: area, category, scenario,
         entity, and secondary categories. For secondary categories use a ``sec_cats__``
-        prefix. All entries different from "area", "category", "scenario", "entity", and
-        ``sec_cats__<name>`` will raise a ValueError.
+        prefix. All entries different from "area", "category", "scenario", "entity",
+        and ``sec_cats__<name>`` will raise a ValueError.
 
     coords_value_mapping : dict, optional
         A dict with primap2 dimension names as keys. Values are dicts with input values
         as keys and output values as values. A standard use case is to map gas names
         from input data to the standardized names used in primap2.
         Alternatively a value can also be a function which transforms one CSV metadata
         value into the new metadata value.
         A third possibility is to give a string as a value, which defines a rule for
         translating metadata values. The only defined rule at the moment is "PRIMAP1"
         which can be used for the "category", "entity", and "unit" columns to translate
         from PRIMAP1 metadata to PRIMAP2 metadata.
 
     coords_value_filling : dict, optional
         A dict with primap2 dimension names as keys. These are the target columns where
-        values will be filled (or replaced). Vales are dicts with primap2 dimension names
-        as keys. These are the source columns. The values are dicts with source value -
-        target value mappings.
-        The value filling can do everything that the value mapping can, but while mapping
-        can only replace values within a column using information from that column, the
-        filing function can also fill or replace data based on values from a different
-        column.
+        values will be filled (or replaced). Vales are dicts with primap2 dimension
+        names as keys. These are the source columns. The values are dicts with source
+        value - target value mappings.
+        The value filling can do everything that the value mapping can, but while
+        mapping can only replace values within a column using information from that
+        column, the filing function can also fill or replace data based on values from
+        a different column.
         This can be used to e.g. fill missing category codes based on category names or
         to replace category codes which do not meet the terminology using the category
         names.
 
     filter_keep : dict, optional
         Dict defining filters of data to keep. Filtering is done before metadata
         mapping, so use original metadata values to define the filter. Column names are
@@ -552,15 +547,16 @@
         The names of the filters have no relevance.
 
     meta_data : dict, optional
         Meta data for the whole dataset. Will end up in the dataset-wide attrs. Allowed
         keys are "references", "rights", "contact", "title", "comment", "institution",
         and "history". Documentation about the format and meaning of the meta data can
         be found in the
-        `data format documentation <https://primap2.readthedocs.io/en/stable/data_format_details.html#dataset-attributes>`_.  # noqa: E501
+        `data format documentation <https://primap2.readthedocs.io/en/stable/\
+data_format_details.html#dataset-attributes>`_.
 
     time_format : str
         str with strftime style format used to parse the time information for
         the data columns.
         Default: "%Y", which will match years.
 
     time_cols : list, optional
@@ -693,33 +689,34 @@
 
     return data_if
 
 
 def read_wide_csv_file_if(
     filepath_or_buffer: Union[str, Path, IO],
     *,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]] = None,
-    coords_defaults: Optional[Dict[str, Any]] = None,
-    coords_terminologies: Dict[str, str],
-    coords_value_mapping: Optional[Dict[str, Any]] = None,
-    coords_value_filling: Optional[Dict[str, Dict[str, Dict]]] = None,
-    filter_keep: Optional[Dict[str, Dict[str, Any]]] = None,
-    filter_remove: Optional[Dict[str, Dict[str, Any]]] = None,
-    meta_data: Optional[Dict[str, Any]] = None,
+    coords_cols: dict[str, str],
+    add_coords_cols: Union[None, dict[str, list[str]]] = None,
+    coords_defaults: Union[None, dict[str, Any]] = None,
+    coords_terminologies: dict[str, str],
+    coords_value_mapping: Union[None, dict[str, Any]] = None,
+    coords_value_filling: Union[None, dict[str, dict[str, dict]]] = None,
+    filter_keep: Union[None, dict[str, dict[str, Any]]] = None,
+    filter_remove: Union[None, dict[str, dict[str, Any]]] = None,
+    meta_data: Union[None, dict[str, Any]] = None,
     time_format: str = "%Y",
-    convert_str: Union[bool, Dict[str, float]] = True,
+    convert_str: Union[bool, dict[str, float]] = True,
 ) -> pd.DataFrame:
     """Read a CSV file in wide format into the PRIMAP2 interchange format.
 
-    Columns can be renamed or filled with default values to match the PRIMAP2 structure.
-    Where we refer to "dimensions" in the parameter description below we mean the basic
-    dimension names without the added terminology (e.g. "area" not "area (ISO3)"). The
-    terminology information will be added by this function. You can not use the short
-    dimension names in the attributes (e.g. "cat" instead of "category").
+    Columns can be renamed or filled with default values to match the PRIMAP2
+    structure. Where we refer to "dimensions" in the parameter description below we
+    mean the basic dimension names without the added terminology (e.g. "area" not
+    "area (ISO3)"). The terminology information will be added by this function. You can
+    not use the short dimension names in the attributes (e.g. "cat" instead of
+    "category").
 
     TODO: Currently duplicate data points will not be detected.
 
     TODO: enable filtering through query strings
 
     TODO: enable specification of the entity terminology
 
@@ -743,37 +740,37 @@
         The keys are the dimension names and the values are the values for
         the dimensions. For secondary categories use a ``sec_cats__`` prefix.
 
     coords_terminologies : dict
         Dict defining the terminologies used for the different coordinates (e.g. ISO3
         for area). Only possible coordinates here are: area, category, scenario,
         entity, and secondary categories. For secondary categories use a ``sec_cats__``
-        prefix. All entries different from "area", "category", "scenario", "entity", and
-        ``sec_cats__<name>`` will raise a ValueError.
+        prefix. All entries different from "area", "category", "scenario", "entity",
+        and ``sec_cats__<name>`` will raise a ValueError.
 
     coords_value_mapping : dict, optional
         A dict with primap2 dimension names as keys. Values are dicts with input values
         as keys and output values as values. A standard use case is to map gas names
         from input data to the standardized names used in primap2.
         Alternatively a value can also be a function which transforms one CSV metadata
         value into the new metadata value.
         A third possibility is to give a string as a value, which defines a rule for
         translating metadata values. The only defined rule at the moment is "PRIMAP1"
         which can be used for the "category", "entity", and "unit" columns to translate
         from PRIMAP1 metadata to PRIMAP2 metadata.
 
     coords_value_filling : dict, optional
         A dict with primap2 dimension names as keys. These are the target columns where
-        values will be filled (or replaced). Vales are dicts with primap2 dimension names
-        as keys. These are the source columns. The values are dicts with source value -
-        target value mappings.
-        The value filling can do everything that the value mapping can, but while mapping
-        can only replace values within a column using information from that column, the
-        filing function can also fill or replace data based on values from a different
-        column.
+        values will be filled (or replaced). Vales are dicts with primap2 dimension
+        names as keys. These are the source columns. The values are dicts with source
+        value - target value mappings.
+        The value filling can do everything that the value mapping can, but while
+        mapping can only replace values within a column using information from that
+        column, the filing function can also fill or replace data based on values from
+        a different column.
         This can be used to e.g. fill missing category codes based on category names or
         to replace category codes which do not meet the terminology using the category
         names.
 
     filter_keep : dict, optional
         Dict defining filters of data to keep. Filtering is done before metadata
         mapping, so use original metadata values to define the filter. Column names are
@@ -787,15 +784,16 @@
         The names of the filters have no relevance.
 
     meta_data : dict, optional
         Meta data for the whole dataset. Will end up in the dataset-wide attrs. Allowed
         keys are "references", "rights", "contact", "title", "comment", "institution",
         and "history". Documentation about the format and meaning of the meta data can
         be found in the
-        `data format documentation <https://primap2.readthedocs.io/en/stable/data_format_details.html#dataset-attributes>`_.  # noqa: E501
+        `data format documentation <https://primap2.readthedocs.io/en/stable/\
+data_format_details.html#dataset-attributes>`_.
 
     time_format : str, optional
         strftime style format used to parse the time information for the data columns.
         Default: "%Y", which will match years.
 
     convert_str : bool or dict, optional (default: True)
         If set to false, string values in the data columns will be kept.
@@ -873,32 +871,36 @@
         copy_df=False,
     )
 
     return data
 
 
 def interchange_format_attrs_dict(
-    *, xr_attrs: dict, time_format: str, dimensions, additional_coordinates: dict = None
+    *,
+    xr_attrs: dict,
+    time_format: str,
+    dimensions,
+    additional_coordinates: Union[None, dict] = None,
 ) -> dict:
     metadata = {
         "attrs": xr_attrs,
         "time_format": time_format,
         "dimensions": {"*": dimensions.copy()},
     }
 
     if additional_coordinates:
         metadata["additional_coordinates"] = additional_coordinates
 
     return metadata
 
 
 def additional_coordinate_metadata(
-    add_coords_cols: Dict[str, List[str]],
-    coords_cols: Dict[str, str],
-    coords_terminologies: Dict[str, str],
+    add_coords_cols: dict[str, list[str]],
+    coords_cols: dict[str, str],
+    coords_terminologies: dict[str, str],
 ) -> dict:
     """Create the `additional_coordinates` dict and do a few consistency checks"""
 
     additional_coordinates = {}
     for coord in add_coords_cols:
         if coord in coords_terminologies:
             logger.error(
@@ -928,69 +930,68 @@
         else:
             additional_coordinates[coord] = add_coords_cols[coord][1]
 
     return additional_coordinates
 
 
 def check_mandatory_dimensions(
-    coords_cols: Dict[str, str],
-    coords_defaults: Dict[str, Any],
+    coords_cols: dict[str, str],
+    coords_defaults: dict[str, Any],
 ):
     """Check if all mandatory dimensions are specified."""
     for coord in INTERCHANGE_FORMAT_MANDATORY_COLUMNS:
         if coord not in coords_cols and coord not in coords_defaults:
             logger.error(
                 f"Mandatory dimension {coord!r} not found in coords_cols={coords_cols}"
                 f" or coords_defaults={coords_defaults}."
             )
             raise ValueError(f"Mandatory dimension {coord!r} not defined.")
 
 
 def check_overlapping_specifications(
-    coords_cols: Dict[str, str],
-    coords_defaults: Dict[str, Any],
+    coords_cols: dict[str, str],
+    coords_defaults: dict[str, Any],
 ):
     both = set(coords_cols.keys()).intersection(set(coords_defaults.keys()))
     if both:
         logger.error(
             f"{both!r} is given in coords_cols and coords_defaults, but"
             f" it must only be given in one of them."
         )
         raise ValueError(f"{both!r} given in coords_cols and coords_defaults.")
 
 
 def check_overlapping_specifications_add_cols(
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, Any],
+    coords_cols: dict[str, str],
+    add_coords_cols: dict[str, Any],
 ):
     cols_add = [val[0] for val in add_coords_cols.values()]
     both = set(coords_cols.values()).intersection(set(cols_add))
     if both:
         logger.error(
             f"columns {both!r} used for dimensions and additional coordinates, but"
             f" should be used in only one of them."
         )
         raise ValueError(f"{both!r} given in coords_cols and add_coords_cols.")
 
 
-def matches_time_format(value: str, time_format: str):
+def matches_time_format(value: str, time_format: str) -> bool:
     try:
         datetime.datetime.strptime(value, time_format)
         return True
     except ValueError:
         return False
 
 
 def read_wide_csv(
     filepath_or_buffer,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]] = None,
+    coords_cols: dict[str, str],
+    add_coords_cols: Union[None, dict[str, list[str]]] = None,
     time_format: str = "%Y",
-) -> (pd.DataFrame, List[str]):
-
+) -> tuple[pd.DataFrame, list[str]]:
     data = pd.read_csv(
         filepath_or_buffer,
     )
 
     # get all the columns that are actual data not metadata (usually the years)
     time_cols = [
         col for col in data.columns.values if matches_time_format(col, time_format)
@@ -1023,17 +1024,17 @@
         raise ValueError(f"Columns {missing} not found in CSV.")
 
     return data, time_cols
 
 
 def read_long_csv(
     filepath_or_buffer,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]] = None,
-) -> (pd.DataFrame, List[str]):
+    coords_cols: dict[str, str],
+    add_coords_cols: Union[None, dict[str, list[str]]] = None,
+) -> pd.DataFrame:
     if "data" not in coords_cols.keys():
         raise ValueError(
             "No data column in the CSV specified in coords_cols, so nothing to read."
         )
 
     if "time" in coords_cols:
         parse_dates = [coords_cols["time"]]
@@ -1052,15 +1053,15 @@
         parse_dates=parse_dates,
         usecols=usecols,
     )
 
     return data
 
 
-def spec_to_query_string(filter_spec: Dict[str, Union[list, Any]]) -> str:
+def spec_to_query_string(filter_spec: dict[str, Any]) -> str:
     """Convert filter specification to query string.
 
     All column conditions in the filter are combined with &."""
     queries = []
     for col in filter_spec:
         if isinstance(filter_spec[col], list):
             itemlist = ", ".join(repr(x) for x in filter_spec[col])
@@ -1070,16 +1071,16 @@
         queries.append(filter_query)
 
     return " & ".join(queries)
 
 
 def filter_data(
     data: pd.DataFrame,
-    filter_keep: Optional[Dict[str, Dict[str, Any]]] = None,
-    filter_remove: Optional[Dict[str, Dict[str, Any]]] = None,
+    filter_keep: Union[None, dict[str, dict[str, Any]]] = None,
+    filter_remove: Union[None, dict[str, dict[str, Any]]] = None,
 ):
     # Filters for keeping data are combined with "or" so that
     # everything matching at least one rule is kept.
     if filter_keep:
         queries = []
         for filter_spec in filter_keep.values():
             q = spec_to_query_string(filter_spec)
@@ -1099,16 +1100,16 @@
 
     data.reset_index(drop=True, inplace=True)
 
 
 def fill_from_other_col(
     df: pd.DataFrame,
     *,
-    coords_value_filling: Dict[str, Dict[str, Dict[str, str]]],
-    attrs: Dict[str, Any],
+    coords_value_filling: dict[str, dict[str, dict[str, str]]],
+    attrs: dict[str, Any],
 ) -> pd.DataFrame:
     """
     This function fills value in one column based on values in other columns.
     It can be used to fill NaN values or to replace e.g. non-standard or
     non-unique category codes based on category names. It operates on pandas
     DataFrames.
 
@@ -1150,15 +1151,15 @@
                     df[source_col_name] == source_value, target_col_name
                 ] = mapping_info[source_value]
     return df
 
 
 def add_dimensions_from_defaults(
     data: pd.DataFrame,
-    coords_defaults: Dict[str, Any],
+    coords_defaults: dict[str, Any],
     additional_allowed_coords: Iterable[str] = (),
 ):
     if_columns = (
         INTERCHANGE_FORMAT_OPTIONAL_COLUMNS
         + INTERCHANGE_FORMAT_MANDATORY_COLUMNS
         + list(additional_allowed_coords)
     )
@@ -1172,16 +1173,16 @@
                 f"{SEC_CATS_PREFIX!r} to add a secondary category."
             )
 
 
 def map_metadata(
     data: pd.DataFrame,
     *,
-    meta_mapping: Dict[str, Union[str, Callable, dict]],
-    attrs: Dict[str, Any],
+    meta_mapping: dict[str, Union[str, Callable, dict]],
+    attrs: dict[str, Any],
 ):
     """Map the metadata according to specifications given in meta_mapping.
     First map entity, then the rest."""
     meta_mapping_copy = meta_mapping.copy()
     if "entity" in meta_mapping.keys():
         meta_mapping_entity = dict(entity=meta_mapping_copy["entity"])
         meta_mapping_copy.pop("entity")
@@ -1189,16 +1190,16 @@
 
     map_metadata_unordered(data, meta_mapping=meta_mapping_copy, attrs=attrs)
 
 
 def map_metadata_unordered(
     data: pd.DataFrame,
     *,
-    meta_mapping: Dict[str, Union[str, Callable, dict]],
-    attrs: Dict[str, Any],
+    meta_mapping: dict[str, Union[str, Callable, dict]],
+    attrs: dict[str, Any],
 ):
     """Map the metadata according to specifications given in meta_mapping."""
     dim_aliases = _alias_selection.translations_from_attrs(attrs, include_entity=True)
 
     # TODO: add additional mapping functions here
     # values: (function, additional arguments)
     mapping_functions = {
@@ -1223,29 +1224,29 @@
                 except KeyError:
                     logger.error(
                         f"Unknown metadata mapping {mapping!r} for column {column!r}, "
                         f"known mappings are: {list(mapping_functions.keys())}."
                     )
                     raise ValueError(
                         f"Unknown metadata mapping {mapping!r} for column {column!r}."
-                    )
+                    ) from None
             else:
                 func = mapping
                 args = []
 
             if not args:  # simple case: no additional args needed
                 values_to_map = data[column_name].unique()
                 values_mapped = map(func, values_to_map)
                 meta_mapping_df[column_name] = dict(zip(values_to_map, values_mapped))
 
             else:  # need to supply additional arguments
                 # this can't be handled using the replace()-call later since the
                 # mapped values don't depend on the original values only, therefore
                 # we do it directly
-                sel = [column_name] + args
+                sel = [column_name, *args]
                 values_to_map = np.unique(data[sel].to_records(index=False))
                 for vals_to_map in values_to_map:
                     # we replace values where all the arguments match - build a
                     # selector for that, then do the replacement
                     selector = data[column_name] == vals_to_map[0]
                     for i, arg in enumerate(args):
                         selector &= data[arg] == vals_to_map[i + 1]
@@ -1256,18 +1257,18 @@
             meta_mapping_df[column_name] = mapping
 
     data.replace(meta_mapping_df, inplace=True)
 
 
 def rename_columns(
     data: pd.DataFrame,
-    coords_cols: Dict[str, str],
-    add_coords_cols: Dict[str, List[str]],
-    coords_defaults: Dict[str, Any],
-    coords_terminologies: Dict[str, str],
+    coords_cols: dict[str, str],
+    add_coords_cols: dict[str, list[str]],
+    coords_defaults: dict[str, Any],
+    coords_terminologies: dict[str, str],
 ) -> dict:
     """Rename columns to match PRIMAP2 specifications and generate the corresponding
     dataset-wide attrs for PRIMAP2."""
 
     attr_names = {"category": "cat", "scenario": "scen", "area": "area"}
 
     attrs = {}
@@ -1317,15 +1318,15 @@
         return True
     except ValueError:
         return False
 
 
 def find_str_values_in_data(
     data: pd.DataFrame,
-    columns: List[str],
+    columns: list[str],
 ) -> list:
     """Find all string values occurring in given columns of a DataFrame"""
     # limit our analysis to columns that contain strings
     # (or other object types)
     cols_with_strs = (
         data[columns].select_dtypes(include=[object]).columns.values.tolist()
     )
@@ -1350,17 +1351,17 @@
         return 0
     if "NE" in parts or "NA" in parts:
         return np.nan
     raise ValueError(f"Could not parse code: {code!r}.")
 
 
 def create_str_replacement_dict(
-    strs: List[str],
-    user_str_conv: Dict[str, str] = {},
-) -> Dict[str, str]:
+    strs: list[str],
+    user_str_conv: Union[bool, dict[str, float]],
+) -> dict[str, str]:
     """Create a dict for replacement of strings by NaN and 0 based on
     general rules and user defined rules"""
 
     if isinstance(user_str_conv, bool):
         if user_str_conv:
             user_str_conv = {}
     elif isinstance(user_str_conv, dict):
@@ -1377,23 +1378,23 @@
             mapping[str_val] = user_str_conv[str_val]
         else:
             mapping[str_val] = parse_code(str_val)
 
     return mapping
 
 
-def replace_values(data: pd.DataFrame, columns: List[str], na_repl_dict):
+def replace_values(data: pd.DataFrame, columns: list[str], na_repl_dict):
     """Replace str values indicating not-a-number by float NaN."""
     for col in columns:
         data[col] = data[col].replace(na_repl_dict)
         data[col] = pd.to_numeric(data[col], errors="coerce")
         data[col] = data[col].astype("float64", copy=False, errors="ignore")
 
 
-def preferred_unit(entity: str, units: List[str], gwp_to_use: Optional[str]) -> str:
+def preferred_unit(entity: str, units: list[str], gwp_to_use: Union[None, str]) -> str:
     """Choose the preferred unit for the given entity.
 
     In general, "Gg <substance> / year" will be preferred if it is compatible with the
     given input units. Otherwise, the first unit from units will be preferred.
 
     Parameters
     ----------
@@ -1441,16 +1442,16 @@
 
     return unit_fallback
 
 
 def harmonize_units(
     data: pd.DataFrame,
     *,
-    unit_col: str = None,
-    attrs: Optional[dict] = None,
+    unit_col: Union[None, str] = None,
+    attrs: Union[None, dict] = None,
     dimensions: Iterable[str],
 ) -> None:
     """Harmonize the units of the input data.
 
     For each entity, convert all time series to the same unit (the unit that occurs
     first). Units must already be in PRIMAP2 style.
 
@@ -1492,15 +1493,15 @@
     entities = data[entity_col].unique()
     # print(entities)
     for entity in entities:
         # check if GWP given in entity
         gwp_match = re.findall(r"\(([A-Z0-9]*)\)$", entity)
         if gwp_match:
             gwp_to_use = gwp_match[0]
-            basic_entity = re.findall(r"^[^\(\)\s]*", entity)
+            basic_entity = re.findall(r"^[^()\s]*", entity)
             basic_entity = basic_entity[0]
         else:
             gwp_to_use = None
             basic_entity = entity
         # print(f"basic_entity: {basic_entity}")
         # get all units for this entity
         data_this_entity = data.loc[data[entity_col] == entity]
@@ -1511,16 +1512,16 @@
             unit_to = preferred_unit(basic_entity, units_this_entity, gwp_to_use)
 
             # if len(units_this_entity) > 1:
             for unit in units_this_entity:
                 if unit != unit_to:
                     # print(f"Working on unit {unit}")
                     unit_pint = ureg[unit]
-                    # could add a try except block here to throw and log an error or add
-                    # error info in DF instead of crashing
+                    # could add a try except block here to throw and log an error or
+                    # add error info in DF instead of crashing
                     if gwp_to_use:
                         with ureg.context(gwp_to_use):
                             unit_pint = unit_pint.to(unit_to)
                     else:
                         unit_pint = unit_pint.to(unit_to)
                     # print(f"Pint unit is {unit_pint}")
                     factor = unit_pint.magnitude
@@ -1534,29 +1535,29 @@
                         strs = find_str_values_in_data(data, data_cols)
                         logger.error(
                             f"The following string values are present and can "
                             f"not be converted during unit conversion: {strs}."
                         )
                         raise ValueError(
                             f"String values {strs} prevent unit conversion."
-                        )
+                        ) from None
 
                     data.loc[mask, unit_col] = unit_to
 
             if gwp_to_use and unit_to not in units_this_entity:
                 # entity was converted
                 entity_mask = data[entity_col] == entity
                 # print(f"Changing entity from {entity} to {basic_entity}")
                 data.loc[entity_mask, entity_col] = basic_entity
 
 
 def sort_columns_and_rows(
     data: pd.DataFrame,
-    dimensions: Iterable[Hashable],
-) -> (pd.DataFrame, List[Hashable]):
+    dimensions: Iterable[str],
+) -> tuple[pd.DataFrame, list[str]]:
     """Sort the data.
 
     The columns are ordered according to the order in
     INTERCHANGE_FORMAT_COLUMN_ORDER, with secondary categories alphabetically after
     the category and all date columns in order at the end.
 
     The rows are ordered by values of the non-date columns.
```

### Comparing `primap2-0.9.5/primap2/pm2io/_interchange_format.py` & `primap2-0.9.6/primap2/pm2io/_interchange_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import csv
 import itertools
 import re
-import typing
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import strictyaml as sy
 import xarray as xr
@@ -80,15 +79,15 @@
     """
     empty_vars = (x for x in ds if ds[x].count() == 0)
     da = ds.drop_vars(empty_vars).to_array("time")
     da["time"] = pd.to_datetime(da["time"].values, format=time_format, exact=False)
     return da
 
 
-def metadata_for_variable(unit: str, variable: str) -> typing.Dict[str, str]:
+def metadata_for_variable(unit: str, variable: str) -> dict[str, str]:
     """Convert a primap2 unit and variable key to a metadata dict.
 
     Derives the information needed for the data variable's attrs dict from the unit
     and the variable's key.
     Takes GWP information from the variable name in primap2 style (if present).
 
     Parameters
@@ -119,16 +118,16 @@
 
     if gwp:
         attrs["gwp_context"] = gwp[0]
 
         regex_variable = r"^(.*)\s\([a-zA-z0-9]*\)$"
         entity = re.findall(regex_variable, variable)
         if not entity:
-            logger.error("Can't extract entity from " + variable)
-            raise ValueError("Can't extract entity from " + variable)
+            logger.error(f"Can't extract entity from {variable}")
+            raise ValueError(f"Can't extract entity from {variable}")
         attrs["entity"] = entity[0]
     else:
         attrs["entity"] = variable
     return attrs
 
 
 def write_interchange_format(
@@ -311,15 +310,15 @@
         if entity not in dtypes:
             dtypes[entity] = "float"
 
     # check resulting shape to estimate memory consumption
     dim_lens = {dim: len(np.unique(data_xr[dim].dropna("index"))) for dim in index_cols}
     dim_lens["time"] = len(time_cols)
     shapes = []
-    for entity, dims in dimensions.items():
+    for _, dims in dimensions.items():
         shapes.append([dim_lens[dim] for dim in dims if dim != "unit"])
     array_size = sum(np.product(shape) for shape in shapes)
     logger.debug(f"Expected array shapes: {shapes}, resulting in size {array_size:,}.")
     if array_size > max_array_size:
         logger.error(
             f"Set with {len(shapes)} entities and a total of {len(index_cols)} "
             f"dimensions will have a size of {array_size:,} "
@@ -341,15 +340,15 @@
         da_entity = da.loc[{entity_col: entity}]
         # we still have a full MultiIndex, so trim it to the relevant dimensions
         da_entity = da_entity.reset_index(list(index_cols - set(dims)), drop=True)
         # depending on the version of xarray, an atomic, 0-dimensional coord
         # for the entity remains. we have to remove it to be able to combine the
         # dataset afterwards.
         if entity_col in da_entity.coords:
-            da_entity = da_entity.drop(entity_col)
+            da_entity = da_entity.drop_vars(entity_col)
         # now we can safely unstack the index
         data_vars[entity] = da_entity.unstack("index").astype(dtypes[entity])
 
     data_xr = xr.Dataset(data_vars)
 
     # add the additional coordinates
     for coord in attrs["additional_coordinates"].keys():
```

### Comparing `primap2-0.9.5/primap2/tests/conftest.py` & `primap2-0.9.6/primap2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv` & `primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc` & `primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml` & `primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/data/test_from_interchange_format_output.nc` & `primap2-0.9.6/primap2/tests/data/test_from_interchange_format_output.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc` & `primap2-0.9.6/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/examples.py` & `primap2-0.9.6/primap2/tests/examples.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_aggregate.py` & `primap2-0.9.6/primap2/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_alias_selection.py` & `primap2-0.9.6/primap2/tests/test_alias_selection.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_conversion.py` & `primap2-0.9.6/primap2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_data_format.py` & `primap2-0.9.6/primap2/tests/test_data_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_data_reading.py` & `primap2-0.9.6/primap2/tests/test_data_reading.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
         coords_defaults,
         coords_terminologies,
         coords_value_mapping,
     ):
         file_input = DATA_PATH / "test_csv_data.csv"
         file_expected = DATA_PATH / "test_read_wide_csv_file_no_sec_cats.csv"
         df_expected: pd.DataFrame = pd.read_csv(file_expected, index_col=0)
-        df_expected.rename(columns={"entity": "entity (PRIMAP1)"}, inplace=True)
+        df_expected = df_expected.rename(columns={"entity": "entity (PRIMAP1)"})
 
         del coords_cols["sec_cats__Class"]
         del coords_defaults["sec_cats__Type"]
         del coords_terminologies["sec_cats__Class"]
         del coords_terminologies["sec_cats__Type"]
 
         coords_terminologies["entity"] = "PRIMAP1"
```

### Comparing `primap2-0.9.5/primap2/tests/test_downscale.py` & `primap2-0.9.6/primap2/tests/test_downscale.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_interchange_format.py` & `primap2-0.9.6/primap2/tests/test_interchange_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_merge.py` & `primap2-0.9.6/primap2/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_metadata.py` & `primap2-0.9.6/primap2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_overview.py` & `primap2-0.9.6/primap2/tests/test_overview.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/test_setters.py` & `primap2-0.9.6/primap2/tests/test_setters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Tests for _setters.py"""
 
 import re
-import typing
 
 import numpy as np
 import pint
 import pytest
 import xarray as xr
 
 from primap2 import ureg
@@ -29,23 +28,23 @@
 
 @pytest.fixture
 def co2() -> pint.Unit:
     return ureg("Gg CO2 / year")
 
 
 @pytest.fixture(params=["fillna_empty", "error", "fillna", "overwrite", None])
-def existing(request) -> typing.Dict[str, str]:
+def existing(request) -> dict[str, str]:
     if request.param is not None:
         return {"existing": request.param}
     else:
         return {}
 
 
 @pytest.fixture(params=["error", "extend", None])
-def new(request) -> typing.Dict[str, str]:
+def new(request) -> dict[str, str]:
     if request.param is not None:
         return {"new": request.param}
     else:
         return {}
 
 
 class TestDASetter:
@@ -57,15 +56,15 @@
                 " insert new values into dim."
             ),
         ):
             da.pr.set("area", "CUB", ts * co2, new="error", **existing)
 
     def test_new_works(self, da: xr.DataArray, ts, co2, existing):
         actual = da.pr.set("area", ["CUB"], 2 * ts * co2, new="extend", **existing)
-        expected = da.reindex({"area (ISO3)": list(da["area (ISO3)"].values) + ["CUB"]})
+        expected = da.reindex({"area (ISO3)": [*da["area (ISO3)"].values, "CUB"]})
         expected.loc[{"area (ISO3)": "CUB"}] = ts[..., np.newaxis] * 2 * co2
         assert_aligned_equal(actual, expected)
 
     def test_exists_default_error(
         self, da: xr.DataArray, ts: np.ndarray, co2: pint.Unit, new
     ):
         with pytest.raises(
@@ -128,15 +127,15 @@
     def test_mixed_default(self, da: xr.DataArray, ts: np.ndarray, co2: pint.Unit):
         da.loc[{"area (ISO3)": "COL"}] = np.nan
         actual = da.pr.set(
             "area",
             ["COL", "CUB"],
             np.array([ts, 2 * ts]).T * co2,
         )
-        expected = da.reindex({"area (ISO3)": list(da["area (ISO3)"].values) + ["CUB"]})
+        expected = da.reindex({"area (ISO3)": [*da["area (ISO3)"].values, "CUB"]})
         expected.loc[{"area (ISO3)": "COL"}] = ts[..., np.newaxis] * co2
         expected.loc[{"area (ISO3)": "CUB"}] = ts[..., np.newaxis] * 2 * co2
         assert_aligned_equal(actual, expected)
 
     def test_mixed_error(self, da: xr.DataArray, ts: np.ndarray, co2: pint.Unit):
         with pytest.raises(
             ValueError,
@@ -155,15 +154,15 @@
     def test_mixed_overwrite(self, da: xr.DataArray, ts: np.ndarray, co2: pint.Unit):
         actual = da.pr.set(
             "area",
             ["COL", "CUB"],
             np.array([ts, 2 * ts]).T * co2,
             existing="overwrite",
         )
-        expected = da.reindex({"area (ISO3)": list(da["area (ISO3)"].values) + ["CUB"]})
+        expected = da.reindex({"area (ISO3)": [*da["area (ISO3)"].values, "CUB"]})
         expected.loc[{"area (ISO3)": "COL"}] = ts[..., np.newaxis] * co2
         expected.loc[{"area (ISO3)": "CUB"}] = ts[..., np.newaxis] * 2 * co2
         assert_aligned_equal(actual, expected)
 
         # with explicit value_dims
         actual = da.pr.set(
             "area",
@@ -179,23 +178,23 @@
         tda.loc[{"area (ISO3)": "COL", "time": "2009"}] = np.nan * co2
         actual = tda.pr.set(
             "area",
             ["COL", "CUB"],
             np.array([ts, 2 * ts]).T * co2,
             existing="fillna",
         )
-        expected = da.reindex({"area (ISO3)": list(da["area (ISO3)"].values) + ["CUB"]})
+        expected = da.reindex({"area (ISO3)": [*da["area (ISO3)"].values, "CUB"]})
         expected.loc[{"area (ISO3)": "COL", "time": "2009"}] = 9 * co2
         expected.loc[{"area (ISO3)": "CUB"}] = ts[..., np.newaxis] * 2 * co2
         assert_aligned_equal(actual, expected)
 
     def test_new_from_array(self, da: xr.DataArray, ts: np.ndarray, co2: pint.Unit):
         # with scalar dimension
         actual = da.pr.set("area", "CUB", 2 * da.pr.loc[{"area": "COL"}])
-        expected = da.reindex({"area (ISO3)": list(da["area (ISO3)"].values) + ["CUB"]})
+        expected = da.reindex({"area (ISO3)": [*da["area (ISO3)"].values, "CUB"]})
         expected = expected.fillna(expected.loc[{"area (ISO3)": "COL"}] * 2)
         assert_aligned_equal(actual, expected)
 
         actual_error = da.pr.set(
             "area", "CUB", 2 * da.pr.loc[{"area": "COL"}], existing="error"
         )
         assert_aligned_equal(actual_error, expected)
@@ -206,15 +205,15 @@
 
     def test_mixed_from_data_array_overwrite(
         self, da: xr.DataArray, ts: np.ndarray, co2: pint.Unit
     ):
         actual = da.pr.set(
             "area", ["CUB", "COL"], 2 * da.pr.loc[{"area": "COL"}], existing="overwrite"
         )
-        expected = da.reindex({"area (ISO3)": list(da["area (ISO3)"].values) + ["CUB"]})
+        expected = da.reindex({"area (ISO3)": [*da["area (ISO3)"].values, "CUB"]})
         expected.loc[{"area (ISO3)": "COL"}] = np.nan
         expected = expected.fillna(da.loc[{"area (ISO3)": "COL"}] * 2)
         assert_aligned_equal(actual, expected)
 
     @pytest.fixture
     def mda(self):
         return xr.DataArray(
@@ -378,15 +377,15 @@
 
 class TestDsSetter:
     def test_new(self, minimal_ds: xr.Dataset, existing):
         actual = minimal_ds.pr.set(
             "area", "CUB", minimal_ds.pr.loc[{"area": "COL"}] * 2, **existing
         )
         expected = minimal_ds.reindex(
-            {"area (ISO3)": list(minimal_ds["area (ISO3)"].values) + ["CUB"]}
+            {"area (ISO3)": [*minimal_ds["area (ISO3)"].values, "CUB"]}
         )
         for key in expected.keys():
             expected[key] = expected[key].fillna(
                 expected[key].pr.loc[{"area": "COL"}] * 2
             )
         assert_ds_aligned_equal(actual, expected)
 
@@ -448,15 +447,15 @@
 
     def test_inhomogeneous(self, minimal_ds: xr.Dataset):
         minimal_ds["population"] = minimal_ds["CO2"].pr.dequantify().sum("area (ISO3)")
         actual = minimal_ds.pr.set(
             "area", "CUB", minimal_ds.pr.loc[{"area": "COL"}] * 2
         )
         expected = minimal_ds.reindex(
-            {"area (ISO3)": list(minimal_ds["area (ISO3)"].values) + ["CUB"]}
+            {"area (ISO3)": [*minimal_ds["area (ISO3)"].values, "CUB"]}
         )
         for key in expected.keys():
             if key == "population":
                 continue
             expected[key] = expected[key].fillna(
                 expected[key].pr.loc[{"area": "COL"}] * 2
             )
```

### Comparing `primap2-0.9.5/primap2/tests/test_units.py` & `primap2-0.9.6/primap2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/primap2/tests/utils.py` & `primap2-0.9.6/primap2/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import typing
-
 import numpy as np
 import pint
 import xarray as xr
 
 
 def allclose(a: xr.DataArray, b: xr.DataArray, *args, **kwargs) -> bool:
     """Like np.allclose, but converts a to b's units before comparing."""
@@ -20,17 +18,15 @@
 def assert_equal(a: xr.DataArray, b: xr.DataArray, *args, **kwargs):
     """Asserts that contents are allclose(), and the name and attrs are also equal."""
     assert allclose(a, b, *args, **kwargs)
     assert a.attrs == b.attrs, (a.attrs, b.attrs)
     assert a.name == b.name, (a.name, b.name)
 
 
-def assert_align(
-    a: xr.DataArray, b: xr.DataArray
-) -> typing.Tuple[xr.DataArray, xr.DataArray]:
+def assert_align(a: xr.DataArray, b: xr.DataArray) -> tuple[xr.DataArray, xr.DataArray]:
     """Asserts that a and b have the same shape and returns a and b with axes and
     dimensions aligned and sorted equally so that naive comparisons can be done."""
     assert set(a.dims) == set(b.dims), (a.dims, b.dims)
     aa, ba = xr.align(a, b, join="outer")
     aa = aa.transpose(*ba.dims)
     size_unchanged = sorted(aa.shape) == sorted(a.shape) and ba.shape == b.shape
     assert size_unchanged, (a.shape, b.shape)
```

### Comparing `primap2-0.9.5/primap2.egg-info/PKG-INFO` & `primap2-0.9.6/primap2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: primap2
-Version: 0.9.5
+Version: 0.9.6
 Summary: The next generation of the PRIMAP climate policy analysis suite.
 Home-page: https://github.com/pik-primap/primap2
 Author: Mika Pflüger
-Author-email: mika.pflueger@pik-potsdam.de
+Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://primap2.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: datalad
 License-File: LICENSE
 
 =======
@@ -58,15 +57,17 @@
 ------
 
 PRIMAP2 is in active development, and not everything promised above is built
 yet.
 
 License
 -------
-Copyright 2020-2021, Potsdam-Institut für Klimafolgenforschung e.V.
+Copyright 2020-2022, Potsdam-Institut für Klimafolgenforschung e.V.
+
+Copyright 2023, Climate Resource Pty Ltd
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this
 file except in compliance with the License. You may obtain a copy of the License at
 
 https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under
@@ -78,22 +79,29 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2022-12-13).
-pik-primap/primap2: PRIMAP2 Version 0.9.5.
-Zenodo. https://doi.org/10.5281/zenodo.7434154
+Mika Pflüger and Johannes Gütschow. (2023-04-28).
+pik-primap/primap2: PRIMAP2 Version 0.9.6.
+Zenodo. https://doi.org/10.5281/zenodo.7875234
 
 =========
 Changelog
 =========
 
+0.9.6
+-----
+* Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
+* stop building pdf output documentation, it doesn't support SVG and isn't used much.
+* Drop support for Python version 3.8 to prepare for it being dropped
+  in Numpy on April 14.
+
 0.9.5
 -----
 * pr.merge: use xarray's combine_first instead of own algorithm for better performance.
 * Fix in nan handling of to_interchange_format
 * made regexp_unit optional in nir_add_unit_information as intended already before
 * Add support for Python 3.11
```

### Comparing `primap2-0.9.5/primap2.egg-info/SOURCES.txt` & `primap2-0.9.6/primap2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/rosetta/combine_rows-set.ipynb` & `primap2-0.9.6/rosetta/combine_rows-set.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/setup.cfg` & `primap2-0.9.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 [metadata]
 name = primap2
-version = 0.9.5
+version = 0.9.6
 author = Mika Pflüger
-author_email = mika.pflueger@pik-potsdam.de
+author_email = mika.pflueger@climate-resource.com
 description = The next generation of the PRIMAP climate policy analysis suite.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/primap2
 project_urls = 
 	Documentation = https://primap2.readthedocs.io/
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 license = Apache Software License 2.0
 license_file = LICENSE
 
 [options]
 packages = 
 	primap2
 	primap2.pm2io
 	primap2.tests
 	primap2.tests.data
-python_requires = >=3.8
+python_requires = >=3.9
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	xarray
 	pint>=0.20.1
 	pint_xarray>=0.2
 	numpy
 	pandas
-	openscm_units>=0.3
+	openscm_units>=0.5.1
 	loguru
 	scipy
 	h5netcdf>=0.10
 	h5py
 	bottleneck
 	matplotlib
 	ruamel.yaml
@@ -81,20 +80,14 @@
 	datalad
 
 [options.package_data]
 * = 
 	*.csv
 	*.nc
 
-[flake8]
-exclude = docs
-max-line-length = 88
-extend-ignore = E203, W503
-per-file-ignores = primap2/__init__.py:F401
-
 [doc8]
 max-line-length = 88
 ignore-path-errors = docs/data_format_details.rst;D001,docs/interchange_format_details.rst;D001
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `primap2-0.9.5/tbump.toml` & `primap2-0.9.6/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/primap2/"
 
 [version]
-current = "0.9.5"
+current = "0.9.6"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `primap2-0.9.5/update_changelog.py` & `primap2-0.9.6/update_changelog.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.5/update_citation_info.py` & `primap2-0.9.6/update_citation_info.py`

 * *Files identical despite different names*

