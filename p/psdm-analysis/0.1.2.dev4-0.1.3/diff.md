# Comparing `tmp/psdm-analysis-0.1.2.dev4.tar.gz` & `tmp/psdm-analysis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdm-analysis-0.1.2.dev4.tar", max compression
+gzip compressed data, was "psdm-analysis-0.1.3.tar", max compression
```

## Comparing `psdm-analysis-0.1.2.dev4.tar` & `psdm-analysis-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,67 @@
--rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.2.dev4/LICENSE
--rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.2.dev4/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.2.dev4/psdm_analysis/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/__init__.py
--rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/calc.py
--rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/grid.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.2.dev4/psdm_analysis/io/__init__.py
--rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.2.dev4/psdm_analysis/io/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.2.dev4/psdm_analysis/models/__init__.py
--rw-r--r--   0        0        0     7232 2023-04-19 12:49:15.039262 psdm-analysis-0.1.2.dev4/psdm_analysis/models/entity.py
--rw-r--r--   0        0        0     5988 2023-04-19 12:49:15.039392 psdm-analysis-0.1.2.dev4/psdm_analysis/models/grid_with_results.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/__init__.py
--rw-r--r--   0        0        0     2126 2023-04-19 12:49:15.039712 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/lines.py
--rw-r--r--   0        0        0      578 2023-04-19 12:49:15.039922 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/switches.py
--rw-r--r--   0        0        0     2455 2023-04-19 12:49:15.040033 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/transformer.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/__init__.py
--rw-r--r--   0        0        0     3925 2023-04-19 12:49:15.040286 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/grid_container.py
--rw-r--r--   0        0        0     3456 2023-04-19 12:49:15.040383 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/mixins.py
--rw-r--r--   0        0        0     6113 2023-04-19 12:49:15.040661 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/participants_container.py
--rw-r--r--   0        0        0     1884 2023-04-19 12:49:15.040834 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/enums.py
--rw-r--r--   0        0        0     1129 2023-04-19 12:49:15.041071 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/node.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/bm.py
--rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/charging.py
--rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/em.py
--rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evcs.py
--rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evs.py
--rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/fixed_feed_in.py
--rw-r--r--   0        0        0      814 2023-04-19 12:49:15.042128 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/hp.py
--rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/load.py
--rw-r--r--   0        0        0     1032 2023-04-19 12:49:15.042559 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/participant.py
--rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/pv.py
--rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/storage.py
--rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/wec.py
--rw-r--r--   0        0        0     2887 2023-04-19 12:49:15.043116 psdm-analysis-0.1.2.dev4/psdm_analysis/models/primary_data.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/flex_option.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/__init__.py
--rw-r--r--   0        0        0     2314 2023-04-19 12:49:15.043655 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/enhanced_node.py
--rw-r--r--   0        0        0     3670 2023-04-19 12:49:15.043790 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/node.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/__init__.py
--rw-r--r--   0        0        0     3645 2023-04-19 12:49:15.043937 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/dict.py
--rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/flex_options.py
--rw-r--r--   0        0        0     6261 2023-04-19 12:49:15.044315 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participant.py
--rw-r--r--   0        0        0     9664 2023-04-19 12:49:15.044458 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participants_res_container.py
--rw-r--r--   0        0        0     5776 2023-04-19 12:49:15.044578 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/power.py
--rw-r--r--   0        0        0     2340 2023-04-19 12:49:15.044687 psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/res_container.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/__init__.py
--rw-r--r--   0        0        0     1349 2023-04-19 12:49:15.044823 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/grid.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/__init__.py
--rw-r--r--   0        0        0     2431 2023-04-19 12:49:15.045086 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/bar_plot.py
--rw-r--r--   0        0        0     3461 2023-04-19 12:49:15.045391 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/flex_plot.py
--rw-r--r--   0        0        0     1096 2023-04-19 12:49:15.045589 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/line_plot.py
--rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/nodes.py
--rw-r--r--   0        0        0    11954 2023-04-19 12:49:15.045955 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/power_plot.py
--rw-r--r--   0        0        0     4096 2023-04-19 12:49:15.046076 psdm-analysis-0.1.2.dev4/psdm_analysis/plots/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.2.dev4/psdm_analysis/processing/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-19 12:49:15.046231 psdm-analysis-0.1.2.dev4/psdm_analysis/processing/dataframe.py
--rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.2.dev4/psdm_analysis/processing/series.py
--rw-r--r--   0        0        0      668 2023-04-19 12:50:52.147307 psdm-analysis-0.1.2.dev4/pyproject.toml
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 psdm-analysis-0.1.2.dev4/setup.py
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 psdm-analysis-0.1.2.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.3/LICENSE
+-rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.3/psdm_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.3/psdm_analysis/analysis/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.3/psdm_analysis/analysis/calc.py
+-rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.3/psdm_analysis/analysis/grid.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:49:33.826962 psdm-analysis-0.1.3/psdm_analysis/conversion/__init__.py
+-rw-r--r--   0        0        0   254685 2023-04-28 08:32:26.669910 psdm-analysis-0.1.3/psdm_analysis/conversion/pandapower.ipynb
+-rw-r--r--   0        0        0     3960 2023-04-28 08:49:33.827267 psdm-analysis-0.1.3/psdm_analysis/conversion/pandapower.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.3/psdm_analysis/io/__init__.py
+-rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.3/psdm_analysis/io/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.3/psdm_analysis/models/__init__.py
+-rw-r--r--   0        0        0     7232 2023-04-19 12:49:15.039262 psdm-analysis-0.1.3/psdm_analysis/models/entity.py
+-rw-r--r--   0        0        0     5988 2023-04-19 12:49:15.039392 psdm-analysis-0.1.3/psdm_analysis/models/grid_with_results.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.3/psdm_analysis/models/input/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/__init__.py
+-rw-r--r--   0        0        0     2126 2023-04-19 12:49:15.039712 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/lines.py
+-rw-r--r--   0        0        0      578 2023-04-19 12:49:15.039922 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/switches.py
+-rw-r--r--   0        0        0     2455 2023-04-19 12:49:15.040033 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.3/psdm_analysis/models/input/container/__init__.py
+-rw-r--r--   0        0        0     3925 2023-04-19 12:49:15.040286 psdm-analysis-0.1.3/psdm_analysis/models/input/container/grid_container.py
+-rw-r--r--   0        0        0     3456 2023-04-19 12:49:15.040383 psdm-analysis-0.1.3/psdm_analysis/models/input/container/mixins.py
+-rw-r--r--   0        0        0     6113 2023-04-19 12:49:15.040661 psdm-analysis-0.1.3/psdm_analysis/models/input/container/participants_container.py
+-rw-r--r--   0        0        0     1884 2023-04-19 12:49:15.040834 psdm-analysis-0.1.3/psdm_analysis/models/input/enums.py
+-rw-r--r--   0        0        0     1129 2023-04-19 12:49:15.041071 psdm-analysis-0.1.3/psdm_analysis/models/input/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/__init__.py
+-rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/bm.py
+-rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/charging.py
+-rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/em.py
+-rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evcs.py
+-rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evs.py
+-rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/fixed_feed_in.py
+-rw-r--r--   0        0        0      814 2023-04-19 12:49:15.042128 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/hp.py
+-rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/load.py
+-rw-r--r--   0        0        0     1032 2023-04-19 12:49:15.042559 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/participant.py
+-rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/pv.py
+-rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/storage.py
+-rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/wec.py
+-rw-r--r--   0        0        0     2887 2023-04-19 12:49:15.043116 psdm-analysis-0.1.3/psdm_analysis/models/primary_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.3/psdm_analysis/models/result/__init__.py
+-rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.3/psdm_analysis/models/result/flex_option.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.3/psdm_analysis/models/result/grid/__init__.py
+-rw-r--r--   0        0        0     2314 2023-04-19 12:49:15.043655 psdm-analysis-0.1.3/psdm_analysis/models/result/grid/enhanced_node.py
+-rw-r--r--   0        0        0     3670 2023-04-19 12:49:15.043790 psdm-analysis-0.1.3/psdm_analysis/models/result/grid/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/__init__.py
+-rw-r--r--   0        0        0     3645 2023-04-19 12:49:15.043937 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/dict.py
+-rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/flex_options.py
+-rw-r--r--   0        0        0     6261 2023-04-19 12:49:15.044315 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participant.py
+-rw-r--r--   0        0        0     9664 2023-04-19 12:49:15.044458 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participants_res_container.py
+-rw-r--r--   0        0        0     5776 2023-04-19 12:49:15.044578 psdm-analysis-0.1.3/psdm_analysis/models/result/power.py
+-rw-r--r--   0        0        0     2340 2023-04-19 12:49:15.044687 psdm-analysis-0.1.3/psdm_analysis/models/result/res_container.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.3/psdm_analysis/plots/__init__.py
+-rw-r--r--   0        0        0     1349 2023-04-20 07:54:56.450726 psdm-analysis-0.1.3/psdm_analysis/plots/grid.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.3/psdm_analysis/plots/results/__init__.py
+-rw-r--r--   0        0        0     2431 2023-04-19 12:49:15.045086 psdm-analysis-0.1.3/psdm_analysis/plots/results/bar_plot.py
+-rw-r--r--   0        0        0     3461 2023-04-19 12:49:15.045391 psdm-analysis-0.1.3/psdm_analysis/plots/results/flex_plot.py
+-rw-r--r--   0        0        0     1096 2023-04-19 12:49:15.045589 psdm-analysis-0.1.3/psdm_analysis/plots/results/line_plot.py
+-rw-r--r--   0        0        0     2644 2023-04-28 08:49:33.827702 psdm-analysis-0.1.3/psdm_analysis/plots/results/node_plot.py
+-rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.3/psdm_analysis/plots/results/nodes.py
+-rw-r--r--   0        0        0    11954 2023-04-19 12:49:15.045955 psdm-analysis-0.1.3/psdm_analysis/plots/results/power_plot.py
+-rw-r--r--   0        0        0     4318 2023-04-28 09:03:18.431942 psdm-analysis-0.1.3/psdm_analysis/plots/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.3/psdm_analysis/processing/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-19 12:49:15.046231 psdm-analysis-0.1.3/psdm_analysis/processing/dataframe.py
+-rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.3/psdm_analysis/processing/series.py
+-rw-r--r--   0        0        0      683 2023-04-28 09:04:17.744077 psdm-analysis-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 psdm-analysis-0.1.3/setup.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 psdm-analysis-0.1.3/PKG-INFO
```

### Comparing `psdm-analysis-0.1.2.dev4/LICENSE` & `psdm-analysis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/calc.py` & `psdm-analysis-0.1.3/psdm_analysis/analysis/calc.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/analysis/grid.py` & `psdm-analysis-0.1.3/psdm_analysis/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/io/utils.py` & `psdm-analysis-0.1.3/psdm_analysis/io/utils.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/entity.py` & `psdm-analysis-0.1.3/psdm_analysis/models/entity.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/grid_with_results.py` & `psdm-analysis-0.1.3/psdm_analysis/models/grid_with_results.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/lines.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/connector/lines.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/switches.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/connector/switches.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/connector/transformer.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/connector/transformer.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/grid_container.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/container/grid_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/mixins.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/container/mixins.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/container/participants_container.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/container/participants_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/enums.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/enums.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/node.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/bm.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/bm.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/charging.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/charging.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/em.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/em.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evcs.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evcs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/evs.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/fixed_feed_in.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/fixed_feed_in.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/hp.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/hp.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/load.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/load.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/participant.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/pv.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/pv.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/storage.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/storage.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/input/participant/wec.py` & `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/wec.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/primary_data.py` & `psdm-analysis-0.1.3/psdm_analysis/models/primary_data.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/flex_option.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/flex_option.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/enhanced_node.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/grid/enhanced_node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/grid/node.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/grid/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/dict.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/dict.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/flex_options.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/flex_options.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participant.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/participant/participants_res_container.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participants_res_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/power.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/power.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/models/result/res_container.py` & `psdm-analysis-0.1.3/psdm_analysis/models/result/res_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/grid.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/bar_plot.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/results/bar_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/flex_plot.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/results/flex_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/line_plot.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/results/line_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/nodes.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/results/nodes.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/results/power_plot.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/results/power_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/plots/utils.py` & `psdm-analysis-0.1.3/psdm_analysis/plots/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 import os.path
-from typing import Dict
+from typing import Dict, NewType, Tuple
 
 import seaborn as sns
 from matplotlib import dates as mdates
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from pandas import Series
 
