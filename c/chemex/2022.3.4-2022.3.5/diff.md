# Comparing `tmp/chemex-2022.3.4.tar.gz` & `tmp/chemex-2022.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemex-2022.3.4.tar", max compression
+gzip compressed data, was "chemex-2022.3.5.tar", max compression
```

## Comparing `chemex-2022.3.4.tar` & `chemex-2022.3.5.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34916 2023-04-19 20:10:31.302739 chemex-2022.3.4/LICENSE.md
--rw-r--r--   0        0        0     1046 2023-04-19 20:10:31.302739 chemex-2022.3.4/README.md
--rw-r--r--   0        0        0      326 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/__init__.py
--rw-r--r--   0        0        0      185 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/__main__.py
--rw-r--r--   0        0        0     2583 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/chemex.py
--rw-r--r--   0        0        0     5876 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/cli.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/__init__.py
--rw-r--r--   0        0        0      447 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/base.py
--rw-r--r--   0        0        0     4619 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/conditions.py
--rw-r--r--   0        0        0     1491 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/data.py
--rw-r--r--   0        0        0     1418 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/experiment.py
--rw-r--r--   0        0        0     4588 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/methods.py
--rw-r--r--   0        0        0     1971 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/configuration/parameters.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/__init__.py
--rw-r--r--   0        0        0     3158 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/data.py
--rw-r--r--   0        0        0     1497 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/dataset.py
--rw-r--r--   0        0        0     5406 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/experiment.py
--rw-r--r--   0        0        0     4238 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/experiments.py
--rw-r--r--   0        0        0     3840 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/containers/profile.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/__init__.py
--rw-r--r--   0        0        0     4379 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/builder.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/__init__.py
--rw-r--r--   0        0        0     3678 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_13c.py
--rw-r--r--   0        0        0     3588 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_15n.py
--rw-r--r--   0        0        0     4060 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_15n_cw.py
--rw-r--r--   0        0        0     4353 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_15n_tr.py
--rw-r--r--   0        0        0     3682 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ap.py
--rw-r--r--   0        0        0     4771 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4084 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
--rw-r--r--   0        0        0     5188 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/coscest_13c.py
--rw-r--r--   0        0        0     5472 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/coscest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4782 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_13c_ip.py
--rw-r--r--   0        0        0     5174 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_13co_ap.py
--rw-r--r--   0        0        0     4864 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip.py
--rw-r--r--   0        0        0     5702 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip_0013.py
--rw-r--r--   0        0        0     5456 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr.py
--rw-r--r--   0        0        0     7561 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr_0013.py
--rw-r--r--   0        0        0     5192 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap.py
--rw-r--r--   0        0        0     7764 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
--rw-r--r--   0        0        0     5016 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
--rw-r--r--   0        0        0     5869 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
--rw-r--r--   0        0        0     6696 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
--rw-r--r--   0        0        0     5871 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
--rw-r--r--   0        0        0     7400 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
--rw-r--r--   0        0        0     4292 2023-04-19 20:10:31.302739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_mq.py
--rw-r--r--   0        0        0     4916 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
--rw-r--r--   0        0        0     5290 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/cpmg_hn_dq_zq.py
--rw-r--r--   0        0        0     4412 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/dcest_13c.py
--rw-r--r--   0        0        0     4643 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/dcest_15n.py
--rw-r--r--   0        0        0     3330 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/relaxation_hznz.py
--rw-r--r--   0        0        0     2991 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/relaxation_nz.py
--rw-r--r--   0        0        0     2921 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sq.py
--rw-r--r--   0        0        0     3283 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sqmq.py
--rw-r--r--   0        0        0     3235 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/factories.py
--rw-r--r--   0        0        0      970 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/experiments/loader.py
--rw-r--r--   0        0        0     2671 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/filterers.py
--rw-r--r--   0        0        0     7125 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/messages.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/__init__.py
--rw-r--r--   0        0        0     2753 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/constraints.py
--rw-r--r--   0        0        0     1071 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/factory.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/__init__.py
--rw-r--r--   0        0        0      575 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_1st.py
--rw-r--r--   0        0        0     1241 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st.py
--rw-r--r--   0        0        0     2954 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a2.py
--rw-r--r--   0        0        0     2958 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a3.py
--rw-r--r--   0        0        0     2966 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a4.py
--rw-r--r--   0        0        0     2722 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_binding.py
--rw-r--r--   0        0        0     2878 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_eyring.py
--rw-r--r--   0        0        0     1985 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_hd.py
--rw-r--r--   0        0        0     1278 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_2st_rs.py
--rw-r--r--   0        0        0     4590 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a3.py
--rw-r--r--   0        0        0     4298 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a4.py
--rw-r--r--   0        0        0     5043 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_double_binding.py
--rw-r--r--   0        0        0     4463 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_eyring.py
--rw-r--r--   0        0        0     4079 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_3st_induced_fit.py
--rw-r--r--   0        0        0     3994 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_4st_hd.py
--rw-r--r--   0        0        0     4768 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/kinetic/settings_nst.py
--rw-r--r--   0        0        0      945 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/loader.py
--rw-r--r--   0        0        0     1384 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/models/model.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/__init__.py
--rw-r--r--   0        0        0    10952 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/basis.py
--rw-r--r--   0        0        0     6309 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/constants.py
--rw-r--r--   0        0        0     9538 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/liouvillian.py
--rw-r--r--   0        0        0     8795 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/rates.py
--rw-r--r--   0        0        0    13135 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/nmr/spectrometer.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/__init__.py
--rw-r--r--   0        0        0     5309 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/fitting.py
--rw-r--r--   0        0        0     8679 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/gridding.py
--rw-r--r--   0        0        0     2946 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/grouping.py
--rw-r--r--   0        0        0     5459 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/helper.py
--rw-r--r--   0        0        0     2763 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/optimize/minimizer.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/__init__.py
--rw-r--r--   0        0        0    12804 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/database.py
--rw-r--r--   0        0        0     3236 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/factory.py
--rw-r--r--   0        0        0     4659 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/name.py
--rw-r--r--   0        0        0     3937 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/setting.py
--rw-r--r--   0        0        0    12623 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/spin_system.py
--rw-r--r--   0        0        0     9618 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/spins.py
--rw-r--r--   0        0        0      901 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/parameters/userfunctions.py
--rw-r--r--   0        0        0      316 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/__init__.py
--rw-r--r--   0        0        0     7907 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/cest.py
--rw-r--r--   0        0        0     6634 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/cpmg.py
--rw-r--r--   0        0        0     2376 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/plot.py
--rw-r--r--   0        0        0      329 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/plotter.py
--rw-r--r--   0        0        0     3706 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/relaxation.py
--rw-r--r--   0        0        0     1674 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/plotters/shift.py
--rw-r--r--   0        0        0        0 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/__init__.py
--rw-r--r--   0        0        0     1785 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/data.py
--rw-r--r--   0        0        0     4510 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/parameters.py
--rw-r--r--   0        0        0     2679 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/printers/plot.py
--rw-r--r--   0        0        0     2929 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/toml.py
--rw-r--r--   0        0        0       98 2023-04-19 20:10:31.306739 chemex-2022.3.4/chemex/tools/__init__.py
--rw-r--r--   0        0        0     9332 2023-04-19 20:10:31.310739 chemex-2022.3.4/chemex/tools/pick_cest.py
--rw-r--r--   0        0        0     1819 2023-04-19 20:10:31.310739 chemex-2022.3.4/chemex/tools/plot_param.py
--rw-r--r--   0        0        0     2667 2023-04-19 20:10:31.310739 chemex-2022.3.4/chemex/uncertainty.py
--rw-r--r--   0        0        0     1056 2023-04-19 20:10:31.542741 chemex-2022.3.4/pyproject.toml
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 chemex-2022.3.4/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-04-28 11:59:29.349853 chemex-2022.3.5/LICENSE.md
+-rw-r--r--   0        0        0     1046 2023-04-28 11:59:29.349853 chemex-2022.3.5/README.md
+-rw-r--r--   0        0        0      326 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/__main__.py
+-rw-r--r--   0        0        0     2583 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/chemex.py
+-rw-r--r--   0        0        0     5876 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/cli.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/base.py
+-rw-r--r--   0        0        0     4619 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/conditions.py
+-rw-r--r--   0        0        0     1491 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/data.py
+-rw-r--r--   0        0        0     1418 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/experiment.py
+-rw-r--r--   0        0        0     4588 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/methods.py
+-rw-r--r--   0        0        0     1971 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/configuration/parameters.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/containers/__init__.py
+-rw-r--r--   0        0        0     3158 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/containers/data.py
+-rw-r--r--   0        0        0     1497 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/containers/dataset.py
+-rw-r--r--   0        0        0     5406 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/containers/experiment.py
+-rw-r--r--   0        0        0     4238 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/containers/experiments.py
+-rw-r--r--   0        0        0     3840 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/containers/profile.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/builder.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/__init__.py
+-rw-r--r--   0        0        0     3678 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_13c.py
+-rw-r--r--   0        0        0     3588 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_15n.py
+-rw-r--r--   0        0        0     4060 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_15n_cw.py
+-rw-r--r--   0        0        0     4353 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_15n_tr.py
+-rw-r--r--   0        0        0     3682 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_1hn_ap.py
+-rw-r--r--   0        0        0     4771 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4084 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
+-rw-r--r--   0        0        0     5188 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/coscest_13c.py
+-rw-r--r--   0        0        0     5472 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/coscest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4782 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_13c_ip.py
+-rw-r--r--   0        0        0     5174 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_13co_ap.py
+-rw-r--r--   0        0        0     4864 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_ip.py
+-rw-r--r--   0        0        0     5702 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_ip_0013.py
+-rw-r--r--   0        0        0     5456 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_tr.py
+-rw-r--r--   0        0        0     7561 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_tr_0013.py
+-rw-r--r--   0        0        0     5192 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_1hn_ap.py
+-rw-r--r--   0        0        0     7764 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
+-rw-r--r--   0        0        0     5016 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
+-rw-r--r--   0        0        0     5869 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
+-rw-r--r--   0        0        0     6696 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
+-rw-r--r--   0        0        0     5871 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
+-rw-r--r--   0        0        0     7400 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
+-rw-r--r--   0        0        0     4292 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_mq.py
+-rw-r--r--   0        0        0     4916 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
+-rw-r--r--   0        0        0     5290 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/cpmg_hn_dq_zq.py
+-rw-r--r--   0        0        0     4412 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/dcest_13c.py
+-rw-r--r--   0        0        0     4643 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/dcest_15n.py
+-rw-r--r--   0        0        0     3330 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/relaxation_hznz.py
+-rw-r--r--   0        0        0     2991 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/relaxation_nz.py
+-rw-r--r--   0        0        0     2921 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/shift_15n_sq.py
+-rw-r--r--   0        0        0     3283 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/catalog/shift_15n_sqmq.py
+-rw-r--r--   0        0        0     3235 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/factories.py
+-rw-r--r--   0        0        0      970 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/experiments/loader.py
+-rw-r--r--   0        0        0     2671 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/filterers.py
+-rw-r--r--   0        0        0     7125 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/messages.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/__init__.py
+-rw-r--r--   0        0        0     2753 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/constraints.py
+-rw-r--r--   0        0        0     1071 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/factory.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_1st.py
+-rw-r--r--   0        0        0     1241 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st.py
+-rw-r--r--   0        0        0     2954 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_a_a2.py
+-rw-r--r--   0        0        0     2958 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_a_a3.py
+-rw-r--r--   0        0        0     2966 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_a_a4.py
+-rw-r--r--   0        0        0     2722 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_binding.py
+-rw-r--r--   0        0        0     2878 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_eyring.py
+-rw-r--r--   0        0        0     1985 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_hd.py
+-rw-r--r--   0        0        0     1278 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_2st_rs.py
+-rw-r--r--   0        0        0     4590 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_3st_a_a2_a3.py
+-rw-r--r--   0        0        0     4298 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_3st_a_a2_a4.py
+-rw-r--r--   0        0        0     5043 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_3st_double_binding.py
+-rw-r--r--   0        0        0     4497 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_3st_eyring.py
+-rw-r--r--   0        0        0     4079 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_3st_induced_fit.py
+-rw-r--r--   0        0        0     3994 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_4st_hd.py
+-rw-r--r--   0        0        0     4768 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/kinetic/settings_nst.py
+-rw-r--r--   0        0        0      945 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/loader.py
+-rw-r--r--   0        0        0     1384 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/models/model.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/nmr/__init__.py
+-rw-r--r--   0        0        0    10952 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/nmr/basis.py
+-rw-r--r--   0        0        0     6309 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/nmr/constants.py
+-rw-r--r--   0        0        0     9538 2023-04-28 11:59:29.349853 chemex-2022.3.5/chemex/nmr/liouvillian.py
+-rw-r--r--   0        0        0     8795 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/nmr/rates.py
+-rw-r--r--   0        0        0    13135 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/nmr/spectrometer.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/optimize/__init__.py
+-rw-r--r--   0        0        0     5309 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/optimize/fitting.py
+-rw-r--r--   0        0        0     8679 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/optimize/gridding.py
+-rw-r--r--   0        0        0     2946 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/optimize/grouping.py
+-rw-r--r--   0        0        0     5459 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/optimize/helper.py
+-rw-r--r--   0        0        0     2763 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/optimize/minimizer.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/__init__.py
+-rw-r--r--   0        0        0    12804 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/database.py
+-rw-r--r--   0        0        0     3234 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/factory.py
+-rw-r--r--   0        0        0     4659 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/name.py
+-rw-r--r--   0        0        0     3937 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/setting.py
+-rw-r--r--   0        0        0    12623 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/spin_system.py
+-rw-r--r--   0        0        0     9618 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/spins.py
+-rw-r--r--   0        0        0      901 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/parameters/userfunctions.py
+-rw-r--r--   0        0        0      316 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/cest.py
+-rw-r--r--   0        0        0     6634 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/cpmg.py
+-rw-r--r--   0        0        0     2376 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/plot.py
+-rw-r--r--   0        0        0      329 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/plotter.py
+-rw-r--r--   0        0        0     3706 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/relaxation.py
+-rw-r--r--   0        0        0     1674 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/plotters/shift.py
+-rw-r--r--   0        0        0        0 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/printers/__init__.py
+-rw-r--r--   0        0        0     1785 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/printers/data.py
+-rw-r--r--   0        0        0     4510 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/printers/parameters.py
+-rw-r--r--   0        0        0     2679 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/printers/plot.py
+-rw-r--r--   0        0        0     2929 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/toml.py
+-rw-r--r--   0        0        0       98 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/tools/__init__.py
+-rw-r--r--   0        0        0     9332 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/tools/pick_cest.py
+-rw-r--r--   0        0        0     1819 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/tools/plot_param.py
+-rw-r--r--   0        0        0     2667 2023-04-28 11:59:29.353853 chemex-2022.3.5/chemex/uncertainty.py
+-rw-r--r--   0        0        0     1056 2023-04-28 11:59:29.545855 chemex-2022.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 chemex-2022.3.5/PKG-INFO
```

### Comparing `chemex-2022.3.4/LICENSE.md` & `chemex-2022.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/README.md` & `chemex-2022.3.5/README.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/chemex.py` & `chemex-2022.3.5/chemex/chemex.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/cli.py` & `chemex-2022.3.5/chemex/cli.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/configuration/conditions.py` & `chemex-2022.3.5/chemex/configuration/conditions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/configuration/data.py` & `chemex-2022.3.5/chemex/configuration/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/configuration/experiment.py` & `chemex-2022.3.5/chemex/configuration/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/configuration/methods.py` & `chemex-2022.3.5/chemex/configuration/methods.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/configuration/parameters.py` & `chemex-2022.3.5/chemex/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/containers/data.py` & `chemex-2022.3.5/chemex/containers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/containers/dataset.py` & `chemex-2022.3.5/chemex/containers/dataset.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/containers/experiment.py` & `chemex-2022.3.5/chemex/containers/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/containers/experiments.py` & `chemex-2022.3.5/chemex/containers/experiments.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/containers/profile.py` & `chemex-2022.3.5/chemex/containers/profile.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/builder.py` & `chemex-2022.3.5/chemex/experiments/builder.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_13c.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_15n.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_15n_cw.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_15n_cw.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_15n_tr.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_1hn_ip_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/coscest_13c.py` & `chemex-2022.3.5/chemex/experiments/catalog/coscest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/coscest_1hn_ip_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/coscest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_13c_ip.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_13c_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_13co_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_13co_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_ip_0013.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_ip_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_15n_tr_0013.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_15n_tr_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_1hn_ap_0013.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_1hn_ap_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_dq.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_dq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_sq.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_tq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_ch3_mq.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_ch3_mq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_chd2_1h_ap.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_chd2_1h_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/cpmg_hn_dq_zq.py` & `chemex-2022.3.5/chemex/experiments/catalog/cpmg_hn_dq_zq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/dcest_13c.py` & `chemex-2022.3.5/chemex/experiments/catalog/dcest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/dcest_15n.py` & `chemex-2022.3.5/chemex/experiments/catalog/dcest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/relaxation_hznz.py` & `chemex-2022.3.5/chemex/experiments/catalog/relaxation_hznz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/relaxation_nz.py` & `chemex-2022.3.5/chemex/experiments/catalog/relaxation_nz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sq.py` & `chemex-2022.3.5/chemex/experiments/catalog/shift_15n_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/catalog/shift_15n_sqmq.py` & `chemex-2022.3.5/chemex/experiments/catalog/shift_15n_sqmq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/factories.py` & `chemex-2022.3.5/chemex/experiments/factories.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/experiments/loader.py` & `chemex-2022.3.5/chemex/experiments/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/filterers.py` & `chemex-2022.3.5/chemex/filterers.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/messages.py` & `chemex-2022.3.5/chemex/messages.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/constraints.py` & `chemex-2022.3.5/chemex/models/constraints.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/factory.py` & `chemex-2022.3.5/chemex/models/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_1st.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_1st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a2.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_a_a2.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a3.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_a_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_a_a4.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_a_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_binding.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_eyring.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_hd.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_2st_rs.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_2st_rs.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a3.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_3st_a_a2_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_3st_a_a2_a4.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_3st_a_a2_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_3st_double_binding.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_3st_double_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_3st_eyring.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_3st_eyring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import lru_cache
-from itertools import combinations
+from itertools import permutations
 from typing import TYPE_CHECKING
 
 import numpy as np
 from scipy.constants import constants
 
 from chemex.models.constraints import pop_3st
 from chemex.models.factory import model_factory
