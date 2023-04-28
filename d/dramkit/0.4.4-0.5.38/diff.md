# Comparing `tmp/dramkit-0.4.4.tar.gz` & `tmp/dramkit-0.5.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.4.4.tar", last modified: Wed Feb 15 01:28:22 2023, max compression
+gzip compressed data, was "dramkit-0.5.38.tar", last modified: Fri Apr 28 01:18:45 2023, max compression
```

## Comparing `dramkit-0.4.4.tar` & `dramkit-0.5.38.tar`

### file list

```diff
@@ -1,175 +1,187 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.684108 dramkit-0.4.4/
--rw-rw-rw-   0        0        0     1072 2022-04-24 03:14:10.000000 dramkit-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     1098 2023-02-15 01:28:22.683108 dramkit-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.338520 dramkit-0.4.4/dramkit/
--rw-rw-rw-   0        0        0      668 2022-10-20 01:51:03.000000 dramkit-0.4.4/dramkit/__init__.py
--rw-rw-rw-   0        0        0      661 2023-02-15 01:27:36.000000 dramkit-0.4.4/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.453223 dramkit-0.4.4/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.4.4/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.4.4/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.4.4/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.4.4/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0     1917 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_AES.py
--rw-rw-rw-   0        0        0     1308 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_AES_CBC.py
--rw-rw-rw-   0        0        0     1117 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_AES_ECB.py
--rw-rw-rw-   0        0        0     1158 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_AES_ECB2.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.4.4/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.4.4/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.4.4/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.4.4/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.4.4/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.4.4/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.4.4/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.4.4/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1077 2022-05-13 12:32:03.000000 dramkit-0.4.4/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.4.4/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.4.4/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.4.4/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl.py
--rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl2.py
--rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl3.py
--rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl4.py
--rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl5.py
--rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl6.py
--rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_rl7.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.461248 dramkit-0.4.4/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.4.4/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.4.4/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.491623 dramkit-0.4.4/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21004 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3920949 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-02-10 04:51:36.000000 dramkit-0.4.4/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0    30350 2023-02-10 04:42:15.000000 dramkit-0.4.4/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.533928 dramkit-0.4.4/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.4.4/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     2875 2022-05-06 07:55:38.000000 dramkit-0.4.4/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.4.4/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19123 2022-06-25 18:20:13.000000 dramkit-0.4.4/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     3028 2022-05-04 14:19:57.000000 dramkit-0.4.4/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.4.4/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.4.4/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     7002 2022-05-05 07:54:48.000000 dramkit-0.4.4/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8252 2022-05-05 08:06:42.000000 dramkit-0.4.4/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.4.4/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    49631 2022-12-06 05:16:13.000000 dramkit-0.4.4/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7359 2022-05-05 23:24:31.000000 dramkit-0.4.4/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     6257 2022-12-01 08:24:37.000000 dramkit-0.4.4/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    19065 2022-12-12 03:02:35.000000 dramkit-0.4.4/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0    41417 2022-10-24 01:43:21.000000 dramkit-0.4.4/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    36152 2022-06-28 07:29:40.000000 dramkit-0.4.4/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.4.4/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.4.4/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.4.4/dramkit/datsci/utils_ml.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.549596 dramkit-0.4.4/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3463 2022-05-02 02:58:03.000000 dramkit-0.4.4/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.4.4/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12648 2022-05-01 09:12:47.000000 dramkit-0.4.4/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4544 2022-05-01 09:10:28.000000 dramkit-0.4.4/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9566 2022-05-01 09:11:33.000000 dramkit-0.4.4/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.4.4/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   104308 2023-02-09 15:40:14.000000 dramkit-0.4.4/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.4.4/dramkit/install_check.py
--rw-rw-rw-   0        0        0    55622 2023-02-09 09:14:07.000000 dramkit-0.4.4/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.559591 dramkit-0.4.4/dramkit/logtools/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.4.4/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.4.4/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.4.4/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.4.4/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4089 2023-02-08 04:12:28.000000 dramkit-0.4.4/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.588312 dramkit-0.4.4/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9745 2022-09-04 10:06:04.000000 dramkit-0.4.4/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.4.4/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7461 2022-09-04 10:06:57.000000 dramkit-0.4.4/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8896 2022-09-04 10:06:52.000000 dramkit-0.4.4/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13448 2022-09-04 10:06:48.000000 dramkit-0.4.4/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8734 2022-09-04 10:06:44.000000 dramkit-0.4.4/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9344 2022-09-04 10:06:39.000000 dramkit-0.4.4/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9962 2022-09-04 10:06:35.000000 dramkit-0.4.4/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8850 2022-09-04 10:06:29.000000 dramkit-0.4.4/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8922 2022-09-04 10:06:24.000000 dramkit-0.4.4/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.4.4/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7367 2022-09-04 10:06:12.000000 dramkit-0.4.4/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.604978 dramkit-0.4.4/dramkit/other/
--rw-rw-rw-   0        0        0      705 2023-02-10 09:36:50.000000 dramkit-0.4.4/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2573 2023-02-09 01:47:42.000000 dramkit-0.4.4/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0       70 2023-02-07 06:10:30.000000 dramkit-0.4.4/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.4.4/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.4.4/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.4.4/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1834 2022-12-07 07:37:09.000000 dramkit-0.4.4/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.4.4/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.618823 dramkit-0.4.4/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.4.4/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.4.4/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48517 2022-10-25 16:20:29.000000 dramkit-0.4.4/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.4.4/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     1681 2022-08-23 08:52:20.000000 dramkit-0.4.4/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     5120 2022-11-30 12:28:15.000000 dramkit-0.4.4/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.626713 dramkit-0.4.4/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.4.4/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.4.4/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.643331 dramkit-0.4.4/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.4.4/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.4.4/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.4.4/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.4.4/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.4.4/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.651260 dramkit-0.4.4/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     3597 2022-09-17 08:34:03.000000 dramkit-0.4.4/dramkit/speedup/multi_process.py
--rw-rw-rw-   0        0        0     5536 2022-05-20 16:05:33.000000 dramkit-0.4.4/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.668366 dramkit-0.4.4/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2051 2023-02-10 09:56:27.000000 dramkit-0.4.4/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    29245 2023-02-10 01:58:19.000000 dramkit-0.4.4/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6848 2023-02-07 04:30:25.000000 dramkit-0.4.4/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0       58 2022-09-29 03:34:58.000000 dramkit-0.4.4/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    19592 2023-02-07 07:05:17.000000 dramkit-0.4.4/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    23328 2023-02-10 05:07:12.000000 dramkit-0.4.4/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    49942 2023-02-07 07:24:12.000000 dramkit-0.4.4/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    17605 2023-02-07 07:05:31.000000 dramkit-0.4.4/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.675463 dramkit-0.4.4/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.4.4/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.4.4/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.681049 dramkit-0.4.4/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.4.4/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.4.4/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-02-15 01:28:22.348662 dramkit-0.4.4/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1098 2023-02-15 01:28:17.000000 dramkit-0.4.4/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4500 2023-02-15 01:28:21.000000 dramkit-0.4.4/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 01:28:17.000000 dramkit-0.4.4/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-15 01:28:18.000000 dramkit-0.4.4/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 01:28:22.684108 dramkit-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1516 2022-09-06 14:06:41.000000 dramkit-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.803705 dramkit-0.5.38/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.38/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-04-28 01:18:45.802705 dramkit-0.5.38/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.38/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.336723 dramkit-0.5.38/dramkit/
+-rw-rw-rw-   0        0        0      999 2023-04-24 03:43:26.000000 dramkit-0.5.38/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-04-28 01:17:38.000000 dramkit-0.5.38/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.483716 dramkit-0.5.38/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.38/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.38/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.38/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.38/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.38/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.38/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.38/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.38/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.38/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.38/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.38/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.38/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.38/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.38/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.38/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.38/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.38/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.38/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.38/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.38/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.38/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl.py
+-rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl2.py
+-rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl3.py
+-rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl4.py
+-rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl5.py
+-rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl6.py
+-rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_rl7.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.493715 dramkit-0.5.38/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.38/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.38/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.529715 dramkit-0.5.38/dramkit/chncal/
+-rw-rw-rw-   0        0        0      730 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21004 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3952591 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-04-27 13:34:54.000000 dramkit-0.5.38/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.38/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    33510 2023-04-19 02:53:20.000000 dramkit-0.5.38/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.582712 dramkit-0.5.38/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.38/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.38/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.38/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.38/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.38/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.38/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.38/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.38/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.38/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.38/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50059 2023-03-22 08:02:24.000000 dramkit-0.5.38/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.38/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.38/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    19374 2023-04-25 08:42:22.000000 dramkit-0.5.38/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.38/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.38/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.38/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.38/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.38/dramkit/datsci/utils_ml.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.604711 dramkit-0.5.38/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.38/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.38/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.38/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.38/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.38/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.38/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   112046 2023-04-27 02:54:14.000000 dramkit-0.5.38/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.38/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    67031 2023-04-12 07:15:28.000000 dramkit-0.5.38/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.620710 dramkit-0.5.38/dramkit/logtools/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.38/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.38/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.38/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.38/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.38/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.634710 dramkit-0.5.38/dramkit/openai/
+-rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.38/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.38/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    16820 2023-04-26 14:09:48.000000 dramkit-0.5.38/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.38/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.672708 dramkit-0.5.38/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.38/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.38/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.38/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.38/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.38/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.38/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.38/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.38/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.38/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.38/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.38/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.38/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.695708 dramkit-0.5.38/dramkit/other/
+-rw-rw-rw-   0        0        0     3791 2023-04-24 05:27:17.000000 dramkit-0.5.38/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     2871 2023-04-19 03:27:58.000000 dramkit-0.5.38/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.38/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.38/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.38/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.38/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.38/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.38/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.714709 dramkit-0.5.38/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.38/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.38/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.38/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.38/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.38/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.38/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.722706 dramkit-0.5.38/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.38/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.38/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.740706 dramkit-0.5.38/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.38/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.38/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.38/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.38/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.38/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.761706 dramkit-0.5.38/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.38/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.38/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.38/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.38/dramkit/speedup/iotools_tmp.py
+-rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.38/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.38/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.784705 dramkit-0.5.38/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.38/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.38/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.38/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0       58 2022-09-29 03:34:58.000000 dramkit-0.5.38/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    19770 2023-02-15 09:03:04.000000 dramkit-0.5.38/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.38/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50395 2023-02-24 11:32:46.000000 dramkit-0.5.38/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.38/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.792704 dramkit-0.5.38/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.38/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.38/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.799704 dramkit-0.5.38/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.38/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.38/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:18:45.350721 dramkit-0.5.38/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-04-28 01:18:41.000000 dramkit-0.5.38/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4852 2023-04-28 01:18:44.000000 dramkit-0.5.38/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 01:18:41.000000 dramkit-0.5.38/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-28 01:18:41.000000 dramkit-0.5.38/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 01:18:41.000000 dramkit-0.5.38/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 01:18:45.803705 dramkit-0.5.38/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2023-03-29 07:39:44.000000 dramkit-0.5.38/setup.py
```

### Comparing `dramkit-0.4.4/LICENSE` & `dramkit-0.5.38/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2022 YueYong Hu
+Copyright (c) 2020-2023 YueYong Hu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dramkit-0.4.4/PKG-INFO` & `dramkit-0.5.38/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.4.4
+Version: 0.5.38
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
@@ -34,9 +34,7 @@
 
 Pypi
 
 [dramkit](https://pypi.org/project/dramkit/)
 
 感谢使用和支持！
 
-
-
```

### Comparing `dramkit-0.4.4/README.md` & `dramkit-0.5.38/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/__init__.py` & `dramkit-0.5.38/dramkit/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,31 @@
 
 from ._pkg_info import pkg_info
 __version__ = pkg_info['__version__']
 from .install_check import install_check
 
 from .gentools import isnull
 from .gentools import log_used_time
-from .gentools import StructureObject
+from .gentools import GenObject
 from .gentools import TimeRecoder
+from .gentools import tmprint
 
 from .iotools import load_csv
 from .iotools import load_text, write_txt
 from .iotools import load_json, write_json
 from .iotools import pickle_file, unpickle_file
 
 from .plottools import plot_series
 from .plottools import plot_series_conlabel
 
 from .logtools.utils_logger import logger_show, close_log_file
 from .logtools.logger_general import get_logger as simple_logger
+
+from . import gentools
+from . import iotools
+from . import cryptotools
+from . import datetimetools as dttools
+from .datsci import find_maxmin
+from .openai import openai_chat
+from .other import othertools
+from .speedup import multi_thread, multi_process_concurrent
+from .sqltools import py_mysql
```

### Comparing `dramkit-0.4.4/dramkit/_pkg_info.py` & `dramkit-0.5.38/dramkit/_pkg_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.4.4',
+    '__version__': '0.5.38',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.4.4/dramkit/_tmp/CRR.py` & `dramkit-0.5.38/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.38/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.38/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.38/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.38/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/VMD.py` & `dramkit-0.5.38/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/cca_test.py` & `dramkit-0.5.38/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.38/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/explore.py` & `dramkit-0.5.38/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/gini.py` & `dramkit-0.5.38/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.38/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.38/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.38/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.38/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/plot_test.py` & `dramkit-0.5.38/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.38/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.38/dramkit/_tmp/simple_smooth.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.38/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_code.py` & `dramkit-0.5.38/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.38/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.38/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_grading.py` & `dramkit-0.5.38/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_lr.py` & `dramkit-0.5.38/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.38/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.38/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_tree.py` & `dramkit-0.5.38/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.38/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.38/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/tmp.py` & `dramkit-0.5.38/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.38/dramkit/_tmp/tmp_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,28 @@
 def h(a, **kwargs):
     b = {'b': 2, **kwargs}
     print(b)
 
 
 def i(*args):
     print(args)
+    
+    
+def fbase(**kwargs):
+    print(kwargs)
+    
+    
+def f1(x=1, y=2, **kwargs):
+    print(x, y)
+    fbase(**kwargs)
+    
+    
+def f2(z=3, **kwargs):
+    print(z)
+    f1(**kwargs)
 
 
 if __name__ == '__main__':
     params = {'b': 2, 'kargs': {'c': 4, 'd': 3}}
     result = e(params['b'], **params['kargs'])
     print('result: {}'.format(result))
 
@@ -58,7 +72,10 @@
     g(a=1, b=2, kwargs_f={'a0': 8, 'c': 3})
 
     print('\n')
     h(5, e=5)
 
     print('\n')
     i(5, 6)
+    
+    print('\n')
+    f2(z=3, y=5, a=6)
```

### Comparing `dramkit-0.4.4/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.38/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.38/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.38/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.38/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl2.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl3.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl4.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl4.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl5.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl5.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl6.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl6.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_rl7.py` & `dramkit-0.5.38/dramkit/_tmp/utils_rl7.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.38/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.38/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.38/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/__init__.py` & `dramkit-0.5.38/dramkit/chncal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # from __future__ import absolute_import, unicode_literals
 
-__version__ = '2.2.0'
+__version__ = '2.2.1'
 
 from .apis import (
     find_workday,
     get_dates,
     get_holiday_detail,
     get_holidays,
     get_solar_terms,
```

### Comparing `dramkit-0.4.4/dramkit/chncal/apis.py` & `dramkit-0.5.38/dramkit/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/constants.py` & `dramkit-0.5.38/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/constants_fate.py` & `dramkit-0.5.38/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/constants_hko.py` & `dramkit-0.5.38/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.38/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6003,14 +6003,90 @@
     ("CFFEX", datetime.date(year=2023, month=2, day=4)): 0,
     ("CFFEX", datetime.date(year=2023, month=2, day=5)): 0,
     ("CFFEX", datetime.date(year=2023, month=2, day=6)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=7)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=8)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=9)): 1,
     ("CFFEX", datetime.date(year=2023, month=2, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=11)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=12)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=15)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=16)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=18)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=19)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=22)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=23)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=24)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=25)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=26)): 0,
+    ("CFFEX", datetime.date(year=2023, month=2, day=27)): 1,
+    ("CFFEX", datetime.date(year=2023, month=2, day=28)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=1)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=2)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=3)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=4)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=5)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=8)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=9)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=11)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=12)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=15)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=16)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=18)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=19)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=22)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=23)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=24)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=25)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=26)): 0,
+    ("CFFEX", datetime.date(year=2023, month=3, day=27)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=28)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=29)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=30)): 1,
+    ("CFFEX", datetime.date(year=2023, month=3, day=31)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=1)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=2)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=3)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=4)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=5)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=8)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=9)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=10)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=11)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=12)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=15)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=16)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=18)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=19)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=22)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=23)): 0,
+    ("CFFEX", datetime.date(year=2023, month=4, day=24)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=25)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=26)): 1,
+    ("CFFEX", datetime.date(year=2023, month=4, day=27)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -17812,14 +17888,90 @@
     ("CZCE", datetime.date(year=2023, month=2, day=4)): 0,
     ("CZCE", datetime.date(year=2023, month=2, day=5)): 0,
     ("CZCE", datetime.date(year=2023, month=2, day=6)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=7)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=8)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=9)): 1,
     ("CZCE", datetime.date(year=2023, month=2, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=11)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=12)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=15)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("CZCE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("CZCE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("CZCE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("CZCE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("CZCE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("CZCE", datetime.date(year=2023, month=4, day=27)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -28750,14 +28902,90 @@
     ("DCE", datetime.date(year=2023, month=2, day=4)): 0,
     ("DCE", datetime.date(year=2023, month=2, day=5)): 0,
     ("DCE", datetime.date(year=2023, month=2, day=6)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=7)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=8)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=9)): 1,
     ("DCE", datetime.date(year=2023, month=2, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=11)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=12)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=15)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("DCE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("DCE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("DCE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("DCE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("DCE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("DCE", datetime.date(year=2023, month=4, day=27)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -30839,14 +31067,90 @@
     ("INE", datetime.date(year=2023, month=2, day=4)): 0,
     ("INE", datetime.date(year=2023, month=2, day=5)): 0,
     ("INE", datetime.date(year=2023, month=2, day=6)): 1,
     ("INE", datetime.date(year=2023, month=2, day=7)): 1,
     ("INE", datetime.date(year=2023, month=2, day=8)): 1,
     ("INE", datetime.date(year=2023, month=2, day=9)): 1,
     ("INE", datetime.date(year=2023, month=2, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=11)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=12)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=15)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("INE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("INE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("INE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("INE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("INE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("INE", datetime.date(year=2023, month=4, day=27)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42420,14 +42724,90 @@
     ("SHFE", datetime.date(year=2023, month=2, day=4)): 0,
     ("SHFE", datetime.date(year=2023, month=2, day=5)): 0,
     ("SHFE", datetime.date(year=2023, month=2, day=6)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=7)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=8)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=9)): 1,
     ("SHFE", datetime.date(year=2023, month=2, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=11)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=12)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=15)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("SHFE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("SHFE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("SHFE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SHFE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("SHFE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("SHFE", datetime.date(year=2023, month=4, day=27)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54162,14 +54542,90 @@
     ("SSE", datetime.date(year=2023, month=2, day=4)): 0,
     ("SSE", datetime.date(year=2023, month=2, day=5)): 0,
     ("SSE", datetime.date(year=2023, month=2, day=6)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=7)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=8)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=9)): 1,
     ("SSE", datetime.date(year=2023, month=2, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=11)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=12)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=15)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("SSE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("SSE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("SSE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SSE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("SSE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("SSE", datetime.date(year=2023, month=4, day=27)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -65708,8 +66164,84 @@
     ("SZSE", datetime.date(year=2023, month=2, day=4)): 0,
     ("SZSE", datetime.date(year=2023, month=2, day=5)): 0,
     ("SZSE", datetime.date(year=2023, month=2, day=6)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=7)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=8)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=9)): 1,
     ("SZSE", datetime.date(year=2023, month=2, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=11)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=12)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=15)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=16)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=18)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=19)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=22)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=23)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=24)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=25)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=26)): 0,