-from psdm_analysis.models.input.enums import EntitiesEnum, SystemParticipantsEnum
+from psdm_analysis.models.input.enums import (
+    EntitiesEnum,
+    RawGridElementsEnum,
+    SystemParticipantsEnum,
+)
 from psdm_analysis.processing.series import hourly_mean_resample
 
 # === COLORS ===
 
 COLOR_PALETTE = sns.color_palette()
+
 BLUE = COLOR_PALETTE[0]
 ORANGE = COLOR_PALETTE[1]
 GREEN = COLOR_PALETTE[2]
 RED = COLOR_PALETTE[3]
 PURPLE = COLOR_PALETTE[4]
 BROWN = COLOR_PALETTE[5]
 PINK = COLOR_PALETTE[6]
 GREY = COLOR_PALETTE[7]
 YELLOW = COLOR_PALETTE[8]
 LIGHT_BLUE = COLOR_PALETTE[9]
 
-COLOR_PALETTE = sns.color_palette()
+# === COLOR MATCHING ===
+
+NODE_COLOR = BLUE
 LOAD_COLOR = BLUE
 PV_COLOR = GREEN
 BS_COLOR = ORANGE
 HP_COLOR = PURPLE
 EVCS_COLOR = YELLOW
 RESIDUAL_LOAD_COLOR = LIGHT_BLUE
 UNKNOWN_COLOR = GREY
 FLEX_MAX = BLUE
 FLEX_MIN = GREEN
 FLEX_REF = YELLOW
 