@@ -39,45 +39,45 @@
     kelvin = temperature + 273.15
     kbt_h = constants.k * kelvin / constants.h
     rt = constants.R * kelvin
     dh_a = ds_a = 0.0
     ddg_ij = np.array(
         (
             dh_ab - dh_a - kelvin * (ds_ab - ds_a),
-            dh_ab - dh_b - kelvin * (ds_ab - ds_b),
             dh_ac - dh_a - kelvin * (ds_ac - ds_a),
-            dh_ac - dh_c - kelvin * (ds_ac - ds_c),
+            dh_ab - dh_b - kelvin * (ds_ab - ds_b),
             dh_bc - dh_b - kelvin * (ds_bc - ds_b),
+            dh_ac - dh_c - kelvin * (ds_ac - ds_c),
             dh_bc - dh_c - kelvin * (ds_bc - ds_c),
         )
     )
     kij_values = kbt_h * np.exp(-ddg_ij / rt)
-    kij_names = (f"k{i}{j}" for i, j in combinations("abc", 2))
+    kij_names = (f"k{i}{j}" for i, j in permutations("abc", 2))
     return dict(zip(kij_names, kij_values))
 
 
 def create_kij_3st_eyring_settings(temperature: float) -> dict[str, ParamLocalSetting]:
     return {
-        f"{i}{j}": ParamLocalSetting(
+        f"k{i}{j}": ParamLocalSetting(
             name_setting=NameSetting(f"k{i}{j}", "", TPL),
             expr=(
                 f"calculate_kij_3st_eyring({{dh_b}}, {{ds_b}}, {{dh_c}}, {{ds_c}}, "
                 f"{{dh_ab}}, {{ds_ab}}, {{dh_ac}}, {{ds_ac}}, {{dh_bc}}, {{ds_bc}},"
                 f" {temperature})['k{i}{j}']"
             ),
         )
-        for i, j in combinations("abc", 2)
+        for i, j in permutations("abc", 2)
     }
 
 
 def create_pop_3st_eyring_settings() -> dict[str, ParamLocalSetting]:
     return {
         f"p{state}": ParamLocalSetting(
             name_setting=NameSetting(f"p{state}", "", TPL),
-            expr=f"pop_2st({{kab}}, {{kba}}, {{kac}}, {{kca}}, {{kbc}}, {{kcb}})['p{state}']",
+            expr=f"pop_3st({{kab}}, {{kba}}, {{kac}}, {{kca}}, {{kbc}}, {{kcb}})['p{state}']",
         )
         for state in "abc"
     }
 
 
 def make_settings_3st_eyring(conditions: Conditions) -> dict[str, ParamLocalSetting]:
     celsius = conditions.temperature
@@ -137,9 +137,12 @@
         **create_kij_3st_eyring_settings(celsius),
         **create_pop_3st_eyring_settings(),
     }
 
 
 def register() -> None:
     model_factory.register(name=NAME, setting_maker=make_settings_3st_eyring)