+    ("SZSE", datetime.date(year=2023, month=2, day=27)): 1,
+    ("SZSE", datetime.date(year=2023, month=2, day=28)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=1)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=2)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=3)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=4)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=5)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=8)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=9)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=11)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=12)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=15)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=16)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=18)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=19)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=22)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=23)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=24)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=25)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=26)): 0,
+    ("SZSE", datetime.date(year=2023, month=3, day=27)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=28)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=29)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=30)): 1,
+    ("SZSE", datetime.date(year=2023, month=3, day=31)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=1)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=2)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=3)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=4)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=5)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=8)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=9)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=10)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=11)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=12)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=15)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=16)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=18)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=19)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=22)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=23)): 0,
+    ("SZSE", datetime.date(year=2023, month=4, day=24)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=25)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=26)): 1,
+    ("SZSE", datetime.date(year=2023, month=4, day=27)): 1,
 }
```

### Comparing `dramkit-0.4.4/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.38/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.38/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/chncal/solar_terms.py` & `dramkit-0.5.38/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datetimetools.py` & `dramkit-0.5.38/dramkit/datetimetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,23 @@
                 return res
             raise
         except:
             if dt_type == 'struct_time':
                 return time.strftime('%Y-%m-%d %H:%M:%S.%f', dt)
             else:
                 return str(dt)
+            
+            
+def dtseries2str(series, joiner='-', strformat=None):
+    '''pd.Series转化为str，若不指定strformat，则按joiner连接年月日'''
+    res = pd.to_datetime(series)
+    if pd.isnull(strformat):
+        strformat = '%Y{x}%m{x}%d'.format(x=joiner)
+    res = res.apply(lambda x: x.strftime(strformat))
+    return res
 
 
 def get_datetime_strformat(tstr,
                            ymd = ['-', '', '.', '/'],
                            ymd_hms = [' ', '', '.'],
                            hms = [':', ''],
                            hms_ms = ['.', '']
@@ -417,14 +426,16 @@
             return pd.to_datetime(x)
 
 
 def copy_format(to_tm, from_tm):
     '''
     复制日期时间格式
     '''
+    if pd.isna(from_tm):
+        return to_tm
     input_type = type(to_tm).__name__
     types1 = ['datetime', 'date', 'Timestamp', 'struct_time']
     types2 = ['str', 'int', 'float']
     types3 = ['ndarray', 'Series', 'list', 'tuple']
     assert input_type in types1+types2+types3
     if input_type == type(from_tm).__name__ and input_type in types1:
         return to_tm
@@ -544,24 +555,108 @@
 
 def get_quarter(dt=None, joiner='Q'):
     '''获取日期所在季度'''
     if pd.isnull(dt):
         dt = datetime.datetime.now()
     t = x2datetime(dt)
     y, q = t.year, t.quarter
+    if not joiner:
+        return (y, q)
     return joiner.join([str(y), str(q)])
 
 
+def get_quarter_start_end_by_yq(y, q, joiner='-'):
+    m1 = {1: '01', 2: '04', 3: '07', 4: '10'}[q]
+    d1 = '01'
+    m2 = {1: '03', 2: '06', 3: '09', 4: '12'}[q]
+    d2 = {3: '31', 6: '30', 9: '30', 12: '31'}[int(m2)]
+    start = joiner.join([str(y), m1, d1])
+    end = joiner.join([str(y), m2, d2])
+    return start, end
+
+
+def get_quarter_start_end_by_date(date=None):
+    '''获取date日期所在季度的起始日期'''
+    y, q = get_quarter(date, None)
+    return copy_format(get_quarter_start_end_by_yq(y, q),
+                       date)
+
+
 def today_quarter(joiner='Q'):
     '''获取今日所在季度'''
     t = pd.to_datetime(datetime.datetime.now())
     y, q = t.year, t.quarter
+    if not joiner:
+        return (y, q)
     return joiner.join([str(y), str(q)])
 
 
+def get_2part_next(part1, part2, step, n=1):
+    '''
+    Example
+    -------
+    >>> get_2part_next(2023, 2, 4, 2) # 2023Q2往后推2个季度
+    (2023, 4)
+    >>> get_2part_next(2023, 4, 4, 5) # 2023Q4往后推5个季度
+    (2025, 1)
+    >>> get_2part_next(2023, 4, 12, 8) # 202304往后推8个月
+    (2023, 12)
+    >>> get_2part_next(2023, 9, 12, 10) # 202309往后推10个月
+    (2024, 7)
+    >>> get_2part_next(2023, 2, 4, -2) # 2023Q2往前推2个季度
+    (2022, 4)
+    >>> get_2part_next(2023, 4, 4, -5) # 2023Q4往前推5个季度
+    (2022, 3)
+    >>> get_2part_next(2023, 4, 12, -8) # 202304往前推8个月
+    (2022, 4)
+    >>> get_2part_next(2023, 9, 12, -10) # 202309往前推10个月
+    (2022, 11)
+    '''
+    assert all([isinstance(x, int) for x in [part1, part2, step, n]])
+    if n == 0:
+        p1new, p2new = part1, part2
+    elif n > 0:
+        p1add = n // step + int((part2 + n % step) > step)
+        p1new = part1 + p1add
+        p2new = part2 + (n % step)
+        if p2new > step:
+            p2new = p2new - step
+    else:
+        n = abs(n)
+        p1add = -(n // step) - int((part2 - n % step) <= 0)
+        p1new = part1 + p1add
+        p2new = part2 - (n % step)
+        if p2new <= 0:
+            p2new = step + p2new
+    return (p1new, p2new)
+
+
+def get_pre_quarter(date=None, n=1, joiner='Q'):
+    '''
+    | 获取date前第n个季度
+    | 如:
+    | get_pre_quarter("20230418") -> "2023Q1"
+    | get_pre_quarter("20230418", 2) -> "2022Q4"
+    | get_pre_quarter("20230418", 3) -> "2022Q3"
+    | get_pre_quarter("20230418", 4) -> "2022Q2"
+    | get_pre_quarter("20230418", 5) -> "2022Q1"
+    | get_pre_quarter("20230418", 6) -> "2021Q4"
+    | get_pre_quarter("20230418", 7) -> "2021Q3"
+    | get_pre_quarter("20230418", 8) -> "2021Q2"
+    '''
+    if pd.isnull(date):
+        date = datetime.datetime.now()
+    t = x2datetime(date)
+    y, q = t.year, t.quarter
+    ynew, qnew = get_2part_next(y, q, 4, -n)
+    if not joiner:
+        return (ynew, qnew)
+    return joiner.join([str(ynew), str(qnew)])
+
+
 def get_dayofweek(date=None):
     '''返回date属于星期几（1-7）'''
     if pd.isnull(date):
         date = datetime.date.today()
     return x2datetime(date).weekday() + 1
```

### Comparing `dramkit-0.4.4/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.38/dramkit/datsci/_utils_ann.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,19 +69,20 @@
 
     return mdl
 
 
 if __name__ == '__main__':
     import time
     import pandas as pd
+    from dramkit.gentools import TimeRecoder
     from dramkit.datsci.preprocess import scale_skl
     from sklearn.datasets import load_iris, load_diabetes
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     # 回归数据集
     data_reg = load_diabetes()
     Xreg, yreg = data_reg['data'], data_reg['target']
     data_reg = pd.DataFrame(Xreg,
                           columns=['x_'+str(_) for _ in range(Xreg.shape[1])])
     data_reg['y'] = yreg
@@ -111,8 +112,8 @@
                         columns=['x_'+str(_) for _ in range(Xcls.shape[1])])
     Xcls = scale_skl(Xcls)[0]
 
     # 逻辑回归模型比较
     mdl_lrc_skl = lrc_skl(Xcls, ycls)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.38/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datsci/ahp.py` & `dramkit-0.5.38/dramkit/datsci/ahp.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,18 +271,18 @@
                                          check_JM_tol=check_JM_tol, logger=logger)
 
     return w, isOK, (CR, CI, lmdmax, RI), (JM, P, CIs, CRs)
 
 #%%
 if __name__ == '__main__':
     import time
-    from dramkit import simple_logger
+    from dramkit import simple_logger, TimeRecoder
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     # 来自论文：土地整治的扶贫成效分析及评价——以北川羌族自治县开坪乡土地开发整理项目为例
     # judge_mat = np.array([[1, 3/2, 3/2],
     #                       [2/3, 1, 3/2],
     #                       [2/3, 2/3, 1]])
     judge_mat = np.array([[1, 4, 3, 2, 5],
@@ -460,8 +460,8 @@
                     skip_bad_JM=skip_bad_JM, check_JM_tol=check_JM_tol,
                     logger=logger)
     print('\n')
     print('isOK: {}'.format(isOK))
     print('w: \n{}'.format(w))
 
     #%%
-    print('\nused time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.38/dramkit/datsci/ahp_sim_ri.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,14 @@
         # max_important_level = 9 if k <= 9 else max_num_indicator
         max_important_level = 9
         RI_dict[k] = sim_ri(k, max_important_level, num_sim)
     return RI_dict
 
 
 if __name__ == '__main__':
-    import time
+    from dramkit import TimeRecoder
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     RI_dict = get_RIs()
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/apriori.py` & `dramkit-0.5.38/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datsci/curvature.py` & `dramkit-0.5.38/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datsci/elm_cls.py` & `dramkit-0.5.38/dramkit/datsci/elm_cls.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,23 +164,23 @@
 
     def predict_proba(self, X):
         '''概率预测'''
         raise NotImplementedError
 
 #%%
 if __name__ == '__main__':
-    import time
     import pandas as pd
     from sklearn import metrics
     import sklearn.datasets as datasets
     from sklearn.model_selection import train_test_split as tts
+    from dramkit import TimeRecoder
     from dramkit.datsci.preprocess import scale_skl
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     data = datasets.load_iris()
     X = pd.DataFrame(data['data'], columns=data.feature_names)
     Y = pd.Series(data['target'])
     # Y = np.array(pd.get_dummies(Y), dtype=np.int8)
 
@@ -202,8 +202,8 @@
 
         Ypre = mdlEML.predict(Xtest)
 
         acc = metrics.accuracy_score(Ytest, Ypre)
         print('n_hide - %d, acc：%f' % (n_hide, acc))
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/elm_reg.py` & `dramkit-0.5.38/dramkit/datsci/elm_reg.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,28 +154,28 @@
         if self.Yreshape:
             y_pred = y_pred.reshape(-1)
 
         return y_pred
 
 #%%
 if __name__ == '__main__':
-    import time
     import pandas as pd
     import sklearn.datasets as datasets
     from sklearn.model_selection import train_test_split as tts
+    from dramkit import TimeRecoder
     from dramkit.datsci.stats import mape
 
     import matplotlib as mpl
     mpl.rcParams['font.sans-serif'] = ['SimHei']
     mpl.rcParams['font.serif'] = ['SimHei']
     mpl.rcParams['axes.unicode_minus'] = False
     import matplotlib.pyplot as plt
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     # 产生数据集
     X = np.linspace(0, 20, 200)
     noise = np.random.normal(0, 0.08, 200)
     y = np.sin(X) + np.cos(0.5*X) + noise
     # 转化成二维形式
@@ -242,8 +242,8 @@
         # plt.figure(figsize=(12, 7))
         # plt.plot(Ytest.reset_index(drop=True), '.-b', label='Ytrue')
         # plt.plot(Ypre, '.-r', label='Ypre')
         # plt.legend(loc=0)
         # plt.show()
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.38/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.38/dramkit/datsci/find_maxmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,16 @@
     series.name = 'series'
     if series.index.name is None:
         series.index.name = 'idx'
 
     df = pd.DataFrame(series)
     col = df.columns[0]
     df.reset_index(inplace=True)
+    
+    # plot_series(df, {'series': '.-k'}, title='原始数据', grids=True)
 
     # 所有转折点
     df['dif'] = df[col].diff()
     df['dif_big'] = (df['dif'] > 0).astype(int)
     df['dif_sml'] = -1 * (df['dif'] < 0).astype(int)
     ktmp = 1
     while ktmp < df.shape[0] and df.loc[df.index[ktmp], 'dif'] == 0:
@@ -96,15 +98,15 @@
     elif df.loc[df.index[ktmp], 'dif'] < 0:
         df.loc[df.index[0], 'dif_big'] = 1
     df['label'] = df['dif_big'] + df['dif_sml']
     label_ = replace_repeat_pd(df['label'][::-1], 1, 0)
     label_ = replace_repeat_pd(label_, -1, 0)
     df['label'] = label_[::-1]
 
-    # plot_maxmins(df, col, 'label', title='Ori')
+    # plot_maxmins(df, col, 'label', title='所有拐点')
 
     # t_min应大于等于1
     if t_min is not None and t_min < 1:
         t_min = None
 
     if t_min:
         def _max_dif_ok(v2, v3):
@@ -232,26 +234,26 @@
                     k4 = k3 +1
                     while k4 < df.shape[0] and df.loc[k4, 'label'] == 0:
                         k4 += 1
 
                     to_del, idxs = _to_del(df, k1, k2, k3, k4)
                     if to_del:
                         df.loc[idxs, 'label'] = 0
+                        # plot_maxmins(df, col, 'label', title='筛除不满足条件的极值对', grid=False)
 
                     k2 = k3
 
             return df
 
         df = _del_t_min(df)
-        # plot_maxmins(df, col, 'label', title='1st del1')
+        # plot_maxmins(df, col, 'label', title='第1次正向筛除')
 
         df.index = range(df.shape[0]-1, -1, -1)
         df = _del_t_min(df)
-        # plot_maxmins(df, col, 'label', title='1st del2')
-
+        
         def _check_t_min(df, t_min):
             Fcond = lambda x: True if x == 0 else False
             df['tmp'] = con_count(df['label'], Fcond).shift(1)
             df['tmp'] = abs(df['tmp'] * df['label'])
             df.loc[df.index[0], 'tmp'] = 0
             tmp = list(df[df['label'] != 0]['tmp'])
             df.drop('tmp', axis=1, inplace=True)
@@ -261,24 +263,27 @@
                 tmp = tmp[1:]
                 if all([x >= t_min for x in tmp]):
                     return True, tmp
                 else:
                     return False, tmp
         t_min_ok, tmp = _check_t_min(df, t_min)
         tmp_new = []
-        # plot_maxmins(df, col, 'label', title='t_min check: '+str(t_min_ok))
+        # plot_maxmins(df, col, 'label', title='第1次反向筛除，t_min check: '+str(t_min_ok))
         # 注：特殊情况下不可能满足任何两个极大极小值对之间的间隔都大于t_min
+        k = 2
         while not t_min_ok and not tmp == tmp_new:
             t_min_ok, tmp = _check_t_min(df, t_min)
             df.index = range(df.shape[0])
             df = _del_t_min(df)
+            # plot_maxmins(df, col, 'label', title='第%s次正向筛除'%k)
             df.index = range(df.shape[0]-1, -1, -1)
             df = _del_t_min(df)
             t_min_ok, tmp_new = _check_t_min(df, t_min)
-            # plot_maxmins(df, col, 'label', title='t_min check: '+str(t_min_ok))
+            # plot_maxmins(df, col, 'label', title='第%s次反向筛除，t_min check: %s'%(k, t_min_ok))
+            k += 1
 
     df.set_index(series.index.name, inplace=True)
 
     return df['label']
 
 #%%
 def check_maxmins(df, col, col_label, max_lbl=1, min_lbl=-1):
@@ -974,17 +979,21 @@
                             )
                 time.sleep(plot_sleep)
 
     return data['signal'], data['sig_type']
 
 #%%
 if __name__ == '__main__':
-    strt_tm = time.time()
+    from dramkit import TimeRecoder    
+    from finfactory.load_his_data import load_index_joinquant
 
+    tr = TimeRecoder()    
+    
     #%%
+    # '''
     arr = [1, 1, 1.3, 1.2, 2, 3, 4.8, 4.7, 5, 5]
     df1 = pd.DataFrame({'col': arr})
     df1['label'] = find_maxmin(df1['col'])
     plot_maxmins(df1, 'col', 'label',
                  title='标注极大极小值test1')
     OK, e = check_maxmins(df1, df1.columns[0], df1.columns[1])
     if OK:
@@ -997,16 +1006,18 @@
     plot_maxmins(df2, 'col', 'label',
                  title='标注极大极小值test2')
     OK, e = check_maxmins(df2, df2.columns[0], df2.columns[1])
     if OK:
         print('极值点排列正确！')
     else:
         print('极值点排列错误:', e)
+    # '''
 
     #%%
+    # '''
     # 二次曲线叠加正弦余弦-------------------------------------------------------
     N = 200
     t = np.linspace(0, 1, N)
     s = 6*t*t + np.cos(10*2*np.pi*t*t) + np.sin(6*2*np.pi*t)
     df = pd.DataFrame(s, columns=['test'])
 
     # t_min = None
@@ -1017,16 +1028,18 @@
                  title='标注极大极小值test：t_min='+str(t_min))
 
     OK, e = check_maxmins(df, df.columns[0], df.columns[1])
     if OK:
         print('极值点排列正确！')
     else:
         print('极值点排列错误:', e)
+    # '''
         
     #%%
+    # '''
     # 趋势线叠加正弦余弦---------------------------------------------------------
     N = 200
     t = np.linspace(0, 1, N)
     trend = 6 * t
     circle1 = np.cos(10*2*np.pi*t*t)
     circle2 = np.sin(6*2*np.pi*t)
     # circle2 = 0 * t
@@ -1060,16 +1073,18 @@
                  'trend': ('-r', None),
                  'circle1': ('-b', None),
                  'circle2': ('-g', None),
                  'noise': ('-y', None)},
                 # cols_to_label_info={'series':
                 #     [['label', (1, -1), ('gv', 'r^'), False]]},
                 title='周期波动示例')
+    # '''
 
     #%%
+    # '''
     # 50ETF日线行情------------------------------------------------------------
     fpath = '../_test/510500.SH_daily_qfq.csv'
     his_data = load_csv(fpath)
     his_data.set_index('date', drop=False, inplace=True)
 
     # N = his_data.shape[0]
     N = 5000
@@ -1083,19 +1098,20 @@
     plot_maxmins(df.iloc[:, :], col, 'label', figsize=(12, 7))
 
     OK, e = check_maxmins(df, col, 'label')
     if OK:
         print('极值点排列正确！')
     else:
         print('极值点排列错误:', e)
+    # '''
 
     #%%
+    # '''
     # 上证50分钟行情------------------------------------------------------------
-    fpath = '../../../FinFactory/data/archives/index/joinquant/000016.XSHG_1min.csv'
-    his_data = load_csv(fpath)
+    his_data = load_index_joinquant('000016', '1min')
     his_data['time'] = his_data['time'].apply(lambda x:
                     x.replace('-', '').replace(':', '').replace(' ', '')[:-2])
     his_data.set_index('time', drop=False, inplace=True)
     his_data['ma'] = his_data['close'].rolling(20).mean()
 
     df = his_data.iloc[-240*18:-240*17, :].copy()
     N = df.shape[0]