+RGB = NewType("RGB", Tuple[float, float, float])
+
 
 def set_style(style: str = "whitegrid", context: str = "notebook"):
     sns.set_style(style)
     sns.set_context(context)
 
 
-def get_label_and_color(sp_type: EntitiesEnum):
-    if sp_type == SystemParticipantsEnum.LOAD:
-        return "Load", LOAD_COLOR
-    elif sp_type == SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT:
-        return "PV", PV_COLOR
-    elif sp_type == SystemParticipantsEnum.STORAGE:
-        return "Battery", BS_COLOR
-    elif sp_type == SystemParticipantsEnum.EV_CHARGING_STATION:
-        return "EV Charging Station", EVCS_COLOR
-    elif sp_type == SystemParticipantsEnum.ELECTRIC_VEHICLE:
-        return "Electric Vehicle", EVCS_COLOR
-    elif sp_type == SystemParticipantsEnum.HEATP_PUMP:
-        return "Heat Pump", HP_COLOR
-    elif sp_type == SystemParticipantsEnum.ENERGY_MANAGEMENT:
-        return "Energy Management", LOAD_COLOR
-    elif sp_type == SystemParticipantsEnum.PARTICIPANTS_SUM:
-        return "Participants Sum", LOAD_COLOR
-    else:
-        return sp_type, UNKNOWN_COLOR
+def get_label_and_color(sp_type: EntitiesEnum) -> Tuple[str, RGB]:
+    match sp_type:
+        case RawGridElementsEnum.NODE:
+            return "Node", NODE_COLOR
+        case SystemParticipantsEnum.LOAD:
+            return "Load", LOAD_COLOR
+        case SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT:
+            return "PV", PV_COLOR
+        case SystemParticipantsEnum.STORAGE:
+            return "Battery", BS_COLOR
+        case SystemParticipantsEnum.EV_CHARGING_STATION:
+            return "EV Charging Station", EVCS_COLOR
+        case SystemParticipantsEnum.ELECTRIC_VEHICLE:
+            return "Electric Vehicle", EVCS_COLOR
+        case SystemParticipantsEnum.HEATP_PUMP:
+            return "Heat Pump", HP_COLOR
+        case SystemParticipantsEnum.ENERGY_MANAGEMENT:
+            return "Energy Management", LOAD_COLOR
+        case SystemParticipantsEnum.PARTICIPANTS_SUM:
+            return "Participants Sum", LOAD_COLOR
+        case _:
+            return sp_type.value, UNKNOWN_COLOR
 
 
 def get_label_and_color_dict(sp_type: EntitiesEnum):
     label, color = get_label_and_color(sp_type)
     return {"label": label, "color": color}