-    user_functions = {"kij_2st_eyring": calculate_kij_3st_eyring, "pop_3st": pop_3st}
+    user_functions = {
+        "calculate_kij_3st_eyring": calculate_kij_3st_eyring,
+        "pop_3st": pop_3st,
+    }
     user_function_registry.register(name=NAME, user_functions=user_functions)
```

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_3st_induced_fit.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_3st_induced_fit.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_4st_hd.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_4st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/kinetic/settings_nst.py` & `chemex-2022.3.5/chemex/models/kinetic/settings_nst.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/loader.py` & `chemex-2022.3.5/chemex/models/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/models/model.py` & `chemex-2022.3.5/chemex/models/model.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/nmr/basis.py` & `chemex-2022.3.5/chemex/nmr/basis.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/nmr/constants.py` & `chemex-2022.3.5/chemex/nmr/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/nmr/liouvillian.py` & `chemex-2022.3.5/chemex/nmr/liouvillian.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/nmr/rates.py` & `chemex-2022.3.5/chemex/nmr/rates.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/nmr/spectrometer.py` & `chemex-2022.3.5/chemex/nmr/spectrometer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/optimize/fitting.py` & `chemex-2022.3.5/chemex/optimize/fitting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/optimize/gridding.py` & `chemex-2022.3.5/chemex/optimize/gridding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/optimize/grouping.py` & `chemex-2022.3.5/chemex/optimize/grouping.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/optimize/helper.py` & `chemex-2022.3.5/chemex/optimize/helper.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/optimize/minimizer.py` & `chemex-2022.3.5/chemex/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/parameters/database.py` & `chemex-2022.3.5/chemex/parameters/database.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/parameters/factory.py` & `chemex-2022.3.5/chemex/parameters/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
             parameters[param_id].expr = ""
         pool -= selection
 
 
 def _build_parameters(
     settings: LocalSettings, spin_system: SpinSystem, conditions: Conditions
 ) -> tuple[dict[str, str], Parameters]:
-
     param_names = {
         local_name: setting.name_setting.get_param_name(spin_system, conditions)
         for local_name, setting in settings.items()
     }
 
     name_map = {
         local_name: param_name.id for local_name, param_name in param_names.items()
@@ -67,15 +66,14 @@
 
     return name_map, parameters
 
 
 def create_parameters(
     config: ExperimentConfig, liouvillian: LiouvillianIS
 ) -> dict[str, str]:
-
     # A copy is done because the output of '_build_settings' is cached
     settings, settings_mf = _build_settings(liouvillian.basis, config.conditions)
 
     name_map, parameters = _build_parameters(
         settings, liouvillian.spin_system, config.conditions
     )
```