@@ -1117,14 +1133,15 @@
     if OK:
         print('极值点排列正确！')
     else:
         print('极值点排列错误:', e)
 
     his_cycle_info, df_his = get_his_maxmin_info(df, col, 'label')
     last_pos_info = get_last_pos_info(df.iloc[:-1, :], col, 'label', min_gap=0)
+    # '''
 
     #%%
     # 动态标签
     # df['signal'], df['sig_type'] = find_maxmin_dy(df, col, t_min,
     #                                 his_lag=50,
     #                                 use_all=False,
     #                                 logger=None,
@@ -1141,8 +1158,8 @@
     #                                           False]]},
     #                                     'title': '50ETF',
     #                                     'n_xticks': 4,
     #                                     'figsize': (10, 5)},
     #                                 plot_sleep=0.5)
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.38/dramkit/datsci/freq_item_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,30 +158,30 @@
 
     # 使用mlxtend的算法
     RulesApri_mlx = arpiori_mlx(dataset, min_sup, min_conf)
     RulesFpGrow_mlx = fpgrowth_mlx(dataset, min_sup, min_conf)
 
 
     # test2 ------------------------------------------------------------------
-    # import time
+    # from dramkit import TimeRecoder
     # from dramkit import load_text
 
     # fpath = '../../../DataScience/dataSets/Frequent_Itemset_Mining_Dataset/T10I4D100K.dat'
     # dataset = load_text(fpath, sep=' ', keep_header=False, to_pd=False)
 
     # min_sup = 0.01
     # min_conf = 0.01
 
     # # Apriori
-    # strt_tm = time.time()
+    # tr = TimeRecoder()
     # RulesApriHoo = apriori_dramkit(dataset, min_sup, min_conf)
     # RulesApriHoodf = rules2df(RulesApriHoo)
-    # print('used {}s.'.format(round(time.time()-strt_tm, 6)))
+    # tr.used()
 
     # # 使用mlxtend的算法
-    # strt_tm = time.time()
+    # tr = TimeRecoder()
     # RulesApri_mlx = arpiori_mlx(dataset, min_sup, min_conf)
-    # print('used {}s.'.format(round(time.time()-strt_tm, 6)))
+    # tr.used()
 
-    # strt_tm = time.time()
+    # tr = TimeRecoder()
     # RulesFpGrow_mlx = fpgrowth_mlx(dataset, min_sup, min_conf)
-    # print('used {}s.'.format(round(time.time()-strt_tm, 6)))
+    # tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/lr.py` & `dramkit-0.5.38/dramkit/datsci/lr.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,25 +154,25 @@
         '''标签预测'''
         y_pre_p = self.predict_proba(X)
         y_pre = (y_pre_p >= p_cut).astype(int)
         return y_pre
 
 #%%
 if __name__ == '__main__':
-    import time
     import pandas as pd
+    from dramkit import TimeRecoder
 
     import matplotlib as mpl
     mpl.rcParams['font.sans-serif'] = ['SimHei']
     mpl.rcParams['font.serif'] = ['SimHei']
     mpl.rcParams['axes.unicode_minus'] = False
     import matplotlib.pyplot as plt
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     data = pd.read_excel('./_test/test_data1.xlsx')
     # data = pd.read_excel('./_test/test_data2.xlsx')
     X = data[['x1', 'x2']]
     y = data['y']
 
@@ -205,8 +205,8 @@
             plt.title(title)
 
         plt.show()
 
     plot_result(data, mdl.w, mdl.b, opt_method)
 
     #%%
-    print('\nused time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/preprocess.py` & `dramkit-0.5.38/dramkit/datsci/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,32 @@
 
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 
 from dramkit.gentools import con_count, isnull
 
 
-def mad(ser, param=3):
-    arr = ser.values
-    median = np.nanmedian(arr, axis=0)
-    abs_arr = np.abs(arr - median)
-    med = np.nanmedian(abs_arr) * 1.483
-    ceil = median + param * med
-    floor = median - param * med
-    arr[arr > ceil] = ceil
-    arr[arr < floor] = floor
-    return arr
+def mad(series, n=3, up_cut_val=None, low_cut_val=None):
+    '''MAD计算值处理方法'''
+    values = np.array(series)
+    median = np.nanmedian(values, axis=0)
+    abs_med_dif = np.abs(values - median)
+    med = np.nanmedian(abs_med_dif) * 1.483
+    upper = median + n * med
+    lower = median - n * med
+    if isnull(up_cut_val):
+        up_cut_val = upper
+    if isnull(low_cut_val):
+        low_cut_val = lower
+    values[values > upper] = up_cut_val
+    values[values < lower] = low_cut_val
+    try:
+        return pd.Series(values, index=series.index)
+    except:
+        return values
 
 
 class ExternalStd(object):
     '''极端值处理，标准差倍数法'''
 
     def __init__(self, nstd=3, cols=None):
         raise NotImplementedError
```

### Comparing `dramkit-0.4.4/dramkit/datsci/stats.py` & `dramkit-0.5.38/dramkit/datsci/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
     
     Note
     ----
     series会被当成没有无效值处理
 
     See Also
     --------
-    :func:`dramkit.datsci.utils_stats.delta_var`
+    :func:`dramkit.datsci.stats.delta_var`
     '''
 
     # 数据格式检查
     series = np.array(series)
     assert len(series.shape) == 1, 'series必须为1维！'
     # assert sum(np.isnan(series)) == 0, 'series中不能有无效值！'
 
@@ -750,15 +750,15 @@
         是否忽略无效值
 
 
     :returns: `pd.Series` - 滚动累计方差计算结果
 
     See Also
     --------
-    :func:`dramkit.datsci.utils_stats.cumvar_nonan`
+    :func:`dramkit.datsci.stats.cumvar_nonan`
     '''
     df = pd.DataFrame({'v': series})
     if not skipna:
         df['cumvar'] = cumvar_nonan(df['v'], ddof=ddof)
         return df['cumvar']
     else:
         df_ = df.dropna(subset=['v'], how='any').copy()
@@ -1013,15 +1013,15 @@
     cumranks = [1] * n
 
     nums_sorted = [series[0]]
     ranks = [1]
     for k in range(1, n):
         num = series[k]
         irank, (nums_sorted, ranks) = rank_of_insert_bin(nums_sorted, ranks,
-                                    num, ascending=ascending, method=method)
+                                      num, ascending=ascending, method=method)
         cumranks[k] = irank
 
     return cumranks
 
 
 def cumrank(series, ascending=True, method='dense'):
     '''
@@ -1182,15 +1182,15 @@
 
     return df['Nunique']
 
 
 def cum_pct_loc(series, method='dense'):
     '''
     | 滚动计算series(`np.array, pd.Series`)数据累计所处百分位
-    | 调用 :func:`dramkit.datsci.utils_stats.cum_n_unique_pd` 函数
+    | 调用 :func:`dramkit.datsci.stats.cum_n_unique_pd` 函数
     '''
     if not method in ['dense', 'average']:
         raise ValueError('未识别的并列排序方法！')
     df = pd.DataFrame({'v': series})
     df['cumrank'] = cumrank(df['v'], method=method)
     if method == 'dense':
         df['cumNunique'] = cum_n_unique_pd(df['v'])
@@ -1200,15 +1200,15 @@
         df['PctLoc'] = df['cumrank'] / df['idx']
     return df['PctLoc']
 
 
 def _cum_pct_loc1(series, method='dense'):
     '''
     | 滚动计算series(`np.array, pd.Series`)数据累计所处百分位
-    | 调用 :func:`dramkit.datsci.utils_stats.cum_n_unique` 函数
+    | 调用 :func:`dramkit.datsci.stats.cum_n_unique` 函数
     '''
     if not method in ['dense', 'average']:
         raise ValueError('未识别的并列排序方法！')
     df = pd.DataFrame({'v': series})
     df['cumrank'] = cumrank(df['v'], method=method)
     if method == 'dense':
         df['cumNunique'] = cum_n_unique(df['v'])
@@ -1218,15 +1218,15 @@
         df['PctLoc'] = df['cumrank'] / df['idx']
     return df['PctLoc']
 
 
 def _cum_pct_loc2(series, method='dense'):
     '''
     | 滚动计算series(`np.array, pd.Series`)数据累计所处百分位
-    | 调用 :func:`dramkit.datsci.utils_stats.get_pct_loc` 函数
+    | 调用 :func:`dramkit.datsci.stats.get_pct_loc` 函数
     '''
     df = pd.DataFrame({'v': series})
     df['PctLoc'] = np.nan
     ori_idx = df.index
     df.reset_index(drop=True, inplace=True)
     df.loc[df.index[0], 'PctLoc'] = 1.0
     if isnull(df.loc[df.index[0], 'v']):
```

### Comparing `dramkit-0.4.4/dramkit/datsci/time_series.py` & `dramkit-0.5.38/dramkit/datsci/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -667,27 +667,26 @@
                    ycol, Xcols_series_lag, Xcols_other, y_step, gap, **kwargs)
         test_pre = test_pre.iloc[y_lag+gap:y_lag+gap+n_test, :]
 
     return valid_pre, test_pre
 
 #%%
 if __name__ == '__main__':
-    import time
     from dramkit import plot_series
     from sklearn.linear_model import LinearRegression as lr
     from sklearn.svm import SVR as svr
-    from dramkit.gentools import cut_range_to_subs, replace_repeat_pd
+    from dramkit.gentools import cut_range_to_subs, replace_repeat_pd, TimeRecoder
     from dramkit._tmp.utils_SignalDec import dec_emds, merge_high_modes
     from dramkit._tmp.utils_SignalDec import plot_modes
     from finfactory.fintools import get_yield_curve
     from finfactory.load_his_data import load_future_daily_tushare
     from pprint import pprint
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     code = 'IF.CFX'
     data = load_future_daily_tushare(code)
 
     data.set_index('date', drop=False, inplace=True)
 
@@ -892,8 +891,8 @@
                                             force_final0='settle',
                                             kwargs_plot={'title': code,
                                                          'n_xticks': 6})
 
     pprint(trade_gain_info3)
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/datsci/topsis.py` & `dramkit-0.5.38/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.38/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/datsci/utils_ml.py` & `dramkit-0.5.38/dramkit/datsci/utils_ml.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.38/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
 
-import time
-
 
 def find_addends_backpack01float(tgt_sum, alts):
     '''
     | 从给定的列表alts（正数）中选取若干个数，其和小于等于tgt_sum并且最接近sum_tgt
     | 思路：求和问题转化为物品价值和重量相等的01（正）浮点数背包问题
 
     Parameters
@@ -90,16 +88,16 @@
     max_v = values[-1]
     addends = [alts[x] for x in trace]
 
     return max_v, addends, trace, values
 
 
 if __name__ == '__main__':
-    strt_tm = time.time()
-
+    from dramkit import TimeRecoder
+    tr = TimeRecoder()
 
     tgt_sum = 22 + 21 + 5.1
     alts = [22, 15, 14, 13, 7, 6.1, 5, 21.5, 100]
 
     # alts = [17541875.0, 16901617.0, 10696518.0, 6388100.0, 2305050.0,
     #         783360.0, 632604.0, 628650.0, 609600.0, 601650.0, 600668.0] + \
     #       [590550.0, 599557.0, 628000.0, 628650.0, 628650.0, 628650.0,
@@ -111,8 +109,8 @@
     max_v, addends, trace, values = find_addends_backpack01float(tgt_sum, alts)
     print('目标和:', tgt_sum)
     print('备选加数和:', max_v)
     print('备选加数编号:', trace)
     print('备选加数:', addends)
 
 