```

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/processing/dataframe.py` & `psdm-analysis-0.1.3/psdm_analysis/processing/dataframe.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/psdm_analysis/processing/series.py` & `psdm-analysis-0.1.3/psdm_analysis/processing/series.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.2.dev4/pyproject.toml` & `psdm-analysis-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "psdm-analysis"
-version = "0.1.2.dev4"
+version = "0.1.3"
 description = ""
 authors = ["Thomas Oberliessen <thomas.oberliessen@googlemail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.10, <3.12"
-pandas = "2.0.0"
+pandas = "2.0.1"
 jupyter = "^1.0.0"
 matplotlib = "^3.6.0"
 seaborn = "^0.12.1"
 plotly = "^5.6.0"
 requests = "^2.27.1"
 numpy = "^1.24.1"
 scipy = "^1.10.0"
 pyarrow = "^11.0.0"
+openpyxl = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^6.0.0"
 flake8-black = "^0.3.6"
 flake8-isort = "^6.0.0"
 pre-commit = "^2.21.0"
```

### Comparing `psdm-analysis-0.1.2.dev4/setup.py` & `psdm-analysis-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['psdm_analysis',
  'psdm_analysis.analysis',
+ 'psdm_analysis.conversion',
  'psdm_analysis.io',
  'psdm_analysis.models',
  'psdm_analysis.models.input',
  'psdm_analysis.models.input.connector',
  'psdm_analysis.models.input.container',
  'psdm_analysis.models.input.participant',
  'psdm_analysis.models.result',