### Comparing `chemex-2022.3.4/chemex/parameters/name.py` & `chemex-2022.3.5/chemex/parameters/name.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/parameters/setting.py` & `chemex-2022.3.5/chemex/parameters/setting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/parameters/spin_system.py` & `chemex-2022.3.5/chemex/parameters/spin_system.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/parameters/spins.py` & `chemex-2022.3.5/chemex/parameters/spins.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/parameters/userfunctions.py` & `chemex-2022.3.5/chemex/parameters/userfunctions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/plotters/cest.py` & `chemex-2022.3.5/chemex/plotters/cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/plotters/cpmg.py` & `chemex-2022.3.5/chemex/plotters/cpmg.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/plotters/plot.py` & `chemex-2022.3.5/chemex/plotters/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/plotters/relaxation.py` & `chemex-2022.3.5/chemex/plotters/relaxation.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/plotters/shift.py` & `chemex-2022.3.5/chemex/plotters/shift.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/printers/data.py` & `chemex-2022.3.5/chemex/printers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/printers/parameters.py` & `chemex-2022.3.5/chemex/printers/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/printers/plot.py` & `chemex-2022.3.5/chemex/printers/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/toml.py` & `chemex-2022.3.5/chemex/toml.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/tools/pick_cest.py` & `chemex-2022.3.5/chemex/tools/pick_cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/tools/plot_param.py` & `chemex-2022.3.5/chemex/tools/plot_param.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/chemex/uncertainty.py` & `chemex-2022.3.5/chemex/uncertainty.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.4/pyproject.toml` & `chemex-2022.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chemex"
-version = "2022.3.4"
+version = "2022.3.5"
 description = "ChemEx is an analysis program for chemical exchange detected by NMR"
 authors = ["Guillaume Bouvignies <gbouvignies@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/gbouvignies/chemex"
 homepage = "http://gbouvignies.github.io/ChemEx/"
 classifiers = [
```

### Comparing `chemex-2022.3.4/PKG-INFO` & `chemex-2022.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemex
-Version: 2022.3.4
+Version: 2022.3.5
 Summary: ChemEx is an analysis program for chemical exchange detected by NMR
 Home-page: http://gbouvignies.github.io/ChemEx/
 License: GPL-3.0-only
 Author: Guillaume Bouvignies
 Author-email: gbouvignies@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Science/Research
```

