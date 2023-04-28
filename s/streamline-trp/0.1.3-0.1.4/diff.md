# Comparing `tmp/streamline_trp-0.1.3.tar.gz` & `tmp/streamline_trp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamline_trp-0.1.3.tar", max compression
+gzip compressed data, was "streamline_trp-0.1.4.tar", max compression
```

## Comparing `streamline_trp-0.1.3.tar` & `streamline_trp-0.1.4.tar`

### file list

```diff
@@ -1,75 +1,11 @@
--rw-r--r--   0        0        0    10142 2023-03-17 18:20:00.409140 streamline_trp-0.1.3/LICENSE
--rw-r--r--   0        0        0     2384 2023-03-17 18:20:00.409292 streamline_trp-0.1.3/README.md
--rw-r--r--   0        0        0      352 2023-04-06 21:32:41.439484 streamline_trp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      111 2023-03-17 18:20:00.432328 streamline_trp-0.1.3/src-python/.style.yapf
--rw-r--r--   0        0        0        0 2023-03-17 18:20:00.432439 streamline_trp-0.1.3/src-python/.yapfignore
--rw-r--r--   0        0        0    10299 2023-03-17 18:20:00.432705 streamline_trp-0.1.3/src-python/README.md
--rw-r--r--   0        0        0     3320 2023-03-17 18:20:00.432973 streamline_trp-0.1.3/src-python/a2i/README.md
--rw-r--r--   0        0        0      109 2023-04-06 21:22:22.239450 streamline_trp-0.1.3/src-python/a2i/__init__.py
--rw-r--r--   0        0        0   136560 2023-03-17 18:20:00.433874 streamline_trp-0.1.3/src-python/a2i/a2i-response.json
--rw-r--r--   0        0        0     7188 2023-03-17 18:20:00.434100 streamline_trp-0.1.3/src-python/a2i/a2irp.py
--rw-r--r--   0        0        0     1355 2023-03-17 18:20:00.434257 streamline_trp-0.1.3/src-python/a2i/a2irptest.py
--rwxr-xr-x   0        0        0     1696 2023-03-17 18:20:00.434451 streamline_trp-0.1.3/src-python/bin/amazon-textract-pipeline
--rw-r--r--   0        0        0    25767 2023-03-18 21:18:38.031244 streamline_trp-0.1.3/src-python/dist/streamline_trp-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0    25597 2023-03-18 21:18:37.987679 streamline_trp-0.1.3/src-python/dist/streamline_trp-0.1.0.tar.gz
--rw-r--r--   0        0        0    25766 2023-03-18 21:19:23.543250 streamline_trp-0.1.3/src-python/dist/streamline_trp-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0    25602 2023-03-18 21:19:23.499935 streamline_trp-0.1.3/src-python/dist/streamline_trp-0.1.1.tar.gz
--rw-r--r--   0        0        0        7 2023-03-17 18:20:00.434627 streamline_trp-0.1.3/src-python/extras/dev.txt
--rw-r--r--   0        0        0      467 2023-04-06 21:22:22.239907 streamline_trp-0.1.3/src-python/setup.cfg
--rw-r--r--   0        0        0     1950 2023-04-06 21:22:22.240255 streamline_trp-0.1.3/src-python/setup.py
--rw-r--r--   0        0        0   487699 2023-03-17 18:20:00.436858 streamline_trp-0.1.3/src-python/tests/data/180-degree-roation.json
--rw-r--r--   0        0        0   274499 2023-04-06 21:22:22.241560 streamline_trp-0.1.3/src-python/tests/data/2023-Q2-table-model-sample.json
--rw-r--r--   0        0        0   997174 2023-03-17 18:20:00.446648 streamline_trp-0.1.3/src-python/tests/data/all_features_with_floating_title_header.json
--rw-r--r--   0        0        0   158398 2023-03-17 18:20:00.447057 streamline_trp-0.1.3/src-python/tests/data/employment-application.json
--rw-r--r--   0        0        0   359047 2023-03-17 18:20:00.448928 streamline_trp-0.1.3/src-python/tests/data/gib.json
--rw-r--r--   0        0        0   263699 2023-03-17 18:20:00.450496 streamline_trp-0.1.3/src-python/tests/data/gib1.json
--rw-r--r--   0        0        0   160332 2023-03-17 18:20:00.451354 streamline_trp-0.1.3/src-python/tests/data/gib_10_degrees.json
--rw-r--r--   0        0        0   160332 2023-03-17 18:20:00.452342 streamline_trp-0.1.3/src-python/tests/data/gib__10_degrees.json
--rw-r--r--   0        0        0   155889 2023-03-17 18:20:00.453178 streamline_trp-0.1.3/src-python/tests/data/gib__15_degrees.json
--rw-r--r--   0        0        0   165128 2023-03-17 18:20:00.453954 streamline_trp-0.1.3/src-python/tests/data/gib__180_degrees.json
--rw-r--r--   0        0        0   144206 2023-03-17 18:20:00.454733 streamline_trp-0.1.3/src-python/tests/data/gib__25_degrees.json
--rw-r--r--   0        0        0   162677 2023-03-17 18:20:00.455545 streamline_trp-0.1.3/src-python/tests/data/gib__270_degrees.json
--rw-r--r--   0        0        0   157929 2023-03-17 18:20:00.456286 streamline_trp-0.1.3/src-python/tests/data/gib__90_degrees.json
--rw-r--r--   0        0        0   164235 2023-03-17 18:20:00.457149 streamline_trp-0.1.3/src-python/tests/data/gib__minus_10_degrees.json
--rw-r--r--   0        0        0   602412 2023-03-17 18:20:00.459657 streamline_trp-0.1.3/src-python/tests/data/gib_multi_page_table_merge.json
--rw-r--r--   0        0        0   257271 2023-03-17 18:20:00.460834 streamline_trp-0.1.3/src-python/tests/data/gib_multi_page_tables.json
--rw-r--r--   0        0        0    90704 2023-03-17 18:20:00.461305 streamline_trp-0.1.3/src-python/tests/data/gib_multi_tables_multi_page_sample.json
--rw-r--r--   0        0        0   805976 2023-03-17 18:20:00.462288 streamline_trp-0.1.3/src-python/tests/data/in-table-footer.json
--rw-r--r--   0        0        0   244517 2023-03-17 18:20:00.463197 streamline_trp-0.1.3/src-python/tests/data/in-table-title.json
--rw-r--r--   0        0        0  1653784 2023-03-17 18:20:00.465824 streamline_trp-0.1.3/src-python/tests/data/lending-doc-output.json
--rw-r--r--   0        0        0    45693 2023-03-17 18:20:00.466215 streamline_trp-0.1.3/src-python/tests/data/lending-package-no-signature.json
--rw-r--r--   0        0        0   256534 2023-03-17 18:20:00.467446 streamline_trp-0.1.3/src-python/tests/data/multi-page-forms-samples-2-page.json
--rw-r--r--   0        0        0    90704 2023-03-17 18:20:00.467958 streamline_trp-0.1.3/src-python/tests/data/multi-tables-multi-page-sample.json
--rw-r--r--   0        0        0   336672 2023-03-17 18:20:00.468664 streamline_trp-0.1.3/src-python/tests/data/patient_intake_form_sample.json
--rw-r--r--   0        0        0   631429 2023-03-17 18:20:00.472547 streamline_trp-0.1.3/src-python/tests/data/paystub_with_signature.json
--rw-r--r--   0        0        0   411216 2023-03-17 18:20:00.474475 streamline_trp-0.1.3/src-python/tests/data/queries_sample.json
--rw-r--r--   0        0        0   902193 2023-04-06 21:22:22.247282 streamline_trp-0.1.3/src-python/tests/data/request_for_verification_of_employment.json
--rw-r--r--   0        0        0 36350978 2023-04-06 21:22:22.421604 streamline_trp-0.1.3/src-python/tests/data/table-performance-pretty.json
--rw-r--r--   0        0        0   186485 2023-03-17 18:20:00.475154 streamline_trp-0.1.3/src-python/tests/data/tables_with_headers_and_merged_cells.json
--rw-r--r--   0        0        0   471384 2023-03-17 18:20:00.477328 streamline_trp-0.1.3/src-python/tests/data/tables_with_headers_out_of_order_cells.json
--rw-r--r--   0        0        0   276147 2023-03-17 18:20:00.478786 streamline_trp-0.1.3/src-python/tests/data/tables_with_merged_cells_sample1.json
--rw-r--r--   0        0        0   287678 2023-03-17 18:20:00.479298 streamline_trp-0.1.3/src-python/tests/data/tables_with_merged_cells_sample2.json
--rw-r--r--   0        0        0     5022 2023-03-17 18:20:00.479473 streamline_trp-0.1.3/src-python/tests/data/test-trp2-analyzeid_sample_multi_page.json
--rw-r--r--   0        0        0     6523 2023-03-17 18:20:00.479637 streamline_trp-0.1.3/src-python/tests/data/test-trp2_analyzeid_sample1.json
--rw-r--r--   0        0        0   138932 2023-03-17 18:20:00.481085 streamline_trp-0.1.3/src-python/tests/data/test-trp2_analyzeid_sample1_with_OCR.json
--rw-r--r--   0        0        0       90 2023-03-17 18:20:00.481230 streamline_trp-0.1.3/src-python/tests/data/test-trp2_analyzeid_sample2.json
--rw-r--r--   0        0        0   160326 2023-03-17 18:20:00.482007 streamline_trp-0.1.3/src-python/tests/data/test_trp2_expense_sample1.json
--rw-r--r--   0        0        0    57770 2023-03-17 18:20:00.482330 streamline_trp-0.1.3/src-python/tests/data/test_trp2_expense_sample2.json
--rw-r--r--   0        0        0    95331 2023-03-17 18:20:00.482686 streamline_trp-0.1.3/src-python/tests/data/test_trp2_expense_sample3.json
--rw-r--r--   0        0        0   137121 2023-03-17 18:20:00.482986 streamline_trp-0.1.3/src-python/tests/data/test_trp2_expense_sample4.json
--rw-r--r--   0        0        0   186483 2023-03-17 18:20:00.483584 streamline_trp-0.1.3/src-python/tests/data/textract-new-tables-api.json
--rw-r--r--   0        0        0   142156 2023-03-17 18:20:00.483950 streamline_trp-0.1.3/src-python/tests/test-response.json
--rw-r--r--   0        0        0     1970 2023-03-17 18:20:00.484208 streamline_trp-0.1.3/src-python/tests/test_base_trp2.py
--rw-r--r--   0        0        0     6108 2023-04-06 21:22:22.422351 streamline_trp-0.1.3/src-python/tests/test_trp.py
--rw-r--r--   0        0        0    42476 2023-04-06 21:22:22.422795 streamline_trp-0.1.3/src-python/tests/test_trp2.py
--rw-r--r--   0        0        0     2668 2023-03-17 18:20:00.484674 streamline_trp-0.1.3/src-python/tests/test_trp2_analyzeid.py
--rw-r--r--   0        0        0     1041 2023-03-17 18:20:00.484808 streamline_trp-0.1.3/src-python/tests/test_trp2_expense.py
--rw-r--r--   0        0        0      786 2023-03-17 18:20:00.484928 streamline_trp-0.1.3/src-python/tests/test_trp2_lending.py
--rw-r--r--   0        0        0    20527 2023-04-06 21:22:22.423277 streamline_trp-0.1.3/src-python/trp/__init__.py
--rw-r--r--   0        0        0     9009 2023-04-06 21:22:22.423616 streamline_trp-0.1.3/src-python/trp/t_pipeline.py
--rw-r--r--   0        0        0     4899 2023-04-06 21:22:22.423974 streamline_trp-0.1.3/src-python/trp/t_tables.py
--rw-r--r--   0        0        0    39145 2023-04-06 21:22:50.162433 streamline_trp-0.1.3/src-python/trp/trp2.py
--rw-r--r--   0        0        0     7760 2023-04-06 20:57:51.510628 streamline_trp-0.1.3/src-python/trp/trp2_analyzeid.py
--rw-r--r--   0        0        0    14321 2023-04-06 20:57:51.511146 streamline_trp-0.1.3/src-python/trp/trp2_expense.py
--rw-r--r--   0        0        0     8225 2023-04-06 20:57:51.511745 streamline_trp-0.1.3/src-python/trp/trp2_lending.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 streamline_trp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-03-17 18:20:00.409140 streamline_trp-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2384 2023-03-17 18:20:00.409292 streamline_trp-0.1.4/README.md
+-rw-r--r--   0        0        0      356 2023-04-27 23:59:54.732895 streamline_trp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    20527 2023-04-27 23:59:41.126455 streamline_trp-0.1.4/src-python/trp/__init__.py
+-rw-r--r--   0        0        0     9009 2023-04-27 23:59:41.127322 streamline_trp-0.1.4/src-python/trp/t_pipeline.py
+-rw-r--r--   0        0        0     4899 2023-04-27 23:59:41.128000 streamline_trp-0.1.4/src-python/trp/t_tables.py
+-rw-r--r--   0        0        0    39145 2023-04-27 23:59:41.129006 streamline_trp-0.1.4/src-python/trp/trp2.py
+-rw-r--r--   0        0        0     7760 2023-04-06 20:57:51.510628 streamline_trp-0.1.4/src-python/trp/trp2_analyzeid.py
+-rw-r--r--   0        0        0    14321 2023-04-06 20:57:51.511146 streamline_trp-0.1.4/src-python/trp/trp2_expense.py
+-rw-r--r--   0        0        0     8225 2023-04-06 20:57:51.511745 streamline_trp-0.1.4/src-python/trp/trp2_lending.py
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 streamline_trp-0.1.4/PKG-INFO
```

### Comparing `streamline_trp-0.1.3/LICENSE` & `streamline_trp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/README.md` & `streamline_trp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/__init__.py` & `streamline_trp-0.1.4/src-python/trp/__init__.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/t_pipeline.py` & `streamline_trp-0.1.4/src-python/trp/t_pipeline.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/t_tables.py` & `streamline_trp-0.1.4/src-python/trp/t_tables.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/trp2.py` & `streamline_trp-0.1.4/src-python/trp/trp2.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/trp2_analyzeid.py` & `streamline_trp-0.1.4/src-python/trp/trp2_analyzeid.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/trp2_expense.py` & `streamline_trp-0.1.4/src-python/trp/trp2_expense.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/src-python/trp/trp2_lending.py` & `streamline_trp-0.1.4/src-python/trp/trp2_lending.py`

 * *Files identical despite different names*

### Comparing `streamline_trp-0.1.3/PKG-INFO` & `streamline_trp-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamline-trp
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Doug Qian
 Author-email: douglas@spirals.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