-    print('used {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.38/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.38/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     adds_process : list
         搜索中间过程
     '''
 
     adds_process = [] if save_process else None
 
     if log_info:
-        start_time = time.time()
+        start_time = time.monotonic()
 
     all_postive = all([x >= 0 for x in alts])
 
     if len(alts) == 0:
         return [], [], adds_process
 
     # 当目标和小于alts的最小值且alts没有负数时可直接返回最接近值
@@ -164,15 +164,15 @@
         chosed_addends.append(alts[idx_last])
         if save_process:
             adds_process.append(chosed_addends.copy())
         now_sum += alts[idx_last]
 
     if log_info:
         logger_show('loop_count: {}'.format(loop_count), logger, 'info')
-        logger_show('used time {}s.'.format(round(time.time()-start_time, 6)),
+        logger_show('used time {}s.'.format(round(time.monotonic()-start_time, 6)),
                     logger, 'info')
 
     return choseds_best, chosed_addends, adds_process
 
 
 if __name__ == '__main__':
     alts = [17541875.0, 16901617.0, 10696518.0, 6388100.0, 2305050.0, 987414.0,
```

### Comparing `dramkit-0.4.4/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.38/dramkit/find_addends/find_addends_recu.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,17 +79,16 @@
                                tol_above=tol_above, n_result=n_result,
                                keep_order=keep_order)
 
     return results
 
 
 if __name__ == '__main__':
-    import time
-    start_time = time.time()
-
+    from dramkit import TimeRecoder
+    tr = TimeRecoder()
 
     tgt_sum = 22 + 21 + 4.1
     alts = [22, 15, 14, 13, 7, 6.1, 5, 21.5, 100]
 
     # alts = [100, 99, 98, 98.2, 6, 5, 3, -20, -25]
     # tgt_sum = 78.2
 
@@ -131,8 +130,8 @@
     print('可能的序列:')
     for result in results:
         print(result, end='')
         s = sum(result)
         print('\n和:', s, '\n目标和:', tgt_sum, '\n差:', tgt_sum-s, end='\n\n')
 
 
-    print('used time {}s.'.format(round(time.time() - start_time,6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.38/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     adds_process : list
         搜索中间过程
     '''
 
     adds_process = [] if save_process else None
 
     if log_info:
-        start_time = time.time()
+        start_time = time.monotonic()
 
     if len(alts) == 0:
         return [], [], adds_process
 
     alts.sort(reverse=True) # 降序（小的数优先进入）
 
     # 初始化，idx_last记录最新进入的数的索引号
@@ -138,15 +138,15 @@
         chosed_addends.append(alts[idx_last])
         if save_process:
             adds_process.append(chosed_addends.copy())
         now_sum += alts[idx_last]
 
     if log_info:
         logger_show('loop_count: {}'.format(loop_count), logger, 'info')
-        logger_show('used time {}s.'.format(round(time.time() - start_time,6)),
+        logger_show('used time {}s.'.format(round(time.monotonic() - start_time,6)),
                     logger, 'info')
 
     return choseds_best, chosed_addends, adds_process
 
 
 if __name__ == '__main__':
     alts = [1201008.0, 1254715.0, 1269351.0, 1277352.0, 1291173.81, 1317600.0,
```

### Comparing `dramkit-0.4.4/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.38/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/gentools.py` & `dramkit-0.5.38/dramkit/gentools.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import operator
 import argparse
 import datetime
 import traceback
 import numpy as np
 import pandas as pd
 import urllib.parse
+from tqdm import tqdm
+from collections import Counter
 from functools import reduce, wraps
 from random import randint, random, uniform
 from dramkit.logtools.utils_logger import logger_show
 from dramkit.speedup.multi_thread import SingleThread
 
 
 PYTHON_VERSION = float(sys.version[:3])
@@ -36,51 +38,71 @@
     >>> tr.useds()
     >>> time.sleep(60)
     >>> tr.usedm()
     >>> time.sleep(5)
     >>> tr.used()
     '''
     
-    def __init__(self):
-        self.strt_tm = time.time()
+    def __init__(self, monotonic=True, logger=None):
+        self.monotonic = monotonic
+        self.strt_tm = self.now()
+        self.end_tm = None
+        self.logger = logger
+        
+    def _check_logger(self, logger=None):
+        if isnull(logger):
+            return self.logger
+        return logger
+        
+    def now(self):
+        if self.monotonic:
+            return time.monotonic()
+        else:
+            return time.time()
         
     def used(self, logger=None):
-        s = time.time() - self.strt_tm
+        self.end_tm = self.now()
+        s = self.end_tm - self.strt_tm
         if s < 60:
             s = round(s, 6)
-            logger_show('used time: %ss.'%s, logger)
+            logger_show('used time: %ss.'%s, self._check_logger(logger))
         elif s < 3600:
             m, s = divmod(s, 60)
             logger_show('used time: %sm, %ss.'%(m, round(s, 2)),
-                        logger)
+                        self._check_logger(logger))
         else:
             h, s = divmod(s, 3600)
             m, s = divmod(s, 60)
             logger_show('used time: %sh, %sm, %ss.'%(h, m, round(s, 2)),
-                        logger)
+                        self._check_logger(logger))
         return s
     
     def useds(self, logger=None):
-        s = round(time.time()-self.strt_tm, 6)
-        logger_show('used time: %ss.'%s, logger)
+        self.end_tm = self.now()
+        s = round(self.end_tm-self.strt_tm, 6)
+        logger_show('used time: %ss.'%s, self._check_logger(logger))
         return s
         
     def usedm(self, logger=None):
-        s = time.time()-self.strt_tm
+        self.end_tm = self.now()
+        s = self.end_tm - self.strt_tm
         m = round(s/60, 6)
-        logger_show('used time: %sm.'%m, logger)
+        logger_show('used time: %sm.'%m, self._check_logger(logger))
         return s
     
     
 class DirtModifyError(Exception):
     pass
 
 
-class StructureObject(object):
-    '''类似于MATLAB结构数组，存放变量，便于直接赋值和查看'''
+class GenObject(object):
+    '''
+    | 创建一个数据类型，用于存放变量值，
+    | 既可以用.key调用，也可以像字典一样调用[key]调用
+    '''
 
     def __init__(self, dirt_modify=True, **kwargs):
         '''初始化'''
         self.set_dirt_modify(dirt_modify)
         self.set_from_dict(kwargs)
         
     @property
@@ -89,95 +111,202 @@
         
     def set_dirt_modify(self, dirt_modify):
         assert isinstance(dirt_modify, bool)
         self.__dirt_modify = dirt_modify
         
     def __setattr__(self, key, value):
         _defaults = ['__dirt_modify']
-        _defaults = ['_StructureObject' + x for x in _defaults]
+        _defaults = ['_%s'%type(self).__name__ + x for x in _defaults]
         if key in _defaults:
             self.__dict__[key] = value
             return
         if self.dirt_modify:
             self.__dict__[key] = value
         else:
-            raise DirtModifyError('不允许直接赋值！')
-            # raise DirtModifyError(
-            #     '不允许直接赋值，请调用`set_key_value`或`set_from_dict`方法！')
+            # raise DirtModifyError('不允许直接赋值！')
+            raise DirtModifyError(
+                  '不允许直接赋值，请调用`set_key_value`或`set_from_dict`方法！')
 
     def __repr__(self):
         '''查看时以key: value格式打印'''
         _defaults = ['__dirt_modify']
-        _defaults = ['_StructureObject' + x for x in _defaults]
+        _defaults = ['_%s'%type(self).__name__ + x for x in _defaults]
         return ''.join('{}: {}\n'.format(k, v) for k, v in self.__dict__.items() \
                        if k not in _defaults)
             
+    def __getitem__(self, key):
+        '''像dict一样通过key获取value'''
+        return self.__dict__[key]
+    
+    def __setitem__(self, key, value):
+        '''像dict一样直接通过key赋值'''
+        self.__setattr__(key, value)
+            
     @property
     def keys(self):
         '''显示所有key'''
         _defaults = ['__dirt_modify']
-        _defaults = ['_StructureObject' + x for x in _defaults]
-        return [x for x in self.__dict__.keys() if x not in _defaults]
+        _defaults = ['_%s'%type(self).__name__ + x for x in _defaults]
+        # return [x for x in self.__dict__.keys() if x not in _defaults]
+        for x in self.__dict__.keys():
+             if x not in _defaults:
+                yield x
+                
+    def listkeys(self):
+        return list(self.keys)
     
     @property
     def items(self):
         _defaults = ['__dirt_modify']
-        _defaults = ['_StructureObject' + x for x in _defaults]
+        _defaults = ['_%s'%type(self).__name__ + x for x in _defaults]
         for x in self.__dict__.keys():
             if not x in _defaults:
                 d = (x, eval('self.{}'.format(x)))
                 yield d
+                
+    def listitems(self):
+        return list(self.items)
     
     def set_key_value(self, key, value):
         self.__dict__[key] = value
     
     def set_from_dict(self, d):
         '''通过dict批量增加属性变量'''
         assert isinstance(d, dict), '必须为dict格式'
         self.__dict__.update(d)
         
+    def update(self, o):
+        '''像dict一样通过update函数传入字典进行更新'''
+        assert isinstance(o, (dict, list, tuple, type(self)))
+        if isinstance(o, dict):
+            self.set_from_dict(o)
+        else:
+            self.merge(o)
+        
     def merge(self, o):
         '''从另一个对象中合并属性和值'''
         assert isinstance(o, (list, tuple, type(self)))
         if isinstance(o, type(self)):
             o = [o]
+        assert all([isinstance(x, type(self)) for x in o])
         for x in o:
             for key in x.keys:
                 exec('self.set_key_value(key, x.{})'.format(key))
     
     def copy(self):
         return copy.deepcopy(self)
     
     def pop(self, key):
         '''删除属性变量key，有返回'''
         return self.__dict__.pop(key)
-    
+
     def remove(self, key):
         '''删除属性变量key，无返回'''
         del self.__dict__[key]
-    
+
     def clear(self):
         '''清空所有属性变量'''
         self.__dict__.clear()
         
         
-def run_func_with_timeout(func, args, timeout=10):
+class DeprecatedError(Exception):
+    pass
+
+
+class StructureObject(object):
+    def __init__(self, *args, **kwargs):
+        raise DeprecatedError('`StructureObject`已弃用，请调用`GenObject`!')
+        
+        
+def run_func_with_timeout_thread(func, *args,
+                                 timeout=10,
+                                 logger_error=False,
+                                 logger_timeout=None,
+                                 timeout_show_str=None,
+                                 kill_when_timeout=True,
+                                 **kwargs):
     '''
     | 限定时间(timeout秒)执行函数func，若限定时间内未执行完毕，返回None
     | args为tuple或list，为func函数接受的参数列表
+    
+    | 注：在线程中强制结束函数可能导致未知错误，
+    | 比如文件资源打开了但是强制结束时不能关闭
     '''
-    task = SingleThread(func, args, False) # 创建线程
+    # 创建线程
+    task = SingleThread(func, args, kwargs,
+                        logger=logger_error,
+                        # daemon=True
+                        )
     task.start() # 启动线程
     task.join(timeout=timeout) # 最大执行时间
-
-    # 若超时后，线程依旧运行，则强制结束
+    # 超时处理
     if task.is_alive():
-        task.stop_thread()
-
+        if not isnull(timeout_show_str):
+            logger_show(timeout_show_str, logger_timeout, 'warn')
+        # 强制结束
+        if kill_when_timeout:
+            task.stop_thread()
+            # task.join()
     return task.get_result()
+
+
+def with_timeout_thread(timeout=30,
+                        logger_error=None,
+                        logger_timeout=None,
+                        timeout_show_str=None,
+                        kill_when_timeout=True):
+    '''
+    | 作为装饰器在指定时间timeout(秒)内运行函数，超时则结束运行
+    | 通过控制线程实现
+
+    Examples
+    --------
+    .. code-block:: python
+        :linenos:
+
+        import os
+        import pandas as pd
+        from dramkit.gentools import tmprint
+        
+        df1 = pd.DataFrame([[1, 2], [3, 4]])
+        df2 = pd.DataFrame([[5, 6], [7, 8]])
+        df1.to_excel('./_test/with_timeout_thread_test_df.xlsx')
+        TIMEOUT = 3
+        
+        @with_timeout_thread(TIMEOUT,
+                             logger_error=False
+                             )
+        def func(x):
+            with open('./_test/with_timeout_thread_test_df.xlsx') as f:
+                tmprint('sleeping...')
+                time.sleep(5)
+            df2.to_excel('./_test/with_timeout_thread_test_df.xlsx')
+            return x
+        
+        def test():
+            res = func('test')
+            print('res:', res)
+            os.remove('./_test/with_timeout_thread_test_df.xlsx')
+            return res
+            
+    >>> res = test()
+    '''
+    def transfunc(func):
+        @wraps(func)
+        def timeouter(*args, **kwargs):
+            '''尝试在指定时间内运行func，超时则结束运行'''
+            return run_func_with_timeout_thread(
+                    func, *args, timeout=timeout, 
+                    logger_error=logger_error,
+                    logger_timeout=logger_timeout,
+                    timeout_show_str=timeout_show_str,
+                    kill_when_timeout=kill_when_timeout,
+                    **kwargs)
+        return timeouter
+    return transfunc
         
         
 def try_repeat_run(n_max_run=3, logger=None, sleep_seconds=0,
                    force_rep=False):
     '''
     | 作为装饰器尝试多次运行指定函数
     | 使用场景：第一次运行可能出错，需要再次运行(比如取数据时第一次可能连接超时，需要再取一次)
@@ -279,19 +408,38 @@
         from dramkit import simple_logger
         logger = simple_logger()
 
         @log_used_time(logger)
         def wait():
             print('wait...')
             time.sleep(3)
+            
+            
+        @log_used_time()
+        def wait1(logger=None):
+            print('wait...')
+            time.sleep(3)
+            
+        @log_used_time(simple_logger(logname='test'))
+        def wait2(logger=None):
+            print('wait...')
+            time.sleep(3)
+            
+        @log_used_time(False)
+        def wait3(logger=None):
+            print('wait...')
+            time.sleep(3)
 
     >>> wait()
     wait...
-    2021-12-28 12:39:54,013 -utils_logger.py[line: 32] -INFO:
-        --func `wait` run time: 3.000383s.
+    func `wait` run time: 3.0s.
+        [INFO: 2023-04-20 13:39:37,292]
+    >>> wait1(logger=simple_logger('./_test/log_used_time_test.log'))
+    >>> wait2(logger=simple_logger('./_test/log_used_time_test.log'))    
+    >>> wait3()
 
     See Also
     --------
     :func:`dramkit.gentools.print_used_time`
 
     References
     ----------
@@ -301,19 +449,23 @@
     - https://www.cnblogs.com/zhzhang/p/11375774.html
     - https://blog.csdn.net/weixin_33711647/article/details/92549215
     '''
     def transfunc(func):
         @wraps(func)
         def timer(*args, **kwargs):
             '''运行func并记录用时'''
-            t0 = time.time()
+            t0 = time.monotonic()
             result = func(*args, **kwargs)
-            t = time.time()
-            logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
-                        logger, 'info')
+            t = time.monotonic()
+            if isnull(logger) and 'logger' in kwargs:
+                logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
+                            kwargs['logger'], 'info')
+            else:
+                logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)),
+                            logger, 'info')
             return result
         return timer
     return transfunc
 
 
 def print_used_time(func):
     '''
@@ -324,40 +476,49 @@
     func : function
         需要记录运行用时的函数
     
     Examples
     --------
     .. code-block:: python
         :linenos:
+            
+        from dramkit import simple_logger
 
         @print_used_time
-        def wait():
+        def wait(x, **kwargs):
             print('wait...')
-            time.sleep(3)
+            time.sleep(x)
 
-    >>> wait()
+    >>> wait(3)
     wait...
-    func `wait` run time: 3.008314s.
+    func `wait` run time: 3.0s.
+    >>> wait(x=3, b=5, logger=simple_logger())
+    wait...
+    func `wait` run time: 3.0s.
+        [INFO: 2023-04-20 13:22:32,643]
 
     See Also
     --------
     :func:`dramkit.gentools.log_used_time`
 
     References
     ----------
     - https://www.cnblogs.com/slysky/p/9777424.html
     - https://www.cnblogs.com/zhzhang/p/11375574.html
     '''
     @wraps(func)
     def timer(*args, **kwargs):
         '''运行func并print用时'''
-        t0 = time.time()
+        t0 = time.monotonic()
         result = func(*args, **kwargs)
-        t = time.time()
-        print('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)))
+        t = time.monotonic()
+        if 'logger' in kwargs:
+            logger_show('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)), kwargs['logger'])
+        else:
+            print('func `%s` run time: %ss.'%(func.__name__, round(t-t0, 6)))
         return result
     return timer
 
 
 def func_res_process_decorator(func_res, *args_res, **kwargs_res):
     '''
     作为装饰器处理函数输出结果
@@ -385,26 +546,34 @@
 
 
 def func_runtime_test(func, n=10000, return_all=False,
                       *args, **kwargs):
     '''函数性能（运行时间）测试，n设置测试运行测试'''
     if not return_all:
         tr = TimeRecoder()
-        for _ in range(n):
+        for _ in tqdm(range(n)):
+        # for _ in range(n):
+        #     pstr = '{}/{}, {}%'.format(_+1, n, round(100*(_+1)/n, 2))
+        #     print('\r', pstr, end='', flush=True)
             res = func(*args, **kwargs)
-        tr.useds()
-        return res
+        # print('')
+        t = tr.useds()
+        return t, res
     else:
         tr = TimeRecoder()
         res_all = []
-        for _ in range(n):
+        for _ in tqdm(range(n)):
+        # for _ in range(n):
+        #     pstr = '{}/{}, {}%'.format(_+1, n, round(100*(_+1)/n, 2))
+        #     print('\r', pstr, end='', flush=True)
             res = func(*args, **kwargs)
             res_all.append(res)
-        tr.useds()
-        return res_all
+        # print('')
+        t = tr.useds()
+        return t, res_all
     
     
 def check_list_arg(arg, allow_none=False):
     '''检查arg，若其不是list或tuple，则转为列表'''
     if not allow_none and isnull(arg):
         raise ValueError('不支持`arg`为无效值！')
     if isnull(arg):
@@ -468,15 +637,17 @@
     >>> get_update_kwargs(key, arg, kwargs, func_update='replace')
     (['aa', 'aa_'], {'b': 'b'})
     >>> key, arg = 'a', 'aa_'
     >>> kwargs = {'a': ['a'], 'b': 'b'}
     >>> get_update_kwargs(key, arg, kwargs)
     (['a', 'aa_'], {'b': 'b'})
     '''
-
+    
+    kwargs = kwargs.copy()
+    
     def _default_update(arg, arg_old):
         if isinstance(arg, dict):
             assert isinstance(arg_old, dict) or isnull(arg_old)
             arg_new = {} if isnull(arg_old) else arg_old
             arg_new.update(arg)
         elif isinstance(arg, list):
             assert isinstance(arg_old, list) or isnull(arg_old)
@@ -1900,14 +2071,18 @@
               sort_cols=None, ascendings=True,
               method='merge', logger=None):
     '''
     | 合并df_new到df_old
     | 注意：df_old和df_new不应该设置index
     | 注意：用merge处理当数据量大时占空间很大，method应设置为`concat`
     
+    TODO
+    ----
+    增加对各列的类型进行指定的参数设置
+    
     Examples
     --------
     >>> df_old = pd.DataFrame({'id1': [1, 2, 3, 4, 5],
     ...                        'id2': [2, 3, 4, 5, 6],
     ...                        'col1': ['a', 'b', 'c', 'd', 'e'],
     ...                        'col2': [2, 4, 6, 8, 10]})
     >>> df_new = pd.DataFrame({'id1': [3, 4, 5, 6, 7],
@@ -2481,52 +2656,53 @@
     df = df.stack(dropna=dropna)
     df = pd.DataFrame(df, columns=[col_val_name])
     df.index.names = idx_cols + [col_name]
     df = df.reset_index()
     return df
 
 
-def df_freq_low2high(df, tcol, id_cols, vcols=None,
+def df_freq_low2high(df, tcol, idcols, vcols=None,
                      tmin=None, tmax=None, keepna=True):
     '''
     数据填充为日频
     
     TODO
     ----
+    - idcols唯一性检查
     - 填充时选择交易日或工作日参数设置
     - idx_cols中有nan时检查和处理
     - 其他参数/变量规范重写
     - 日期格式不写死，根据tcol列转化
     '''
     vcols = check_list_arg(vcols, allow_none=True)
-    id_cols = check_list_arg(id_cols)
+    idcols = check_list_arg(idcols)
     if isnull(vcols):
-        vcols = [x for x in df.columns if not x in id_cols+[tcol]]
+        vcols = [x for x in df.columns if not x in idcols+[tcol]]
     if df.shape[0] == 0:
-        return pd.DataFrame(columns=[tcol]+id_cols+vcols)
+        return pd.DataFrame(columns=[tcol]+idcols+vcols)
     if isnull(tmin):
         tmin = df[tcol].min()
     if isnull(tmax):
         # tmax = datetime.datetime.today().strftime('%Y%m%d')
         tmax = df[tcol].max()
     if tmin == tmax:
-        return df[[tcol]+id_cols+vcols]
+        return df[[tcol]+idcols+vcols]
     dates = pd.date_range(tmin, tmax)
     dates = [x.strftime('%Y%m%d') for x in dates]
     if keepna:
         df = df.fillna('__tmp_None_tmp__')
-    df = df.pivot_table(values=vcols, index=tcol, columns=id_cols,
+    df = df.pivot_table(values=vcols, index=tcol, columns=idcols,
                         aggfunc=lambda x: x)
     index_all = list(set(dates + list(df.index)))
     index_all.sort()
     df = df.reindex(index=index_all)
     df = df.fillna(method='ffill')#.fillna(method='bfill')
-    df = df.stack(level=id_cols).reset_index()
+    df = df.stack(level=idcols).reset_index()
     df = df.replace({'__tmp_None_tmp__': np.nan})
-    df = df.sort_values(id_cols+[tcol])
+    df = df.sort_values(idcols+[tcol])
     return df
 
 
 def get_first_appear_index(series, values, ascending=False,
                            return_iloc=False):
     '''获取values中的值在series中第一次出现时的索引'''
     raise NotImplementedError
@@ -2818,14 +2994,24 @@
     assert all([isinstance(x, list) for x in lists])
     newlist = []
     for item in lists:
         newlist.extend(item)
     return newlist
 
 
+def get_lists_inter(lists):
+    '''获取多个列表的交集'''
+    assert isinstance(lists, (list, tuple))
+    assert all([isinstance(x, (list, tuple)) for x in lists])
+    res = set(lists[0])
+    for x in lists[1:]:
+        res = res.intersection(set(x))
+    return list(res)
+
+
 def list_eq(l1, l2, order=True):
     '''判断两个列表l1和l2是否相等，若orde为False，则只要元素相同即判断为相等'''
     if order:
         return operator.eq(l1, l2)
     return set(l1) == set(l2)
 
 
@@ -2876,21 +3062,33 @@
     if dirt == 'before':
         res.insert(idx, val)
     else:
         res.insert(idx+1, val)
     return res
 
 
+def count_list(l):
+    '''对l中的元素计数，返回dict'''
+    # return dict(Counter(l))
+    return Counter(l)
+
+
+def tmprint(*args, **kwargs):
+    print(*args, **kwargs)
+    print('    [time: {}]'.format(
+        datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')))
+
+
 def url2chn(url):
     '''将url中的中文乱码（实际上为utf-8）转化为正常url'''
     return urllib.parse.unquote(url)
 
 
 def replace_con_blank(string, to):
-    '''将string中连续空格替换为to'''
+    '''将string中连续空格替换为to指定字符'''
     return re.sub(' +', to, string)
 
 
 def change_dict_key(d, func_key_map):
     '''修改字典d中的key值，即d[k]=v变成d[func_key_map(k)]=v'''
     return {func_key_map(k): v for k, v in d.items()}
 
@@ -2984,20 +3182,49 @@
             args_info.append((['--%s'%arg], {'required': True, 'type': func_args['annotations'][arg]}))
     for arg, default in defaults.items():
         if arg not in func_args['annotations']:
             args_info.append((['--%s'%arg], {'default': default}))
         else:
             args_info.append((['--%s'%arg], {'default': default, 'type': func_args['annotations'][arg]}))
     return parse_args(args_info)
+
+
+def get_topn_names(df, n=1, max_or_min='max',
+                   col_or_row='col'):
+    '''
+    获取df中值最大/小的前n列/行的名称
+    
+    Examples
+    --------
+    >>> d = {'A': [30, 2, 6, 4, 5],
+    ...      'B': [6, 7, 80, 5, 10],
+    ...      'C': [11, 12, 13, 14, 15],
+    ...      'D': [16, 17, 18, 19, 20],
+    ...      'E': [21, 22, 23, 24, 25]}
+    >>> df = pd.DataFrame(d, index=['a', 'b', 'c', 'd', 'e'])
+    >>> res = get_topn_names(df, n=2)
+    >>> res1 = get_topn_names(df, n=2, col_or_row='row')
+    '''
+    assert max_or_min.lower() in ['max', 'min']
+    assert col_or_row.lower() in ['col', 'row']
+    axis = 1 if col_or_row.lower() == 'col' else 0
+    if max_or_min.lower() == 'max':
+        res = df.apply(lambda x:
+                 x.nlargest(n).index.tolist(), axis=axis)
+    else:
+        res = df.apply(lambda x:
+                 x.nsmallest(n).index.tolist(), axis=axis)
+    return res
     
 
 if __name__ == '__main__':
     from dramkit import load_csv, plot_series
     from finfactory.fintools.fintools import cci
-
+    
+    tr = TimeRecoder()
     def test():
         # 50ETF日线行情------------------------------------------------------------
         fpath = './_test/510050.SH_daily_qfq.csv'
         data = load_csv(fpath)
         data.set_index('date', drop=False, inplace=True)
         data.index.name = 'time'
     
@@ -3030,7 +3257,8 @@
                                         'close':
                                     [['cci_100_', (-1, 1), ('r^', 'bv'), False]]},
                     xparls_info={'cci': [(100, 'r', '-', 1.3),
                                          (-100, 'r', '-', 1.3)]},
                     figsize=(8, 7), grids=True)
         return data
     # res = test()
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/install_check.py` & `dramkit-0.5.38/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/iotools.py` & `dramkit-0.5.38/dramkit/iotools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,146 @@
 # -*- coding: utf-8 -*-
 
 import re
 import os
+import sys
+import time
 import json
 import yaml
 import pickle
 import shutil
+import logging
 import zipfile
 import socket
 import inspect
+import platform
 import requests
 import traceback
 import subprocess
 import py_compile
 import pandas as pd
 from tqdm import tqdm
+from pathlib import Path
+from urllib.request import urlopen
 from dramkit.gentools import (isnull,
                               check_list_arg,
                               get_update_kwargs,
                               cut_range_to_subs,
                               get_tmp_col,
                               merge_df,
-                              update_df)
+                              update_df,
+                              run_func_with_timeout_thread)
 from dramkit.logtools.utils_logger import (logger_show,
                                            close_log_file)
 from dramkit.datetimetools import timestamp2str
-from dramkit.speedup.multi_thread import SingleThread
-from dramkit.speedup.multi_process import multi_process_concurrent
+from dramkit.speedup.multi_process_concurrent import multi_process_concurrent
+
+_WINDOWS_SYSTEM = 'windows' in platform.system().lower()
+
+_SP = ' '
+_CR = '\r'
+_LF = '\n'
+_CRLF = _CR + _LF
+
+
+class GetInputTimeoutError(Exception):
+    pass
+
+
+def _echo(string):
+    sys.stdout.write(string)
+    sys.stdout.flush()
+    
+    
+def _check_hint_str(timeout, hint_str):
+    if isnull(hint_str):
+        hint_str = 'Please input in {} seconds:\n'.format(timeout)
+    return hint_str
+
+
+def get_input_timeout_win(timeout=10, hint_str=None):
+    '''
+    | windows下设置在等待时间内获取input
+    | https://pypi.org/project/inputimeout/
+    '''
+    import msvcrt
+    hint_str = _check_hint_str(timeout, hint_str)
+    _echo(hint_str)
+    begin = time.monotonic()
+    end = begin + timeout
+    line = ''
+    while time.monotonic() < end:
+        if msvcrt.kbhit():
+            c = msvcrt.getwche()
+            if c in (_CR, _LF):
+                _echo(_CRLF)
+                return line
+            if c == '\003':
+                raise KeyboardInterrupt
+            if c == '\b':
+                line = line[:-1]
+                cover = _SP * len(hint_str + line + _SP)
+                _echo(''.join([_CR, cover, _CR, hint_str, line]))
+            else:
+                line += c
+        time.sleep(0.05)
+    _echo(_CRLF)
+    raise GetInputTimeoutError
+    
+    
+def get_input_timeout_notwin(timeout=10, hint_str=None):
+    '''
+    | 非windows下设置在等待时间内获取input
+    | https://pypi.org/project/inputimeout/
+    '''
+    import selectors
+    import termios
+    hint_str = _check_hint_str(timeout, hint_str)
+    _echo(hint_str)
+    sel = selectors.DefaultSelector()
+    sel.register(sys.stdin, selectors.EVENT_READ)
+    events = sel.select(timeout)
+    if events:
+        key, _ = events[0]
+        return key.fileobj.readline().rstrip(_LF)
+    else:
+        _echo(_LF)
+        termios.tcflush(sys.stdin, termios.TCIFLUSH)
+        raise GetInputTimeoutError
+    
+    
+def get_input_timeout(timeout=10, hint_str=None, logger=None):
+    try:
+        if _WINDOWS_SYSTEM:
+            res = get_input_timeout_win(timeout=timeout, hint_str=hint_str)
+        else:
+            res = get_input_timeout_notwin(timeout=timeout, hint_str=hint_str)
+    except GetInputTimeoutError:
+        logger_show('超时未接收到输入，返回None！', logger, 'warn')
+        res = None
+    return res
 
 
 def get_input_with_timeout(timeout=10, hint_str=None,
                            logger=None):
     '''
     | 通过input函数获取输入
     | 若等待时间超过timeout秒没接收到输入，则返回None
     | hint_str为input函数提示信息
     | 参考：https://zhuanlan.zhihu.com/p/367634630
     '''
     def _get_input(hint_str):
         str_input = input(hint_str)
-        return str_input
-    
-    if hint_str is None:
-        hint_str = 'Please input:\n'
-
-    task = SingleThread(_get_input, (hint_str,), False) # 创建线程
-    task.start() # 启动线程
-    task.join(timeout=timeout) # 最大执行时间
-
-    # 若超时后，线程依旧运行，则强制结束
-    if task.is_alive():
-        logger_show('超时未接收到输入，返回None！', logger, 'warn')
-        task.stop_thread()
-
-    return task.get_result()
+        return str_input    
+    hint_str = _check_hint_str(timeout, hint_str)
+    return run_func_with_timeout_thread(
+            _get_input, hint_str, timeout=timeout,
+            timeout_show_str='超时未接收到输入，返回None！',
+            logger_error=False, logger_timeout=logger,
+            kill_when_timeout=True)
 
 
 def get_input_multi_line(end_word='end', end_char='',
                          hint_str=None, hint_lineno=True):
     '''
     | input读取多行输入（包括回车换行符也会被保留）
     | end_word设置结束词，当在一行里面输入完整结束词，则表示输入完毕
@@ -155,30 +238,24 @@
     :returns: `dict` - 返回读取数据
     '''
 
     if not os.path.exists(fpath):
         logger_show('文件不存在，返回None：{}'.format(fpath),
                     logger, 'warn')
         return None
-
-    try:
-        with open(fpath, 'r', encoding=encoding) as f:
-            data_json = json.load(f)
-    except:
+                
+    for en in [encoding, 'utf-8', 'gbk', None]:
         try:
-            with open(fpath, 'r', encoding='utf-8') as f:
+            with open(fpath, 'r', encoding=en) as f:
                 data_json = json.load(f)
+            break
         except:
-            try:
-                with open(fpath, 'r', encoding='gbk') as f:
-                    data_json = json.load(f)
-            except:
-                logger_show('读取%s出错，请检查文件（如编码或文件末尾多余字符等问题）！'%fpath,
-                            logger, 'error')
-                raise
+            logger_show('读取%s出错，请检查文件（如编码或文件末尾多余字符等问题）！'%fpath,
+                        logger, 'error')
+            raise
 
     return data_json
 
 
 def write_json(data, fpath, encoding=None, mode='w', **kwargs):
     '''
     把data写入json格式文件
@@ -332,14 +409,150 @@
                 data.columns = cols
             else:
                 data = pd.DataFrame(data)
 
     return data
 
 
+def _get_pd_ftype(fpath, ftype):
+    if isnull(ftype):
+        ftype = get_file_ext_type(fpath)
+    ftype = ftype.replace('.', '')
+    if ftype in ['xls', 'xlsx']:
+        ftype = 'excel'
+    if ftype in ['sav']:
+        ftype = 'spss'   
+    if ftype in ['dta']:
+        ftype = 'stata'
+    if ftype in ['pk', 'pkl']:
+        ftype = 'pickle'
+    return ftype
+
+
+def _drop_unname_cols(df):
+    _cols = [x for x in df.columns if 'unnamed:' in str(x).lower()]
+    if len(_cols) > 0:
+        df = df.drop(_cols, axis=1)
+    return df
+
+
+def df2file_pd(df, fpath, ftype=None, **kwargs):
+    '''pandas.DataFrame写入文件'''
+    ftype = _get_pd_ftype(fpath, ftype)
+    exec('df.to_{}(fpath, **kwargs)'.format(ftype))
+
+
+def _pd_load_df_check(fpath, ftype, logger):
+    if not os.path.exists(fpath):
+        logger_show('文件不存在，返回None：{}!'.format(fpath),
+                    logger, 'warn')
+        return None
+    ftype = _get_pd_ftype(fpath, ftype)
+    allows = [x.split('_')[-1] for x in dir(pd) if x.startswith('read_')]
+    if ftype not in allows:
+        logger_show('不支持的文件类型: `{}`！'.format(ftype))
+        raise
+    read_func = eval('pd.read_{}'.format(ftype))
+    return read_func
+
+
+def _process_df_pd_big(read_func, fpath,
+                       chunksize=100000,
+                       read_kwargs={},
+                       del_unname_cols=True,
+                       process_func=None,
+                       process_args=(),
+                       process_kwargs={},
+                       return_df=True):
+    df_iter = read_func(fpath, chunksize=chunksize,
+                        **read_kwargs)
+    res = []
+    for tmp in df_iter:
+        if del_unname_cols:
+            tmp = _drop_unname_cols(tmp)
+        if not isnull(process_func):
+            tmp = process_func(tmp, *process_args, **process_kwargs)
+        res.append(tmp)
+    if return_df:
+        res = pd.concat(res, axis=0)
+    return res
+
+
+def process_df_pd_big(fpath: str,
+                      ftype: str = None,
+                      chunksize : int = 100000,
+                      del_unname_cols: bool = True,
+                      logger: logging.Logger = None,
+                      read_kwargs: dict = {},
+                      process_func=None,
+                      process_args: tuple = (),
+                      process_kwargs: dict = {},
+                      return_df: bool = True):
+    '''用pandas读取大数据文件并分批处理，返回处理后的结果'''
+    read_func = _pd_load_df_check(fpath, ftype, logger)
+    if isnull(read_func):
+        return None
+    res = _process_df_pd_big(read_func, fpath,
+                             chunksize=chunksize,
+                             read_kwargs=read_kwargs,
+                             del_unname_cols=del_unname_cols,
+                             process_func=process_func,
+                             process_args=process_args,
+                             process_kwargs=process_kwargs,
+                             return_df=return_df)
+    return res
+
+
+def load_df_pd(fpath: str,
+               ftype: str = None,
+               del_unname_cols: bool = True,
+               encoding: str = None,
+               logger: logging.Logger = None,
+               **kwargs):
+    '''用pandas读取文件，返回DataFrame'''
+    
+    read_func = _pd_load_df_check(fpath, ftype, logger)
+    if isnull(read_func):
+        return None
+    
+    _big = False
+    if 'chunksize' in kwargs and not isnull(kwargs['chunksize']):
+        _big = True
+        chunksize, kwargs = get_update_kwargs(
+            'chunksize', None, kwargs, func_update=False)
+
+    data = None
+    for en in [encoding, 'utf-8', 'gbk']:
+        try:
+            if not _big:
+                data = read_func(fpath, encoding=en, **kwargs)
+            else:
+                kwargs.update({'encoding': en})
+                data = _process_df_pd_big(read_func, fpath,
+                                          chunksize=chunksize,
+                                          del_unname_cols=False,
+                                          read_kwargs=kwargs)
+            break
+        except:
+            pass
+    if isnull(data):
+        if not _big:
+            data = read_func(fpath, **kwargs)
+        else:
+            data = _process_df_pd_big(read_func, fpath,
+                                      chunksize=chunksize,
+                                      del_unname_cols=False,
+                                      read_kwargs=kwargs)
+
+    if del_unname_cols:
+        data = _drop_unname_cols(data)
+
+    return data
+
+
 def load_csv(fpath, del_unname_cols=True, encoding=None,
              logger=None, **kwargs):
     '''
     用pandas读取csv数据
 
     Parameters
     ----------
@@ -353,74 +566,86 @@
         日志记录器
     **kwargs :
         其它 ``pd.read_csv`` 支持的参数
 
 
     :returns: `pandas.DataFrame` - 读取的数据
     '''
+    return load_df_pd(fpath, ftype='csv',
+                      del_unname_cols=del_unname_cols,
+                      encoding=encoding,
+                      logger=logger,
+                      **kwargs)
 
-    if not os.path.exists(fpath):
-        logger_show('文件不存在，返回None：{}!'.format(fpath),
-                    logger, 'warn')
-        return None
 
-    try:
-        data = pd.read_csv(fpath, encoding=encoding, **kwargs)
-    except:
-        try:
-            data = pd.read_csv(fpath, encoding='utf-8', **kwargs)
-        except:
-            try:
-                data = pd.read_csv(fpath, encoding='gbk', **kwargs)
-            except:
-                data = pd.read_csv(fpath, **kwargs)
-
-    if del_unname_cols:
-        del_cols = [x for x in data.columns if 'Unnamed:' in str(x)]
-        if len(del_cols) > 0:
-            data.drop(del_cols, axis=1, inplace=True)
-
-    return data
-
-
-def load_csvs(fpaths,
-              kwargs_sort={},
-              kwargs_drop_dup={},
-              **kwargs_loadcsv):
+def load_dfs_pd(fpaths,
+                kwargs_sort={},
+                kwargs_drop_dup={},
+                mark_file=False,
+                **kwargs_loaddf):
     '''
-    读取指定路径列表中所有的csv文件，整合到一个df里面
+    读取指定路径列表中所有的dataframe数据文件，整合到一个df里面
 
     Parameters
     ----------
     fpaths : list
         文件夹路径列表
     kwargs_sort : dict
         设置sort_values接受的排序参数
     kwargs_drop_dup : dict
         设置drop_duplicates接受的去重参数
-    **kwargs_loadcsv :
-        :func:`dramkit.iotools.load_csv` 接受的其它参数
+    **kwargs_loaddf :
+        :func:`dramkit.iotools.load_df_pd` 接受的其它参数
 
 
     :returns: `pandas.DataFrame` - 读取的数据
     '''
     data = []
     for fpath in tqdm(fpaths):
-        df = load_csv(fpath, **kwargs_loadcsv)
+        df = load_df_pd(fpath, **kwargs_loaddf)
+        if mark_file:
+            df[get_tmp_col(df, 'fromfile')] = fpath
         data.append(df)
     data = pd.concat(data, axis=0)
     if len(kwargs_sort) > 0:
         _, kwargs_sort = get_update_kwargs('inplace', True, kwargs_sort)
         data.sort_values(**kwargs_sort, inplace=True)
     if len(kwargs_drop_dup) > 0:
         _, kwargs_drop_dup = get_update_kwargs('inplace', True, kwargs_drop_dup)
         data.drop_duplicates(**kwargs_drop_dup, inplace=True)
     return data
 
 
+def load_csvs(fpaths,
+              kwargs_sort={},
+              kwargs_drop_dup={},
+              **kwargs_loadcsv):
+    '''
+    读取指定路径列表中所有的csv文件，整合到一个df里面
+
+    Parameters
+    ----------
+    fpaths : list
+        文件夹路径列表
+    kwargs_sort : dict
+        设置sort_values接受的排序参数
+    kwargs_drop_dup : dict
+        设置drop_duplicates接受的去重参数
+    **kwargs_loadcsv :
+        :func:`dramkit.iotools.load_dfs_pd` 接受的其它参数
+
+
+    :returns: `pandas.DataFrame` - 读取的数据
+    '''
+    return load_dfs_pd(fpaths,
+                       kwargs_sort=kwargs_sort,
+                       kwargs_drop_dup=kwargs_drop_dup,
+                       **kwargs_loadcsv)
+
+
 def load_csvs_dir(fdir,
                   kwargs_sort={},
                   kwargs_drop_dup={},
                   **kwargs_loadcsv):
     '''
     读取指定文件夹中所有的csv文件，整合到一个df里面
 
@@ -429,144 +654,218 @@
     fdir : str
         文件夹路径
     kwargs_sort : dict
         设置sort_values接受的排序参数
     kwargs_drop_dup : dict
         设置drop_duplicates接受的去重参数
     **kwargs_loadcsv :
-        :func:`dramkit.iotools.load_csv` 接受的其它参数
+        :func:`dramkit.iotools.load_dfs_pd` 接受的其它参数
 
 
     :returns: `pandas.DataFrame` - 读取的数据
     '''
     files = os.listdir(fdir)
     files = [os.path.join(fdir, x) for x in files if x[-4:] == '.csv']
     data = load_csvs(files, kwargs_sort, kwargs_drop_dup,
                      **kwargs_loadcsv)
     return data
 
 
+def load_excels(fdirorfpaths,
+                kwargs_sort={},
+                kwargs_drop_dup={},
+                **kwargs_readexcel):
+    '''
+    读取指定文件夹中所有的excel文件，整合到一个df里面
+
+    Parameters
+    ----------
+    fdirorfpaths : str, list
+        Excel文件所在文件夹路径或Excel文件路径列表
+    kwargs_sort : dict
+        设置sort_values接受的排序参数
+    kwargs_drop_dup : dict
+        设置drop_duplicates接受的去重参数
+    **kwargs_readexcel :
+        ``dramkit.iotools.load_dfs_pd`` 接受的其它参数
+
+
+    :returns: `pandas.DataFrame` - 读取的数据
+    '''
+    assert isinstance(fdirorfpaths, (str, list, tuple, set))
+    if isinstance(fdirorfpaths, str):
+        fpaths = os.listdir(fdirorfpaths)
+        fpaths = [os.path.join(fdirorfpaths, x) for x in fpaths if x[-4:] == '.xls' or x[-5:] == '.xlsx']
+    else:
+        fpaths = fdirorfpaths
+    return load_dfs_pd(fpaths,
+                       kwargs_sort=kwargs_sort,
+                       kwargs_drop_dup=kwargs_drop_dup,
+                       **kwargs_readexcel)
+
+
 def archive_df(df_old, df_new, idcols=None,
                del_dup_cols=None, rep_keep='new',
                sort_cols=None, ascendings=True,
-               file_type='.csv', save_path=None,
-               kwargs_read={}, kwargs_save={},
-               method='merge', logger=None):
+               old_ftype=None, new_ftype=None,
+               save_ftype=None, save_path=None,
+               kwargs_read_old={}, kwargs_read_new={},
+               kwargs_save={}, method='merge',
+               logger=None):
     '''
     合并df_new和df_old，再排序、去重、写入csv或excel
     '''
-    assert file_type in ['.csv', '.xlsx']
-    read_func = load_csv if file_type == '.csv' else pd.read_excel
     if isinstance(df_new, str):
-        df_new = read_func(df_new, **kwargs_read)
+        df_new = load_df_pd(df_new, ftype=new_ftype,
+                            logger=logger,
+                            **kwargs_read_new)
     if isinstance(df_old, str):
         if os.path.exists(df_old):
             if isnull(df_new) or df_new.shape[0] < 1:
                 return df_old
-            df_old = read_func(df_old, **kwargs_read)
+            df_old = load_df_pd(df_old, ftype=old_ftype,
+                                logger=logger,
+                                **kwargs_read_old)
         else:
             df_old = pd.DataFrame(columns=df_new.columns)
     res = update_df(df_old, df_new,
                     idcols=idcols,
                     del_dup_cols=del_dup_cols,
                     rep_keep=rep_keep,
                     sort_cols=sort_cols,
                     ascendings=ascendings,
                     method=method,
                     logger=logger)
     if not isnull(save_path) and not isnull(res):
-        if file_type == '.csv':
-            res.to_csv(save_path, **kwargs_save)
-        elif file_type == '.xlsx':
-            res.to_excel(save_path, **kwargs_save)
+        if isnull(save_ftype):
+            save_ftype = get_file_ext_type(save_path)
+        save_ftype = save_ftype.replace('.', '')
+        eval('res.to_{}(save_path, **kwargs_save)'.format(save_ftype))
     return res
 
 
-def cut_csv_by_maxline(fpath, max_line=10000,
-                       kwargs_loadcsv={},
-                       kwargs_tocsv={'index': None}):
-    '''
-    csv大文件分割，max_line指定子文件最大行数
-    '''
-    df = load_csv(fpath, **kwargs_loadcsv)
+def add_ext_to_filename(fpath, ext):
+    '''在fpath路径的尾部（扩展名的前面）添加尾缀ext'''
+    fname, ftype = os.path.splitext(fpath)
+    return fname+str(ext)+ftype
+
+
+def cut_dffile_by_maxline(fpath, max_line=10000,
+                          kwargs_loaddf={},
+                          kwargs_tofile={'index': None}):
+    df = load_df_pd(fpath, **kwargs_loaddf)
     subs = cut_range_to_subs(df.shape[0], max_line)
     for k in range(len(subs)):
         i0, i1 = subs[k]
-        path_ = fpath[:-4]+'_'+str(k+1)+'.csv'
+        path_ = add_ext_to_filename(fpath, '_%s'%(k+1))
         df_ = df.iloc[i0:i1, :].copy()
-        df_.to_csv(path_, **kwargs_tocsv)
-
-
-def cut_csv_by_year(fpath, tcol=None,
-                    name_last_year=False,
-                    kwargs_loadcsv={},
-                    kwargs_tocsv={'index': None},
-                    logger=None):
-    '''csv大文件分割，按年份，tcol指定时间列'''
+        df2file_pd(df_, path_, **kwargs_tofile)
+        
+        
+def get_fpath_ext_num(fpath):
+    '''
+    | 给定路径fpath，若不存在，则返回fpath，若存在则返回带数字在后缀的路径
+    | 比如fpath=xxx.y存在，则返回xxx_1.y，xxx_1.y也存在，则返回xxx_2.y
+    '''
+    if not os.path.exists(fpath):
+        return fpath
+    k = 1
+    res = add_ext_to_filename(fpath, '_%s'%k)
+    while os.path.exists(res):
+        res = add_ext_to_filename(fpath, '_{}'.format(k+1))
+        k += 1
+    return res
+        
+        
+def cut_bigdffile_by_maxline(fpath, max_line=100000,
+                             kwargs_loaddf={},
+                             kwargs_tofile={'index': None}):
+    def _df2file(df, fpath, **kwargs):
+        fpath_ = get_fpath_ext_num(fpath)
+        df2file_pd(df, fpath_, ftype=None, **kwargs)
+        return fpath_
+    fpaths = process_df_pd_big(fpath,
+                      ftype=None,
+                      chunksize=max_line,
+                      del_unname_cols=True,
+                      logger=None,
+                      read_kwargs=kwargs_loaddf,
+                      process_func=_df2file,
+                      process_args=(fpath,),
+                      process_kwargs=kwargs_tofile,
+                      return_df=False)
+    return fpaths
+        
+        
+def cut_dffile_by_year(fpath, tcol=None,
+                       name_last_year=False,
+                       kwargs_loaddf={},
+                       kwargs_tofile={'index': None},
+                       kwargs_exists_merge={},
+                       logger=None):
+    '''
+    dataframe大文件分割，按年份，tcol指定时间列
+    
+    TODO
+    ----
+    指定几年的合并为一个文件，而不是固定每一年单独一个文件
+    '''
     
     logger_show('数据读取...', logger)
-    df = load_csv(fpath, **kwargs_loadcsv)
+    df = load_df_pd(fpath, **kwargs_loaddf)
     if tcol is None:
         for col in ['time', 'date']:
             if col in df.columns:
                 tcol = col
                 break
     logger_show('年份识别...', logger)
     d_ = get_tmp_col(df, 'date_')
     y_ = get_tmp_col(df, 'year_')
     df[d_] = pd.to_datetime(df[tcol])
     df[y_] = df[d_].apply(lambda x: x.year)
-    df[y_] = df[y_].astype(str)
+    def _year2int(x):
+        try:
+            return str(int(x))
+        except:
+            return str(x)
+    df[y_] = df[y_].apply(lambda x: _year2int(x))
     years = df[y_].unique().tolist()
     years.sort()
+    for y in years:
+        try:
+            int(y)
+        except:
+            years.remove(y)
+            years.insert(0, y)
     for k in range(len(years)):
         year = years[k]
         logger_show('{}, 数据写入...'.format(year), logger)
         df_ = df[df[y_] == year].copy()
         df_.drop([d_, y_], axis=1, inplace=True)
-        path_ = fpath[:-4]+'_'+year+'.csv'
+        path_ = add_ext_to_filename(fpath, '_'+year)
         if k == len(years)-1:
             if not name_last_year:
                 path_ = fpath
-        df_.to_csv(path_, **kwargs_tocsv)
-
-
-def load_excels(fdir, kwargs_sort={}, kwargs_drop_dup={},
-                **kwargs_readexcel):
-    '''
-    读取指定文件夹中所有的excel文件，整合到一个df里面
-
-    Parameters
-    ----------
-    fdir : str
-        文件夹路径
-    kwargs_sort : dict
-        设置sort_values接受的排序参数
-    kwargs_drop_dup : dict
-        设置drop_duplicates接受的去重参数
-    **kwargs_readexcel :
-        ``pd.read_excel`` 接受的其它参数
+        if len(kwargs_exists_merge) == 0 or k == len(years)-1:
+            df2file_pd(df_, path_, **kwargs_tofile)
+        else:
+            archive_df(path_, df_, save_path=path_, **kwargs_exists_merge)
 
 
-    :returns: `pandas.DataFrame` - 读取的数据
-    '''
-    files = os.listdir(fdir)
-    files = [os.path.join(fdir, x) for x in files if x[-4:] == '.xls' or x[-5:] == '.xlsx']
-    data = []
-    for file in files:
-        df = pd.read_excel(file, **kwargs_readexcel)
-        data.append(df)
-    data = pd.concat(data, axis=0)
-    if len(kwargs_sort) > 0:
-        _, kwargs_sort = get_update_kwargs('inplace', True, kwargs_sort)
-        data.sort_values(**kwargs_sort, inplace=True)
-    if len(kwargs_drop_dup) > 0:
-        _, kwargs_drop_dup = get_update_kwargs('inplace', True, kwargs_drop_dup)
-        data.drop_duplicates(**kwargs_drop_dup, inplace=True)
-    return data
+def cut_csv_by_year(fpath, tcol=None,
+                    name_last_year=False,
+                    kwargs_loadcsv={},
+                    kwargs_tocsv={'index': None},
+                    logger=None):
+    '''csv大文件分割，按年份，tcol指定时间列'''
+    cut_dffile_by_year(fpath, tcol=tcol,
+                       name_last_year=name_last_year,
+                       kwargs_loaddf=kwargs_loadcsv,
+                       kwargs_tocsv=kwargs_tocsv,
+                       logger=logger)
 
 
 def clear_text_file(fpath, encoding=None):
     '''清空文本文件中的内容，保留文件'''
     with open(fpath, 'w', encoding=encoding) as f:
         f.writelines([''])
         
@@ -829,14 +1128,19 @@
     
 def make_dir(dir_path):
     '''新建文件夹'''
     if not os.path.exists(dir_path):
         os.makedirs(dir_path)
         
         
+def make_file_dir(fpath):
+    '''若路径fpath所指文件夹不存在，创建之'''
+    make_dir(get_parent_path(fpath))
+        
+        
 def make_path_dir(fpath):
     '''若fpath所指文件夹路径不存在，则新建之'''
     if isnull(fpath):
         return
     dir_path = os.path.dirname(fpath)
     if not os.path.exists(dir_path) and len(dir_path) > 0:
         make_dir(dir_path)
@@ -961,14 +1265,28 @@
     import uuid
     mac = uuid.UUID(int=uuid.getnode()).hex[-12:]
     # 转大写
     mac = '-'.join([mac[e: e+2] for e in range(0, 11, 2)]).upper()
     return mac
 
 
+def get_ipconfig_all_win(logger=False):
+    res = cmdrun('ipconfig/all', logger=logger).strip()
+    # TODO: 结果转化为dataframe和dict
+    # res = res.replace('\r\n', '\n').split('\n')
+    # res = [x for x in res if len(x.strip()) > 0]
+    return res
+
+
+def get_ipconfig_win(logger=False):
+    # TODO: 结果转化为dataframe和dict
+    res = cmdrun('ipconfig', logger=logger)
+    return res
+
+
 def get_hardware_ids():
     '''
     | 获取电脑硬件序列号信息，包括主板和硬盘序列号、MAC地址、BIOS序列号等
     | 参考：https://blog.csdn.net/lekmoon/article/details/111478394
     '''
     import wmi
     results = {'cpu': [],
@@ -1035,14 +1353,24 @@
     # 可以获取公网ip的网站
     ip_html = requests.get('http://txt.go.sohu.com/ip/soip')
     # 从响应中提取公网ip
     cur_public_ip = re.findall(r'\d+.\d+.\d+.\d+', ip_html.text)
     return cur_public_ip[0]
 
 
+def get_ip_public2():
+    '''
+    | 获取公网ip
+    | https://blog.csdn.net/qq_39147299/article/details/122469840
+    '''
+    # ip = urlopen('http://ip.42.pl/raw').read().decode()
+    ip = requests.get('http://ip.42.pl/raw').content.decode()
+    return ip
+
+
 def get_tasks_info_win():
     '''windows下获取任务信息'''
     res = cmdrun('tasklist', logger=False)
     res = res.split('\n')[1:-1]
     cols = re.sub(' +', ',', res[0].strip()).split(',')
     lens = [len(x) for x in res[1].split(' ')]
     idxs, start, end = [], 0, 0
@@ -1586,24 +1914,40 @@
     reqs_version = df_pip[df_pip['pkg'].isin(reqs)].copy()
     reqs_version.sort_values('pkg', ascending=True, inplace=True)
     reqs_str = '\n'.join(reqs)
     reqs_version_str = '\n'.join(['=='.join(x) for x in reqs_version.values])
     return (reqs, reqs_version), (reqs_str, reqs_version_str), (pkgs, df)
 
 
+def get_filedir(fpath):
+    '''获取fpath路径所在文件夹路径'''
+    return os.path.split(fpath)[0]
+
+
 def get_filename(fpath, with_ext=True):
     '''获取文件名（去除前缀路径），with_ext为False则返回不带后缀'''
     if with_ext:
         return os.path.basename(fpath)
     else:
         return os.path.basename(os.path.splitext(fpath)[0])
 
 
 def get_file_ext_type(fpath):
     '''提取文件扩展名'''
     return os.path.splitext(fpath)[-1]
 
 
+def get_parent_path(path, n=1):
+    '''获取路径path的n级父路径'''
+    f = Path(path)
+    res = eval('f'+'.parent'*n)
+    res = str(res).replace('\\', '/') + '/'
+    # TODO: path以'./'开头时，得到的res不是以'./'开头，原因待查
+    if path.startswith('./') and not res.startswith('./'):
+        res = './' + res
+    return res
+
+
 if __name__ == '__main__':
     fpath = './_test/load_text_test_utf8.csv'
     data1 = load_text(fpath, encoding='gbk')
     data2 = load_csv(fpath, encoding='gbk')
```

### Comparing `dramkit-0.4.4/dramkit/logtools/logger_general.py` & `dramkit-0.5.38/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.38/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.38/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/logtools/utils_logger.py` & `dramkit-0.5.38/dramkit/logtools/utils_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import os
 import logging
+import datetime
 from pandas import isnull
 
 
 # 日志格式
 # formatter = logging.Formatter(
 # '''%(asctime)s -%(filename)s[line: %(lineno)d] -%(levelname)s:
 # --%(message)s''')
@@ -37,14 +38,16 @@
 
 
     .. todo::
         - 添加更多level和设置
     '''
     if isnull(logger):
         print(log_str)
+        print('    [time: {}]'.format(
+        datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')))
     elif logger is False:
         return
     elif isinstance(logger, logging.Logger):
         if level == 'info':
             logger.info(log_str)
         elif level in ['warn', 'warning']:
             logger.warning(log_str)
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/alo.py` & `dramkit-0.5.38/dramkit/optimizer/alo.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     popsize = func_opter_parms.parms_opter['popsize']
     max_iter = func_opter_parms.parms_opter['max_iter']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -214,35 +214,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, l+1) + \
                             'best fval: {}'.format(gBestVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(gBestVal)
     func_opter_parms.set_best_x(gBest)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     # objf = TestFuncs.f5
     # parms_func = {'func_name': objf.__name__,
     #               'x_lb': -10, 'x_ub': 10, 'dim': 5, 'kwargs': {}}
     # parms_opter = {'opter_name': 'alo-test',
     #                 'popsize': 20, 'max_iter': 1000}
     objf = TestFuncs.f12
@@ -264,8 +264,8 @@
 
     # best_x = func_opter_parms.best_x
     # func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.38/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/optimizer/boa.py` & `dramkit-0.5.38/dramkit/optimizer/boa.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     power_exponent = func_opter_parms.parms_opter['power_exponent']
     sensory_modality = func_opter_parms.parms_opter['power_exponent']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -151,35 +151,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, t) + \
                             'best fval: {}'.format(best_y))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(best_y)
     func_opter_parms.set_best_x(best_x)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.f11
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'boa-test',
                    'popsize': 30, 'max_iter': 500,
                    'p': 0.6, 'power_exponent': 0.1, 'sensory_modality': 0.01}
@@ -197,8 +197,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/cs.py` & `dramkit-0.5.38/dramkit/optimizer/cs.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     beta = func_opter_parms.parms_opter['beta']
     alpha = func_opter_parms.parms_opter['alpha']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -191,35 +191,35 @@
                opter_name = func_opter_parms.parms_opter['opter_name']
                func_name = func_opter_parms.parms_func['func_name']
                logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, l+1) + \
                            'best fval: {}'.format(gBestVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(gBestVal)
     func_opter_parms.set_best_x(gBest)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley2
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'cs-test',
                    'popsize': 20, 'max_iter': 1000,
                    'pa': 0.2, 'beta': 1.5, 'alpha': 0.01}
@@ -237,8 +237,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/ga.py` & `dramkit-0.5.38/dramkit/optimizer/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,15 +334,15 @@
     p_mut = func_opter_parms.parms_opter['p_mut']
     n_top = func_opter_parms.parms_opter['n_top']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -389,35 +389,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, l+1) + \
                             'best fval: {}'.format(gBestVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(gBestVal)
     func_opter_parms.set_best_x(gBest)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley2
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'ga-test',
                    'popsize': 20, 'max_iter': 1000,
                    'p_crs': 0.7, 'p_mut': 0.1, 'n_top': 2}
@@ -436,8 +436,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/gwo.py` & `dramkit-0.5.38/dramkit/optimizer/gwo.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     popsize = func_opter_parms.parms_opter['popsize']
     max_iter = func_opter_parms.parms_opter['max_iter']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -186,34 +186,34 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, l+1) + \
                             'best fval: {}'.format(AlphaVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(AlphaVal)
     func_opter_parms.set_best_x(AlphaPos)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley2
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'gwo-test',
                    'popsize': 30, 'max_iter': 500}
     # logger = simple_logger()
@@ -230,8 +230,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.38/dramkit/optimizer/hcpsoboa.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     power_exponent = func_opter_parms.parms_opter['power_exponent']
     sensory_modality = func_opter_parms.parms_opter['power_exponent']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -192,35 +192,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, t) + \
                             'best fval: {}'.format(best_y))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(best_y)
     func_opter_parms.set_best_x(best_x)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley2
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'hcpsoboa-test',
                    'popsize': 30, 'max_iter': 500,
                    'p': 0.6, 'power_exponent': 0.1, 'sensory_modality': 0.01}
@@ -238,8 +238,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/hho.py` & `dramkit-0.5.38/dramkit/optimizer/hho.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     beta = func_opter_parms.parms_opter['beta']
     alpha = func_opter_parms.parms_opter['alpha']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -197,35 +197,35 @@
                opter_name = func_opter_parms.parms_opter['opter_name']
                func_name = func_opter_parms.parms_func['func_name']
                logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, t+1) + \
                            'best fval: {}'.format(gBestVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(gBestVal)
     func_opter_parms.set_best_x(gBest)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     # objf = TestFuncs.f5
     # parms_func = {'func_name': objf.__name__,
     #               'x_lb': -30, 'x_ub': 30, 'dim': 50, 'kwargs': {}}
     # parms_opter = {'opter_name': 'hho-test',
     #                'popsize': 30, 'max_iter': 1000,
     #                'beta': 1.5, 'alpha': 0.01}
@@ -249,8 +249,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.38/dramkit/optimizer/hpsoboa.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     power_exponent = func_opter_parms.parms_opter['power_exponent']
     sensory_modality = func_opter_parms.parms_opter['power_exponent']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -177,35 +177,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, t) + \
                             'best fval: {}'.format(best_y))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(best_y)
     func_opter_parms.set_best_x(best_x)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley2
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'hpsoboa-test',
                    'popsize': 30, 'max_iter': 1000,
                    'p': 0.6, 'power_exponent': 0.1, 'sensory_modality': 0.01}
@@ -223,8 +223,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/pso.py` & `dramkit-0.5.38/dramkit/optimizer/pso.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     c1 = func_opter_parms.parms_opter['c1']
     c2 = func_opter_parms.parms_opter['c2']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -175,35 +175,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, l+1) + \
                             'best fval: {}'.format(gBestVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(gBestVal)
     func_opter_parms.set_best_x(gBest)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'pso-test',
                    'popsize': 30, 'max_iter': 500,
                    'v_maxs': 5, 'w_max': 0.9, 'w_min': 0.2, 'w_fix': False,
@@ -222,8 +222,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.38/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/optimizer/woa.py` & `dramkit-0.5.38/dramkit/optimizer/woa.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     popsize = func_opter_parms.parms_opter['popsize']
     max_iter = func_opter_parms.parms_opter['max_iter']
     # 日志参数
     logger = func_opter_parms.parms_log['logger']
     nshow = func_opter_parms.parms_log['nshow']
 
     # 时间记录
-    strt_tm = time.time()
+    strt_tm = time.monotonic()
     func_opter_parms.set_start_time(time.strftime('%Y-%m-%d %H:%M:%S'))
 
 
     # 边界统一为列表
     if not isinstance(x_lb, list):
         x_lb = [x_lb] * dim
     if not isinstance(x_ub, list):
@@ -148,35 +148,35 @@
                 opter_name = func_opter_parms.parms_opter['opter_name']
                 func_name = func_opter_parms.parms_func['func_name']
                 logger.info('{} for {}, iter: {}, '.format(opter_name, func_name, t+1) + \
                             'best fval: {}'.format(LeaderVal))
 
 
     # 更新func_opter_parms
-    end_tm = time.time()
+    end_tm = time.monotonic()
     func_opter_parms.set_end_time(time.strftime('%Y-%m-%d %H:%M:%S'))
     func_opter_parms.set_exe_time(end_tm-strt_tm)
     func_opter_parms.set_convergence_curve(convergence_curve)
     func_opter_parms.set_convergence_curve_mean(convergence_curve_mean)
     func_opter_parms.set_best_val(LeaderVal)
     func_opter_parms.set_best_x(LeaderPos)
 
     return func_opter_parms
 
 
 if __name__ == '__main__':
     import pandas as pd
     from dramkit.optimizer.base_funcs import TestFuncs
     from dramkit.optimizer.utils_heuristic import FuncOpterInfo
-    from dramkit import plot_series, simple_logger
+    from dramkit import plot_series, simple_logger, TimeRecoder
     from dramkit.logtools.logger_general import get_logger
     from dramkit.logtools.utils_logger import close_log_file
 
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     objf = TestFuncs.ackley2
     parms_func = {'func_name': objf.__name__,
                   'x_lb': -10, 'x_ub': 10, 'dim': 10, 'kwargs': {}}
     parms_opter = {'opter_name': 'woa-test',
                    'popsize': 20, 'max_iter': 1000}
     # logger = simple_logger()
@@ -193,8 +193,8 @@
 
     best_x = func_opter_parms.best_x
     func_opter_parms.parms_log['logger'].info('best x: {}'.format(best_x))
 
     close_log_file(logger)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/other/_Python_notes.py` & `dramkit-0.5.38/dramkit/other/_Python_notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Python笔记
 
+# 参考：
+# pip命令：https://blog.csdn.net/fancunshuai/article/details/124994040
+
 py_notes = \
 r'''
 # conda查看镜像
 conda config --show-sources
 
 # conda设置镜像
 # 首先用命令创建配置文件（或手动创建）.condarc：
@@ -35,14 +38,15 @@
 conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
 
 # pip查看镜像源
 pip config list
 
 # pip安装时带临时镜像
 pip install pkgname -i https://mirror.baidu.com/pypi/simple
+pip install pkgname -i https://pypi.org/simple # PYPI官方镜像
 
 # pip设置镜像
 pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
 
 # 在pip.ini（windows）中设置镜像
 [global]
 index-url = https://pypi.tuna.tsinghua.edu.cn/simple
@@ -74,8 +78,14 @@
 
 # conda虚拟环境安装spyder
 conda install spyder
 
 # conda虚拟环境安装notebook
 conda install nb_conda
 
+# pip安装忽略依赖
+--no-dependencies
+ 
+# pip强制重新安装所有软件包，即使它们已经是最新的
+--force-reinstall
+
 # '''
```

### Comparing `dramkit-0.4.4/dramkit/other/langconv.py` & `dramkit-0.5.38/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/other/othertools.py` & `dramkit-0.5.38/dramkit/other/othertools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/other/replace_endblank.py` & `dramkit-0.5.38/dramkit/other/replace_endblank.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         lines_new.pop()
 
     # 写入新文件
     write_txt(lines_new, fpath_new, encoding=encoding_new)
 
 
 if __name__ == '__main__':
-    import time
-    strt_tm = time.time()
+    from dramkit import TimeRecoder
+    tr = TimeRecoder()
 
     root_dir = './'
     files_types = ['.py_']
     all_files = get_all_paths(root_dir, ext=files_types)
 
     # func_new_path = lambda x: x
     func_new_path = None
     encoding_new = 'utf-8'
     for fpath in all_files:
         replace_endblank_in_file(fpath, func_new_path,
                                  encoding_new=encoding_new)
 
 
-    print('used time: %ss.'%(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/other/zh_wiki.py` & `dramkit-0.5.38/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/plottools/plot_barline.py` & `dramkit-0.5.38/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/plottools/plot_common.py` & `dramkit-0.5.38/dramkit/plottools/plot_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 fills_yparl_up=None, fills_yparl_low=None, fills_xparl={},
                 twinx_align_up=None, twinx_align_low=None,
                 ylabels=None, xlabels=None, grids=False, figsize=(11, 7),
                 title=None, n_xticks=8, xticks_rotation=None,
                 fontsize_label=15, fontsize_title=15, fontsize_text=10,
                 fontsize_legend=15, fontsize_tick=10, fontname=None,
                 markersize=10, legend_locs=None, fig_save_path=None,
-                logger=None):
+                show=True, logger=None):
     '''
     对data (`pd.DataFrame`)进行多列绘图
 
     .. note::
         目前功能未考虑data.index重复情况，若有重复可能会导致部分绘图错误
 
     Parameters
@@ -796,15 +796,18 @@
 
     plt.tight_layout()
 
     # 保存图片
     if fig_save_path:
         plt.savefig(fig_save_path)
 
-    plt.show()
+    if not show:
+        plt.close()
+    else:
+        plt.show()
 
 #%%
 def plot_series_conlabel(data, conlabel_info, del_repeat_lbl=True, **kwargs):
     '''
     在 :func:`dramkit.plottools.plot_common.plot_series` 基础上添加了连续标注绘图功能
 
     Parameters
@@ -944,18 +947,18 @@
     if fig_save_path:
         plt.savefig(fig_save_path)
 
     plt.show()
 
 #%%
 if __name__ == '__main__':
-    import time
     import pandas as pd
-
-    strt_tm = time.time()
+    from dramkit.gentools import TimeRecoder
+    
+    tr = TimeRecoder()
 
     #%%
     col1 = np.random.normal(10, 5, (100, 1))
     col2 = np.random.rand(100, 1)
     col3 = np.random.uniform(0, 20, (100, 1))
     col4 = col1 ** 2
 
@@ -1076,8 +1079,8 @@
                           #         'color': 'c', 'alpha': 0.3}}
                           cols_to_fill_info={
                             'x': {'y2': df3['x1'],
                                   'color': 'c', 'alpha': 0.3}},
                           xticks_rotation=45)
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `dramkit-0.4.4/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.38/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.38/dramkit/plottools/plot_scatter.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,46 @@
 mpl.rcParams['text.usetex'] = False
 mpl.rcParams['mathtext.fontset'] = 'cm' # 'dejavusans', 'cm', 'stix'
 import matplotlib.pyplot as plt
 
 from sklearn.linear_model import LinearRegression as lr
 
 
-def plot_scatter(data, colx, coly, reg_type=None, dotstyl='.k', regstyl='-b',
-                 figsize=(10, 7), title=None, xlabel=None, ylabel=None,
-                 fontsize=15, nXticks=8, fig_save_path=None):
+def plot_scatter(data, colx, coly, reg_type=None, dotstyl='.k',
+                 group_col=None, group_dotstyles={}, regstyl='-b',
+                 figsize=(10, 7), title=None, xlabel=None,
+                 ylabel=None, fontsize=15, nXticks=8,
+                 fig_save_path=None):
     '''
-    散点图绘制
+    | 散点图绘制
+    | group_dotstyles格式: {-1: 'ob', 1: 'or', 0: 'ok'}
     '''
-    df = data.reindex(columns=[colx, coly])
+    cols = [colx, coly]
+    if not group_col is None:
+        cols.append(group_col)
+    df = data[list(set(cols))].copy()
     _, ax = plt.subplots(figsize=figsize)
-    ax.plot(df[colx], df[coly], dotstyl)
+    if group_col is None:
+        ax.plot(df[colx], df[coly], dotstyl)
+    else:
+        for val, dotstyle in group_dotstyles.items():
+            dftmp = df[df[group_col] == val]
+            ax.plot(dftmp[colx], dftmp[coly], dotstyle,
+                    label='%s=%s'%(group_col, val))
     if reg_type in ['lr', 'linear']:
         mdl = lr().fit(df[[colx]], df[coly])
         df['yreg'] = mdl.predict(df[[colx]])
         if mdl.intercept_ > 0:
             lblstr = 'y = {a}x + {b}'.format(
                      a=round(mdl.coef_[0], 4), b=round(mdl.intercept_, 4))
         else:
             lblstr = 'y = {a}x {b}'.format(
                      a=round(mdl.coef_[0], 4), b=round(mdl.intercept_, 4))
         ax.plot(df[colx], df['yreg'], regstyl, label=lblstr)
-        plt.legend(loc=0, fontsize=fontsize)
+    plt.legend(loc=0, fontsize=fontsize)
     if title:
         plt.title(title, fontsize=fontsize)
     xlabel = colx if xlabel is None else xlabel
     ylabel = coly if ylabel is None else ylabel
     plt.xlabel(xlabel, fontsize=fontsize)
     plt.ylabel(ylabel, fontsize=fontsize)
     plt.show()
```

### Comparing `dramkit-0.4.4/dramkit/plottools/utils_plot.py` & `dramkit-0.5.38/dramkit/plottools/utils_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     
     # 对齐作图
     plot_series(df,
                 {'value_net': ('-k', False)},
                 cols_styl_up_right={'pct': ('-b', False)},
                 xparls_info={'value_net': [(1,)], 'pct': [(0,)]},
                 twinx_align_up=[1, 0],
-                ylabels=['净值', '总盈亏率'], title='普通作图')
+                ylabels=['净值', '总盈亏率'], title='对齐作图')
     
     
     # from matplotlib import pyplot as plt
     
     # # 普通作图
     # plt.figure(figsize=(10, 7.5))
     # ax1 = plt.subplot(111)
```

### Comparing `dramkit-0.4.4/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.38/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.38/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.38/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/sorts/insert_sort.py` & `dramkit-0.5.38/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.38/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/sorts/quick_sort.py` & `dramkit-0.5.38/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/speedup/multi_process.py` & `dramkit-0.5.38/dramkit/speedup/multi_process_concurrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import time
-from concurrent.futures import as_completed
-from concurrent.futures import ProcessPoolExecutor
+import platform
+from concurrent.futures import (as_completed,
+                                ProcessPoolExecutor)
+from dramkit.gentools import tmprint, print_used_time
 
+_WINDOWS_SYSTEM = 'windows' in platform.system().lower()
 
+#%%
+@print_used_time
 def multi_process_concurrent(func, args_list,
                              keep_order=True,
                              multi_line=None):
     '''
     多进程，同一个函数执行多次
 
     Parameters
@@ -22,15 +27,15 @@
 
         .. caution:: 
             若keep_order为True，则func的格式应转化为：
 
             | def func(args):
             |     return f(\*args)
     multi_line : int, None
-        最大线程数，默认等于len(args_list)
+        最大进程数，默认等于len(args_list)
 
     Returns
     -------
     results : list
         每个元素对应func以args_list的元素为输入的返回结果
 
     Note
@@ -69,38 +74,40 @@
 
 
 def _func_test_win_new(args):
     return _func_test_win(*args)
 
 #%%
 if __name__ == '__main__':
-    import platform
-
+    from dramkit import TimeRecoder
 
     def func(idx, sleep_tm):
         '''注：若此目标函数定义在__name__ == '__main__'之后，则在windows下会报错'''
         print('task id:', idx)
         time.sleep(sleep_tm)
         print('task id: {}; slept: {}s.'.format(idx, sleep_tm))
         return [idx, sleep_tm]
 
     def func_new(args):
         return func(*args)
 
     args_list = [[1, 2], [3, 4], [4, 5], [2, 3]]
+    args_list = [[1, 20], [3, 40], [4, 50], [2, 30]]
 
 
-    print('multi-process, concurrent............................')
-    strt_tm = time.time()
-    if platform.system() == 'Windows':
+    # '''
+    tmprint('multi-process, concurrent...................')
+    tr = TimeRecoder()
+    if _WINDOWS_SYSTEM:
         results_Order = multi_process_concurrent(_func_test_win_new, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(_func_test_win, args_list,
                                                    keep_order=False)
         results_Order2 = multi_process_concurrent(_func_test_win_new, args_list,
                                                   keep_order=True, multi_line=2)
     else:
         results_Order = multi_process_concurrent(func_new, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(func, args_list,
                                                    keep_order=False)
-    print('total used time: {tm}s.'.format(tm=round(time.time() - strt_tm,6)))
+    tr.used()
+    # '''
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.38/dramkit/sqltools/_Hive_notes.py`

 * *Files 26% similar despite different names*

```diff
@@ -63,9 +63,18 @@
 
 # 关闭hadoop安全模式
 hadoop dfsadmin -safemode leave
 
 # 打开hadoop安全模式
 hadoop dfsadmin -safemode enter
 
+# 报错：
+This command is not allowed on an ACID table xxx.xxx_table  with a non-ACID transaction manager
+解决方案：
+SET hive.support.concurrency=true;
+SET hive.txn.manager=org.apache.hadoop.hive.ql.lockmgr.DbTxnManager;
+
+# 客户端kerberos认证命令（先cd到kerberos目录，windows一般为program Files\MIT\Kerberos\bin）
+# TODO: 命令具体意义
+kinit -kt hive.keytab hive/hadoop-003-250.guoyuanml.com@GUOYUANML.COM
 
 # '''
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.38/dramkit/sqltools/_MySQL_notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,41 @@
 -- 查看安装文件目录
 SHOW VARIABLES LIKE "basedir";
 SELECT @@basedir;
 
 -- （windows）mysql57开启bin log，在配置文件my.ini中[mysqld]下添加内容：log-bin=mysql-bin
 -- （windows）mysql8关闭bin log，在配置文件my.ini中[mysqld]下添加内容：skip-log-bin
 
+-- 2006 MySQL server has gone解决
+show global status like 'uptime'; /*查看mysql的运行时长*/
+show global variables like '%timeout'; /*查看超时设置*/
+set global wait_timeout=3600*48; /*设置连接超时*/
+show global status like 'com_kill'; /*查看连接进程被kill*/
+show global variables like 'max_allowed_packet'; /*查看查询结果大小限制*/
+set global max_allowed_packet=1024*1024*16; /*修改查询结果大小限制*/
+
+-- Ubuntu设置MySql局域网可以访问
+-- 1. 编辑 /etc/mysql/mysql.conf.d/mysqld.cnf
+-- 把里面的bind-address = 127.0.0.1
+-- 改成  # bind-address = 127.0.0.1 进行屏蔽
+-- 2：
+mysql -uroot -ppassword /*登录*/
+use mysql;
+update user set host = '%' where user ='root';
+grant all privileges on *.* to 'root'@'%' with grant option;
+flush privileges;
+exit;
+-- 3. 重启mysql
+sudo /etc/init.d/mysql restart
+
+-- 刚安装没有密码时设置初始密码
+[sudo] mysql /*登入数据库*/
+ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password by 'mynewpassword'; /*登入数据库之后*/
+[sudo] mysql_secure_installation /*退出数据库之后，出现的问题都选n*/
+
 -- 创建新用户
 CREATE USER "username"@"host" IDENTIFIED BY "password";
 CREATE USER "ff"@"localhost" IDENTIFIED BY "xxxxxxxxxxx"; /*创建用户ff，允许本地登录*/
 CREATE USER "ff"@"192.168.0.102" IDENTIFIED BY "xxxxxxxxxxx"; /*创建用户ff，允许指定ip登录*/
 CREATE USER "ff"@"192.168.0.%" IDENTIFIED BY "xxxxxxxxxxx"; /*创建用户ff，允许指定ip范围登录*/
 CREATE USER "ff"@"%" IDENTIFIED BY "xxxxxxxxxxx"; /*创建用户ff，允许任意ip登录*/
 CREATE USER "ff"@"%"; /*创建用户ff，允许任意ip免密登录*/
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.38/dramkit/sqltools/_Oracle_notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 orcl_notes = \
 r'''
 -- 基于OraDB19Home1社区版本
 -- 大写字母为SQL命令，小写字母为对象名称
 -- []中为可选参数
 
--- 登录: sqlplus 输入用户名(sys as sysdb)和密码
+-- 登录: sqlplus 输入用户名(sys as sysdba)和密码
 
 CONN / as sysdba; /*sys连接，出现`SP2-0640: 未连接`错误时用*/
 
 -- 查看数据库版本信息
 SELECT * FROM v$version;
 
 SHOW con_name; /*显示数据库名称*/
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.38/dramkit/sqltools/cxoracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,15 @@
         待存数据
     conn : cx_oracle.connect
         cx_oracle.connect数据库连接对象
     tb_name : str
         存入的表名
     act_type : str
         | 存入方式：
+        |     若为'ignore_tb'，则当表已经存在时不进行任何操作
         |     若为'new'，则新建表（若原表已存在，则会先删除再重建）
         |     若为'insert'，则直接插入
         |     若为'replace'，则将已存在的数据更新，不存在的行和列都新插入
         |     若为'insert_ignore'，则已有的行不更新，不存在的行新插入
         |     若为'insert_newcols'（谨慎使用），则对已存在的列同直接insert（但是遇到已存在的行时不会报错，可能会丢失数据），有新列则插入新列内容
         |     若为'insert_ignore_newcols'，则对已存在的列同直接insert_ignore，有新列则插入新列内容
     cols : None, list
@@ -383,16 +384,19 @@
     ...                     'value': [66, 7, 8, 9],
     ...                     'VALUE2': [10, 11, 12, 13],
     ...                     'VALUE3': ['10a', '11b', 12, '13']})
     >>> df_to_sql(df, conn, tb_name, act_type='new', idcols=idcols)
     >>> df_to_sql(df1, conn, tb_name, act_type='replace', idcols=idcols)
     '''
     
-    assert act_type in ['new', 'insert', 'insert_ignore', 'replace',
+    assert act_type in ['ignore_tb', 'new', 'insert', 'insert_ignore', 'replace',
                         'insert_newcols', 'insert_ignore_newcols']
+    if act_type == 'ignore_tb' and has_table(conn, tb_name):
+        return
+    
     # 待入库字段检查
     cols = check_list_arg(cols, allow_none=True)
     # 字段名称统一处理为大写
     df = df.rename(columns={x: x.upper() for x in df.columns})
     if not isnull(cols):
         cols = [x.upper() for x in cols]
         df = df[cols].copy()
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/py_hive.py` & `dramkit-0.5.38/dramkit/sqltools/py_hive.py`

 * *Files 11% similar despite different names*

```diff
@@ -128,22 +128,32 @@
             return
         if has_ and force:
             self.execute_sql('DROP TABLE %s PURGE'%tb_name, db_name=db_name)
         idcols = check_list_arg(idcols, allow_none=True)
         colstr = '('
         colstr = colstr + ', '.join(cols_info)
         if not isnull(idcols):
-            pkstr = '\nUNIQUE ({}) DISABLE NOVALIDATE'.format(', '.join(idcols))
+            if self.hive_version >= '3.0':
+                pkstr = '\nCONSTRAINT uni_{} UNIQUE ({}) DISABLE NOVALIDATE'.format(tb_name, ', '.join(idcols))
+            else:
+                pkstr = '\nPRIMARY KEY ({}) DISABLE NOVALIDATE'.format(', '.join(idcols))
             colstr = colstr + ',' + pkstr + ')'
         else:
             colstr = colstr + ')'
-        sql = '''CREATE TABLE {} 
-                 {} 
-                 STORED AS ORC TBLPROPERTIES('transactional'='true')
-              '''.format(tb_name, colstr)
+        if not isnull(idcols):
+            sql = '''CREATE TABLE {} 
+                     {} 
+                     CLUSTERED BY ({}) INTO 31 BUCKETS 
+                     STORED AS ORC TBLPROPERTIES('transactional'='true')
+                  '''.format(tb_name, colstr, ', '.join(idcols))
+        else:
+            sql = '''CREATE TABLE {} 
+                     {} 
+                     STORED AS ORC TBLPROPERTIES('transactional'='true')
+                  '''.format(tb_name, colstr)
         self.execute_sql(sql, db_name=db_name)
         
     def merge_into(self, *args, **kwargs):
         if self.hive_version >= '2.2':
             return self.merge_into1(*args, **kwargs)
             # try:
             #     return self.merge_into1(*args, **kwargs)
@@ -178,14 +188,16 @@
         
     def merge_into2(self, tb_tgt, tb_src, replace_cols, idcols,
                     rep_keep='src', db_name=None):
         assert rep_keep in ['src', 'tgt']
         assert isinstance(replace_cols, list) and isinstance(idcols, list)
         if rep_keep == 'tgt':
             tb_tgt_, tb_src_ = tb_src, tb_tgt
+        else:
+            tb_tgt_, tb_src_ = tb_tgt, tb_src
         idcols = [x.lower() for x in idcols]
         replace_cols = [x.lower() for x in replace_cols]
         on_ = ' AND '.join(['t.%s=s.%s'%(c, c) for c in idcols])
         t_cols = self.get_fields(tb_tgt, db_name=db_name)[0]
         t_cols = [x.lower() for x in t_cols]
         select_ = []
         for col in t_cols:
@@ -196,15 +208,27 @@
         select_ = ', \n'.join(select_)
         sql = '''INSERT OVERWRITE TABLE {f1} 
                  SELECT {f4} 
                  FROM {f2} s 
                  FULL OUTER JOIN {f5} t 
                  ON {f3} 
               '''.format(f1=tb_tgt, f2=tb_src_, f3=on_, f4=select_, f5=tb_tgt_)
+
+        self.execute_sql('SET hive.auto.convert.join=false')
+        self.execute_sql('SET hive.stats.autogather=false')
+		# self.execute_sql(sql, db_name=db_name)
+        sql = '''INSERT INTO TABLE {f1} 
+                 SELECT {f4} 
+                 FROM {f2} s 
+                 FULL OUTER JOIN {f5} t 
+                 ON {f3} 
+              '''.format(f1=tb_tgt, f2=tb_src_, f3=on_, f4=select_, f5=tb_tgt_)
+        self.execute_sql('TRUNCATE TABLE {}'.format(tb_tgt))
         self.execute_sql(sql, db_name=db_name)
+
     
     @print_used_time
     def df_to_sql(self, df, tb_name, act_type='replace',
                   db_name=None, cols=None, idcols=None,
                   col_types={}, na_val=None, 
                   inf_val='inf', _inf_val='-inf',
                   **kwargs_cols):
@@ -236,16 +260,19 @@
         ...                     'value': [66, 7, 8, 9],
         ...                     'VALUE2': [10, 11, 12, 13],
         ...                     'VALUE3': ['10a', '11b', 12, '13']})
         >>> db.df_to_sql(df, tb_name, act_type='new', idcols=idcols)
         >>> db.df_to_sql(df1, tb_name, act_type='insert_ignore_newcols', idcols=idcols)
         '''
         
-        assert act_type in ['new', 'insert', 'insert_ignore',
+        assert act_type in ['ignore_tb', 'new', 'insert', 'insert_ignore',
                             'replace', 'insert_ignore_newcols']
+        if act_type == 'ignore_tb' and self.has_table(tb_name, db_name=db_name):
+            return
+        
         # 待入库字段检查
         cols = check_list_arg(cols, allow_none=True)
         # 字段名称统一处理为大写
         df = df.rename(columns={x: x.upper() for x in df.columns})
         if not isnull(cols):
             cols = [x.upper() for x in cols]
             df = df[cols].copy()
@@ -300,27 +327,45 @@
         
         # 数据更新
         # values = df.values.tolist()
         # TODO: pyhive用cur_.executemany报错，原因待查
         # impala用cur_.executemany很慢
         values_str = df_to_sql_insert_values(df, cols=cols)
         if act_type == 'new' or isnull(idcols):
-            # cur_.executemany('INSERT INTO {a} ({b}) VALUES ({c})'.format(
-            #                  a=tb_name, b=','.join(cols), c=ph),
-            #                  values)
-            cur_.execute('INSERT INTO {a} ({b}) VALUES {c}'.format(
-                         a=tb_name, b=','.join(cols), c=values_str))
-        elif act_type == 'insert':
-            # 批量插入新数据
-            try:
+            # TODO: 低版本不能全字段插入，待确定从哪个版本开始
+            # TODO: 解决低版本不能全字段插入式只更新部分字段的问题
+            if self.hive_version >= '3.0':
                 # cur_.executemany('INSERT INTO {a} ({b}) VALUES ({c})'.format(
                 #                  a=tb_name, b=','.join(cols), c=ph),
                 #                  values)
                 cur_.execute('INSERT INTO {a} ({b}) VALUES {c}'.format(
-                              a=tb_name, b=','.join(cols), c=values_str))
+                             a=tb_name, b=','.join(cols), c=values_str))
+            else:
+                # 解决报错：This command is not allowed on an ACID table xxx.xxx_table  with a non-ACID transaction manager
+                cur_.execute('SET hive.support.concurrency=true')
+                cur_.execute('SET hive.txn.manager=org.apache.hadoop.hive.ql.lockmgr.DbTxnManager')
+                cur_.execute('INSERT INTO {a} VALUES {c}'.format(
+                             a=tb_name, c=values_str))
+        elif act_type == 'insert':
+            # 批量插入新数据
+            try:
+                # TODO: 低版本不能全字段插入，待确定从哪个版本开始
+                # TODO: 解决低版本不能全字段插入式只更新部分字段的问题
+                if self.hive_version >= '3.0':
+                    # cur_.executemany('INSERT INTO {a} ({b}) VALUES ({c})'.format(
+                    #                  a=tb_name, b=','.join(cols), c=ph),
+                    #                  values)
+                    cur_.execute('INSERT INTO {a} ({b}) VALUES {c}'.format(
+                                  a=tb_name, b=','.join(cols), c=values_str))
+                else:
+                    # 解决报错：This command is not allowed on an ACID table xxx.xxx_table  with a non-ACID transaction manager
+                    cur_.execute('SET hive.support.concurrency=true')
+                    cur_.execute('SET hive.txn.manager=org.apache.hadoop.hive.ql.lockmgr.DbTxnManager')
+                    cur_.execute('INSERT INTO {a} VALUES {c}'.format(
+                                 a=tb_name, c=values_str))
             except:
                 self.drop_cols(tb_name, cols_loss, db_name=db_name)
                 raise
         else:
             tb_name_tmp = self._get_tmp_tb_name(tb_name+'_TMP')
             df_tmp = df.reindex(columns=fields_)
             self.df_to_sql(df_tmp, tb_name_tmp, act_type='new',
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.38/dramkit/sqltools/py_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         res = copy(self)
         conn_args = self.__db_conn_args.copy()
         conn_args.update({'client_flag': CLIENT.MULTI_STATEMENTS})
         res.conn = get_conn(**conn_args)
         return res
     
     def has_table(self, tb_name, db_name=None):
-        tbs = self.show_tables(db_name=None)
+        tbs = self.show_tables(db_name=db_name)
         return tb_name.lower() in [x.lower() for x in tbs]
         
         
 def _check_list_arg(arg, allow_none=True):
     if allow_none:
         assert isinstance(arg, (type(None), str, list, tuple))
     else:
@@ -288,14 +288,19 @@
         cols = [x[0] for x in cur.description]
         res = pd.DataFrame(res, columns=cols)
     cur.close()
     conn.commit()
     return res
 
 
+def has_table(conn, tb_name, db_name=None):
+    tbs = show_tables(conn, db_name=db_name)
+    return tb_name.lower() in [x.lower() for x in tbs]
+
+
 def get_fields(conn, tb_name, db_name=None):
     '''获取表字段名列表'''
     sql_str = 'DESC {};'.format(tb_name)
     fields_info = execute_sql(conn, sql_str,
                               db_name=db_name, to_df=True)
     fields = fields_info['Field'].tolist()
     return fields, fields_info
@@ -761,15 +766,15 @@
             raise ValueError('未识别（暂不支持）的字段类型: %s！'%col)
         char_ = '%s'
         cols_info.append(char)
         placeholder.append(char_)
         cols_info_dict[col] = (char, char_)
     cols_info, placeholder = ', '.join(cols_info), ', '.join(placeholder)
     dtype = {k: v[0].split(' ')[-1] for k, v in cols_info_dict.items()}
-    
+
     return cols_info, dtype, placeholder, cols_info_dict
 
 
 def df_to_sql_insert_values(df, cols=None):
     '''
     df转化为mysql插入的VALUES格式
     
@@ -817,14 +822,15 @@
         待存数据
     conn : pymysql.connect
         pymysql.connect数据库连接对象
     tb_name : str
         存入的表名
     act_type : str
         | 存入方式：
+        |     若为'ignore_tb'，则当表已经存在时不进行任何操作
         |     若为'new'，则新建表（若原表已存在，则会先删除再重建）
         |     若为'insert'，则直接插入
         |     若为'replace'，则将已存在的数据更新，不存在的行和列都新插入
         |     若为'insert_ignore'，则已有的行不更新，不存在的行新插入
         |     若为'insert_newcols'（谨慎使用），则对已存在的列同直接insert（但是遇到已存在的行时不会报错，可能会丢失数据），有新列则插入新列内容
         |     若为'insert_ignore_newcols'，则对已存在的列同直接insert_ignore，有新列则插入新列内容
     cols : None, list
@@ -915,17 +921,19 @@
     -----------
     - https://blog.csdn.net/qq_43279637/article/details/92797641
     - https://blog.csdn.net/tonydz0523/article/details/82529941
     - https://blog.csdn.net/weixin_44848356/article/details/119113174
     - https://blog.csdn.net/weixin_42272869/article/details/116480732
     '''
     
-    assert act_type in ['new', 'insert', 'replace',
+    assert act_type in ['ignore_tb', 'new', 'insert', 'replace',
                         'insert_ignore', 'insert_newcols',
                         'insert_ignore_newcols']
+    if act_type == 'ignore_tb' and has_table(conn, tb_name, db_name=db_name):
+        return
     
     idcols = _check_list_arg(idcols)
     if isnull(idcols):
         act_type = 'insert' if act_type != 'new' else 'new'
     
     # 清除原数据或直接新增数据
     if act_type in ['new', 'insert', 'insert_ignore']:
@@ -1060,15 +1068,18 @@
     Note
     ----
     判断数据是否存在时是根据主键或唯一索引来的，
     因此当待插入数据字段只是已存在数据字段的一部分时，
     此函数应慎用'replace'（可能导致原有数据变成Null）
     '''
     
-    assert act_type in ['new', 'insert', 'replace', 'insert_ignore']
+    assert act_type in ['ignore_tb', 'new', 'insert', 'replace', 'insert_ignore']
+    if act_type == 'ignore_tb' and has_table(conn, tb_name, db_name=db_name):
+        return
+    
     # 待入库字段检查
     cols = _check_list_arg(cols)
     # 字段名称统一处理为大写
     df = df.rename(columns={x: x.upper() for x in df.columns})
     if not isnull(cols):
         cols = [x.upper() for x in cols]
         df = df[cols].copy()
```

### Comparing `dramkit-0.4.4/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.38/dramkit/sqltools/sql_alchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import warnings
 from copy import copy
 import pandas as pd
 from sqlalchemy import text, create_engine
 from sqlalchemy.orm import Session
 from sqlalchemy.types import NVARCHAR, DATE, FLOAT, INT, CLOB
-from dramkit.gentools import isnull, change_dict_key
+from dramkit.gentools import (isnull,
+                              change_dict_key,
+                              get_update_kwargs)
 
 
 class SQLAlchemy(object):
     
     def __init__(self,
                  dialect='mysql',
                  driver='pymysql',
@@ -43,14 +45,17 @@
                              **kwargs)
         self.db_name = database
         self.execute_sql = self._execute_sql if not orcl_pdb else self._execute_sql_orm
         
     def df_to_sql(self, *args, **kwargs):
         if self.dbtype == 'oracle':
             return self.df_to_oracle(*args, **kwargs)
+        elif self.dbtype == 'mysql':
+            # from dramkit.sqltools.py_mysql import df_to_sql
+            raise NotImplementedError
         
     def _execute_sql(self, sql_str, to_df=True):
         with self.conn.connect() as conn:
             try:
                 res = conn.execute(text(sql_str))
             except:
                 # warnings.filterwarnings('ignore')
@@ -197,16 +202,19 @@
         ...                     'VALUE2': [10, 11, 12, 13],
         ...                     # 'VALUE3': ['10a', '11b', '12', '13']
         ...                    })
         >>> db.df_to_sql(df, tb_name, act_type='new', idcols=idcols)
         >>> db.df_to_sql(df1, tb_name, act_type='replace', idcols=idcols)
         '''
         df = df.rename(columns={x: x.upper() for x in df.columns})
-        assert act_type in ['new', 'insert', 'insert_ignore',
+        assert act_type in ['ignore_tb', 'new', 'insert', 'insert_ignore',
                             'replace', 'insert_ignore_newcols']
+        if act_type == 'ignore_tb' and self.has_table(tb_name):
+            return
+        
         if not act_type in ['new', 'insert']:
             assert not isnull(idcols)
         _, dtype, _, cols_info_dict = get_cols_info_df_oracle(df,
               col_types=change_dict_key(col_types, lambda x: x.upper()),
               **kwargs_cols)
         tbs, _ = self.get_tables()
         tb_not_exists = not tb_name.upper() in [x.upper() for x in tbs]
@@ -225,18 +233,20 @@
             fields = [x.upper() for x in fields]
             # 缺失字段新增
             cols_loss = [x for x in cols if x not in fields]
             for col in cols_loss:
                 self.execute_sql('ALTER TABLE {} ADD {}'.format(
                                  tb_name, cols_info_dict[col][0]))
             if act_type == 'insert':
-                df.to_sql(tb_name.lower(), self.conn,
-                          if_exists='append', index=None,
-                          dtype=dtype)
-                self.drop_table(tb_name_tmp, purge=True)
+                try:
+                    df.to_sql(tb_name.lower(), self.conn,
+                              if_exists='append', index=None,
+                              dtype=dtype)
+                finally:
+                    self.drop_table(tb_name_tmp, purge=True)
                 return
             idcols = [x.upper() for x in idcols]
             if act_type == 'replace':
                 # 有则更新，无则插入
                 self.oracle_merge_into(tb_name, tb_name_tmp,
                                        cols, idcols,
                                        rep_keep='src')
@@ -262,14 +272,22 @@
             self.drop_table(tb_name_tmp, purge=True)
     
     
 def get_conn(dialect='mysql', driver='pymysql', username='root',
              password=None, host='localhost', port=3306,
              database=None, orcl_pdb=False,
              **kwargs):
+    '''
+    TODO: oracle连接参数有service_name的处理？
+    '''
+    if dialect.lower() == 'sqlite':
+        assert 'dbfile' in kwargs, '必须通过kwargs指定sqlite数据库文件路径'
+        file, kwargs_ = get_update_kwargs('dbfile', None, kwargs, func_update=False)
+        engine_str = 'sqlite:///{}'.format(file)
+        return create_engine(engine_str, **kwargs_)
     if isnull(driver):
         part1 = '{}://'.format(dialect)
     else:
         part1 = '{}+{}://'.format(dialect, driver)
     part2 = '{}:{}@'.format(username, password)
     if not orcl_pdb:
         if dialect == 'oracle':
```

### Comparing `dramkit-0.4.4/dramkit/webtools/utils_html.py` & `dramkit-0.5.38/dramkit/webtools/utils_html.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit/wechat/qywechat.py` & `dramkit-0.5.38/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.4.4/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.38/dramkit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.4.4
+Version: 0.5.38
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
@@ -34,9 +34,7 @@
 
 Pypi
 
 [dramkit](https://pypi.org/project/dramkit/)
 
 感谢使用和支持！
 
-
-
```

### Comparing `dramkit-0.4.4/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.38/dramkit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 setup.py
 dramkit/__init__.py
 dramkit/_pkg_info.py
+dramkit/cryptotools.py
 dramkit/datetimetools.py
 dramkit/gentools.py
 dramkit/install_check.py
 dramkit/iotools.py
 dramkit.egg-info/PKG-INFO
 dramkit.egg-info/SOURCES.txt
 dramkit.egg-info/dependency_links.txt
+dramkit.egg-info/requires.txt
 dramkit.egg-info/top_level.txt
 dramkit/_tmp/CRR.py
 dramkit/_tmp/CtrlPreTS.py
 dramkit/_tmp/NPairSum.py
 dramkit/_tmp/PIDtest.py
 dramkit/_tmp/PIDtest2.py
 dramkit/_tmp/VMD.py
@@ -26,28 +28,29 @@
 dramkit/_tmp/mouse_move.py
 dramkit/_tmp/mpc_test1.py
 dramkit/_tmp/options_Implied_volatility.py
 dramkit/_tmp/pf_test.py
 dramkit/_tmp/plot_test.py
 dramkit/_tmp/plot_test2.py
 dramkit/_tmp/simple_smooth.py
-dramkit/_tmp/test_AES.py
-dramkit/_tmp/test_AES_CBC.py
-dramkit/_tmp/test_AES_ECB.py
-dramkit/_tmp/test_AES_ECB2.py
+dramkit/_tmp/test_async_washs.py
+dramkit/_tmp/test_await_timeout.py
 dramkit/_tmp/test_backtrader.py
+dramkit/_tmp/test_chatgpt_v1.py
 dramkit/_tmp/test_code.py
 dramkit/_tmp/test_find_peaks.py
 dramkit/_tmp/test_get_var_name.py
 dramkit/_tmp/test_grading.py
 dramkit/_tmp/test_lr.py
 dramkit/_tmp/test_maxsort.py
+dramkit/_tmp/test_multiprocessing.py
 dramkit/_tmp/test_ocr.py
 dramkit/_tmp/test_pywechat.py
 dramkit/_tmp/test_tree.py
+dramkit/_tmp/test_tree2.py
 dramkit/_tmp/test_wechat_work.py
 dramkit/_tmp/tfDNNCls_test.py
 dramkit/_tmp/tmp.py
 dramkit/_tmp/tmp_args.py
 dramkit/_tmp/transformer_pytorch.py
 dramkit/_tmp/utils_SignalDec.py
 dramkit/_tmp/utils_TimeSeries.py
@@ -99,14 +102,18 @@
 dramkit/find_addends/find_addends_smlfirst.py
 dramkit/find_addends/find_addends_utils.py
 dramkit/logtools/__init__.py
 dramkit/logtools/logger_general.py
 dramkit/logtools/logger_rotating.py
 dramkit/logtools/logger_timedrotating.py
 dramkit/logtools/utils_logger.py
+dramkit/openai/__init__.py
+dramkit/openai/aiedu_chat.py
+dramkit/openai/openai_chat.py
+dramkit/openai/openai_chat_hs.py
 dramkit/optimizer/__init__.py
 dramkit/optimizer/alo.py
 dramkit/optimizer/base_funcs.py
 dramkit/optimizer/boa.py
 dramkit/optimizer/cs.py
 dramkit/optimizer/ga.py
 dramkit/optimizer/gwo.py
@@ -135,15 +142,19 @@
 dramkit/sorts/__init__.py
 dramkit/sorts/bubble_sort.py
 dramkit/sorts/bucket_sort.py
 dramkit/sorts/insert_sort.py
 dramkit/sorts/insert_sort_bin.py
 dramkit/sorts/quick_sort.py
 dramkit/speedup/__init__.py
-dramkit/speedup/multi_process.py
+dramkit/speedup/_mp_test1.py
+dramkit/speedup/_mp_test2.py
+dramkit/speedup/_mp_test3.py
+dramkit/speedup/iotools_tmp.py
+dramkit/speedup/multi_process_concurrent.py
 dramkit/speedup/multi_thread.py
 dramkit/sqltools/_Hive_notes.py
 dramkit/sqltools/_MySQL_notes.py
 dramkit/sqltools/_Oracle_notes.py
 dramkit/sqltools/__init__.py
 dramkit/sqltools/cxoracle.py
 dramkit/sqltools/py_hive.py
```

### Comparing `dramkit-0.4.4/setup.py` & `dramkit-0.5.38/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,25 +28,32 @@
       url=pkg_info['__url__'],
       license=pkg_info['__license__'],
       description=pkg_info['__description__'],
       # long_description=pkg_info['__long_description__'],
       long_description=readme,
       long_description_content_type='text/markdown',
       platforms='any',
+      setup_requires=[],
+      install_requires=['pycryptodome',
+                        'cryptography',
+                        'tqdm',
+                        'pymysql',
+                        'openai'],
       packages=['dramkit',
+                'dramkit.backpacks',
                 'dramkit.chncal',
+                'dramkit.datsci',
+                'dramkit.find_addends',                
                 'dramkit.logtools',
+                'dramkit.openai',
+                'dramkit.optimizer',
+                'dramkit.other',
                 'dramkit.plottools',
-                'dramkit.datsci',
+                'dramkit.pystyles',                
                 'dramkit.sorts',
+                'dramkit.speedup',
 				'dramkit.sqltools',
-				'dramkit.speedup',
-				'dramkit.optimizer',
-				'dramkit.webtools',
+                'dramkit.webtools',
                 'dramkit.wechat',
-				'dramkit.find_addends',
-				'dramkit.backpacks',
-				'dramkit.pystyles',
-                'dramkit.other',
                 'dramkit._tmp'
                 ]
       )
```