@@ -20,24 +21,25 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jupyter>=1.0.0,<2.0.0',
  'matplotlib>=3.6.0,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
- 'pandas==2.0.0',
+ 'openpyxl>=3.1.2,<4.0.0',
+ 'pandas==2.0.1',
  'plotly>=5.6.0,<6.0.0',
  'pyarrow>=11.0.0,<12.0.0',
  'requests>=2.27.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0',
  'seaborn>=0.12.1,<0.13.0']
 
 setup_kwargs = {
     'name': 'psdm-analysis',
-    'version': '0.1.2.dev4',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# psdm-analysis\n\nThe psdm-analysis tool is meant to parse the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel) as well as provide calculation and plotting utilities to analyze the respective data.\n\nIt is currently under development and therefore highly unstable. So if you want to use it, expect it to change quite frequently for now.',
     'author': 'Thomas Oberliessen',
     'author_email': 'thomas.oberliessen@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psdm-analysis-0.1.2.dev4/PKG-INFO` & `psdm-analysis-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: psdm-analysis
-Version: 0.1.2.dev4
+Version: 0.1.3
 Summary: 
 Author: Thomas Oberliessen
 Author-email: thomas.oberliessen@googlemail.com
 Requires-Python: >3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: pandas (==2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pandas (==2.0.1)
 Requires-Dist: plotly (>=5.6.0,<6.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.1,<0.13.0)
 Description-Content-Type: text/markdown
```

