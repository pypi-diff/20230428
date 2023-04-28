# Comparing `tmp/rootmd-0.5.5.tar.gz` & `tmp/rootmd-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootmd-0.5.5.tar", max compression
+gzip compressed data, was "rootmd-0.5.6.tar", max compression
```

## Comparing `rootmd-0.5.5.tar` & `rootmd-0.5.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1075 2022-01-14 16:47:08.057953 rootmd-0.5.5/LICENSE
--rw-r--r--   0        0        0      645 2022-03-03 14:58:52.702820 rootmd-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3503 2022-02-06 01:13:31.898156 rootmd-0.5.5/rootmd/Executor.py
--rw-r--r--   0        0        0     4796 2022-02-11 15:30:34.463201 rootmd-0.5.5/rootmd/Md2MacroRenderer.py
--rw-r--r--   0        0        0     2866 2022-02-08 19:39:13.044715 rootmd-0.5.5/rootmd/RootBaseRenderer.py
--rw-r--r--   0        0        0    20986 2022-02-11 15:27:31.131687 rootmd-0.5.5/rootmd/RootHtmlRenderer.py
--rw-r--r--   0        0        0     4049 2022-01-20 16:23:16.125406 rootmd-0.5.5/rootmd/RootMdRenderer.py
--rw-r--r--   0        0        0     6549 2022-01-29 17:07:49.742045 rootmd-0.5.5/rootmd/YamlBlock.py
--rw-r--r--   0        0        0      531 2022-01-24 19:32:45.122648 rootmd-0.5.5/rootmd/__init__.py
--rwxr-xr-x   0        0        0     8597 2022-03-03 14:57:23.774617 rootmd-0.5.5/rootmd/__main__.py
--rw-r--r--   0        0        0     1130 2022-02-02 15:12:30.704568 rootmd-0.5.5/rootmd/data/css/core.css
--rw-r--r--   0        0        0     2438 2022-01-25 18:04:44.971728 rootmd-0.5.5/rootmd/data/css/prismjs/prism-a11y-dark.css
--rw-r--r--   0        0        0     1945 2022-01-25 18:04:44.972020 rootmd-0.5.5/rootmd/data/css/prismjs/prism-atom-dark.css
--rw-r--r--   0        0        0     3332 2022-01-25 18:04:44.972274 rootmd-0.5.5/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css
--rw-r--r--   0        0        0     2618 2022-01-25 18:04:44.972624 rootmd-0.5.5/rootmd/data/css/prismjs/prism-cb.css
--rw-r--r--   0        0        0     6782 2022-01-25 18:04:44.972916 rootmd-0.5.5/rootmd/data/css/prismjs/prism-coldark-cold.css
--rw-r--r--   0        0        0     6776 2022-01-25 18:04:44.973160 rootmd-0.5.5/rootmd/data/css/prismjs/prism-coldark-dark.css
--rw-r--r--   0        0        0     2306 2022-01-25 18:04:44.973423 rootmd-0.5.5/rootmd/data/css/prismjs/prism-coy-without-shadows.css
--rw-r--r--   0        0        0     4031 2022-01-26 17:26:54.465267 rootmd-0.5.5/rootmd/data/css/prismjs/prism-coy.css
--rw-r--r--   0        0        0     3062 2022-01-26 17:26:54.465715 rootmd-0.5.5/rootmd/data/css/prismjs/prism-coy.min.css
--rw-r--r--   0        0        0     2680 2022-01-25 18:04:44.973675 rootmd-0.5.5/rootmd/data/css/prismjs/prism-darcula.css
--rw-r--r--   0        0        0     2070 2022-01-26 17:26:54.465978 rootmd-0.5.5/rootmd/data/css/prismjs/prism-dark.css
--rw-r--r--   0        0        0     1533 2022-01-26 17:26:54.466270 rootmd-0.5.5/rootmd/data/css/prismjs/prism-dark.min.css
--rw-r--r--   0        0        0     1795 2022-01-25 18:04:44.973874 rootmd-0.5.5/rootmd/data/css/prismjs/prism-dracula.css
--rw-r--r--   0        0        0     3389 2022-01-25 18:04:44.974121 rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-dark.css
--rw-r--r--   0        0        0     3390 2022-01-25 18:04:44.974356 rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-earth.css
--rw-r--r--   0        0        0     3395 2022-01-25 18:04:44.974587 rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-forest.css
--rw-r--r--   0        0        0     3380 2022-01-25 18:04:44.974832 rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-light.css
--rw-r--r--   0        0        0     3398 2022-01-25 18:04:44.975121 rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-sea.css
--rw-r--r--   0        0        0     3388 2022-01-25 18:04:44.975403 rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-space.css
--rw-r--r--   0        0        0     2495 2022-01-26 17:26:54.466540 rootmd-0.5.5/rootmd/data/css/prismjs/prism-funky.css
--rw-r--r--   0        0        0     1990 2022-01-26 17:26:54.466810 rootmd-0.5.5/rootmd/data/css/prismjs/prism-funky.min.css
--rw-r--r--   0        0        0     2109 2022-01-25 18:04:44.975646 rootmd-0.5.5/rootmd/data/css/prismjs/prism-ghcolors.css
--rw-r--r--   0        0        0     2417 2022-01-25 18:04:44.975906 rootmd-0.5.5/rootmd/data/css/prismjs/prism-gruvbox-dark.css
--rw-r--r--   0        0        0     2529 2022-01-25 18:04:44.976247 rootmd-0.5.5/rootmd/data/css/prismjs/prism-gruvbox-light.css
--rw-r--r--   0        0        0     2011 2022-01-25 18:04:44.976498 rootmd-0.5.5/rootmd/data/css/prismjs/prism-holi-theme.css
--rw-r--r--   0        0        0     1897 2022-01-25 18:04:44.976743 rootmd-0.5.5/rootmd/data/css/prismjs/prism-hopscotch.css
--rw-r--r--   0        0        0     1823 2022-01-25 18:04:44.977007 rootmd-0.5.5/rootmd/data/css/prismjs/prism-lucario.css
--rw-r--r--   0        0        0     2497 2022-01-25 18:04:44.977236 rootmd-0.5.5/rootmd/data/css/prismjs/prism-material-dark.css
--rw-r--r--   0        0        0     2534 2022-01-25 18:04:44.977495 rootmd-0.5.5/rootmd/data/css/prismjs/prism-material-light.css
--rw-r--r--   0        0        0     2556 2022-01-25 18:04:44.977769 rootmd-0.5.5/rootmd/data/css/prismjs/prism-material-oceanic.css
--rw-r--r--   0        0        0     2589 2022-01-25 18:04:44.978022 rootmd-0.5.5/rootmd/data/css/prismjs/prism-night-owl.css
--rw-r--r--   0        0        0     1814 2022-01-25 18:04:44.978485 rootmd-0.5.5/rootmd/data/css/prismjs/prism-nord.css
--rw-r--r--   0        0        0     1812 2022-01-26 17:26:54.467051 rootmd-0.5.5/rootmd/data/css/prismjs/prism-okaidia.css
--rw-r--r--   0        0        0     1380 2022-01-26 17:26:54.467296 rootmd-0.5.5/rootmd/data/css/prismjs/prism-okaidia.min.css
--rw-r--r--   0        0        0    12132 2022-01-25 18:04:44.978940 rootmd-0.5.5/rootmd/data/css/prismjs/prism-one-dark.css
--rw-r--r--   0        0        0    11915 2022-01-25 18:04:44.979313 rootmd-0.5.5/rootmd/data/css/prismjs/prism-one-light.css
--rw-r--r--   0        0        0     3839 2022-01-25 18:04:44.979733 rootmd-0.5.5/rootmd/data/css/prismjs/prism-pojoaque.css
--rw-r--r--   0        0        0     3246 2022-01-25 18:04:44.980147 rootmd-0.5.5/rootmd/data/css/prismjs/prism-shades-of-purple.css
--rw-r--r--   0        0        0     1968 2022-01-25 18:04:44.980547 rootmd-0.5.5/rootmd/data/css/prismjs/prism-solarized-dark-atom.css
--rw-r--r--   0        0        0     2606 2022-01-26 17:26:54.467598 rootmd-0.5.5/rootmd/data/css/prismjs/prism-solarizedlight.css
--rw-r--r--   0        0        0     1589 2022-01-26 17:26:54.467906 rootmd-0.5.5/rootmd/data/css/prismjs/prism-solarizedlight.min.css
--rw-r--r--   0        0        0     2456 2022-01-25 18:04:44.980951 rootmd-0.5.5/rootmd/data/css/prismjs/prism-synthwave84.css
--rw-r--r--   0        0        0     1766 2022-01-26 17:26:54.468220 rootmd-0.5.5/rootmd/data/css/prismjs/prism-tomorrow.css
--rw-r--r--   0        0        0     1313 2022-01-26 17:26:54.468651 rootmd-0.5.5/rootmd/data/css/prismjs/prism-tomorrow.min.css
--rw-r--r--   0        0        0     3620 2022-01-26 17:26:54.468909 rootmd-0.5.5/rootmd/data/css/prismjs/prism-twilight.css
--rw-r--r--   0        0        0     2440 2022-01-26 17:26:54.469224 rootmd-0.5.5/rootmd/data/css/prismjs/prism-twilight.min.css
--rw-r--r--   0        0        0     3070 2022-01-25 18:04:44.981346 rootmd-0.5.5/rootmd/data/css/prismjs/prism-vs.css
--rw-r--r--   0        0        0     4178 2022-01-25 18:04:44.981810 rootmd-0.5.5/rootmd/data/css/prismjs/prism-vsc-dark-plus.css
--rw-r--r--   0        0        0     2703 2022-01-25 18:04:44.982241 rootmd-0.5.5/rootmd/data/css/prismjs/prism-xonokai.css
--rw-r--r--   0        0        0     2520 2022-01-25 18:04:44.982641 rootmd-0.5.5/rootmd/data/css/prismjs/prism-z-touch.css
--rw-r--r--   0        0        0     2335 2022-01-26 17:26:54.469498 rootmd-0.5.5/rootmd/data/css/prismjs/prism.css
--rw-r--r--   0        0        0     1789 2022-01-26 17:26:54.469811 rootmd-0.5.5/rootmd/data/css/prismjs/prism.min.css
--rw-r--r--   0        0        0     5472 2022-01-27 01:07:11.056064 rootmd-0.5.5/rootmd/data/js/prism-1.26.0-autoloader.min.js
--rw-r--r--   0        0        0    18650 2022-01-27 01:06:30.716061 rootmd-0.5.5/rootmd/data/js/prism-1.26.0.min.js
--rw-r--r--   0        0        0     3272 2022-02-01 04:07:47.556802 rootmd-0.5.5/rootmd/data/template.html
--rw-r--r--   0        0        0      969 2022-03-03 14:59:57.527684 rootmd-0.5.5/setup.py
--rw-r--r--   0        0        0      767 2022-03-03 14:59:57.527971 rootmd-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-06 15:24:37.795290 rootmd-0.5.6/LICENSE
+-rw-r--r--   0        0        0     6494 2023-02-06 15:24:38.114069 rootmd-0.5.6/README.md
+-rw-r--r--   0        0        0      665 2023-04-28 17:52:46.155451 rootmd-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3503 2023-02-06 15:24:38.044937 rootmd-0.5.6/rootmd/Executor.py
+-rw-r--r--   0        0        0     4796 2023-02-06 15:24:37.988540 rootmd-0.5.6/rootmd/Md2MacroRenderer.py
+-rw-r--r--   0        0        0     2866 2023-02-06 15:24:38.045297 rootmd-0.5.6/rootmd/RootBaseRenderer.py
+-rw-r--r--   0        0        0    20986 2023-02-06 15:24:37.997268 rootmd-0.5.6/rootmd/RootHtmlRenderer.py
+-rw-r--r--   0        0        0     4049 2023-02-06 15:24:38.044529 rootmd-0.5.6/rootmd/RootMdRenderer.py
+-rw-r--r--   0        0        0     6549 2023-02-06 15:24:37.989078 rootmd-0.5.6/rootmd/YamlBlock.py
+-rw-r--r--   0        0        0      531 2023-02-06 15:24:37.989478 rootmd-0.5.6/rootmd/__init__.py
+-rwxr-xr-x   0        0        0     8597 2023-02-06 15:24:38.043952 rootmd-0.5.6/rootmd/__main__.py
+-rw-r--r--   0        0        0     1130 2023-02-06 15:24:38.019160 rootmd-0.5.6/rootmd/data/css/core.css
+-rw-r--r--   0        0        0     2438 2023-02-06 15:24:38.000040 rootmd-0.5.6/rootmd/data/css/prismjs/prism-a11y-dark.css
+-rw-r--r--   0        0        0     1945 2023-02-06 15:24:38.011657 rootmd-0.5.6/rootmd/data/css/prismjs/prism-atom-dark.css
+-rw-r--r--   0        0        0     3332 2023-02-06 15:24:38.013757 rootmd-0.5.6/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css
+-rw-r--r--   0        0        0     2618 2023-02-06 15:24:38.015816 rootmd-0.5.6/rootmd/data/css/prismjs/prism-cb.css
+-rw-r--r--   0        0        0     6782 2023-02-06 15:24:38.018137 rootmd-0.5.6/rootmd/data/css/prismjs/prism-coldark-cold.css
+-rw-r--r--   0        0        0     6776 2023-02-06 15:24:38.002562 rootmd-0.5.6/rootmd/data/css/prismjs/prism-coldark-dark.css
+-rw-r--r--   0        0        0     2306 2023-02-06 15:24:38.006485 rootmd-0.5.6/rootmd/data/css/prismjs/prism-coy-without-shadows.css
+-rw-r--r--   0        0        0     4031 2023-02-06 15:24:38.006001 rootmd-0.5.6/rootmd/data/css/prismjs/prism-coy.css
+-rw-r--r--   0        0        0     3062 2023-02-06 15:24:38.012747 rootmd-0.5.6/rootmd/data/css/prismjs/prism-coy.min.css
+-rw-r--r--   0        0        0     2680 2023-02-06 15:24:38.012408 rootmd-0.5.6/rootmd/data/css/prismjs/prism-darcula.css
+-rw-r--r--   0        0        0     2070 2023-02-06 15:24:38.009811 rootmd-0.5.6/rootmd/data/css/prismjs/prism-dark.css
+-rw-r--r--   0        0        0     1533 2023-02-06 15:24:38.002247 rootmd-0.5.6/rootmd/data/css/prismjs/prism-dark.min.css
+-rw-r--r--   0        0        0     1795 2023-02-06 15:24:38.006828 rootmd-0.5.6/rootmd/data/css/prismjs/prism-dracula.css
+-rw-r--r--   0        0        0     3389 2023-02-06 15:24:38.016149 rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-dark.css
+-rw-r--r--   0        0        0     3390 2023-02-06 15:24:38.018512 rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-earth.css
+-rw-r--r--   0        0        0     3395 2023-02-06 15:24:38.005334 rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-forest.css
+-rw-r--r--   0        0        0     3380 2023-02-06 15:24:37.999330 rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-light.css
+-rw-r--r--   0        0        0     3398 2023-02-06 15:24:38.015165 rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-sea.css
+-rw-r--r--   0        0        0     3388 2023-02-06 15:24:38.013409 rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-space.css
+-rw-r--r--   0        0        0     2495 2023-02-06 15:24:38.018836 rootmd-0.5.6/rootmd/data/css/prismjs/prism-funky.css
+-rw-r--r--   0        0        0     1990 2023-02-06 15:24:38.001000 rootmd-0.5.6/rootmd/data/css/prismjs/prism-funky.min.css
+-rw-r--r--   0        0        0     2109 2023-02-06 15:24:38.001639 rootmd-0.5.6/rootmd/data/css/prismjs/prism-ghcolors.css
+-rw-r--r--   0        0        0     2417 2023-02-06 15:24:38.004131 rootmd-0.5.6/rootmd/data/css/prismjs/prism-gruvbox-dark.css
+-rw-r--r--   0        0        0     2529 2023-02-06 15:24:37.999681 rootmd-0.5.6/rootmd/data/css/prismjs/prism-gruvbox-light.css
+-rw-r--r--   0        0        0     2011 2023-02-06 15:24:38.011256 rootmd-0.5.6/rootmd/data/css/prismjs/prism-holi-theme.css
+-rw-r--r--   0        0        0     1897 2023-02-06 15:24:38.001937 rootmd-0.5.6/rootmd/data/css/prismjs/prism-hopscotch.css
+-rw-r--r--   0        0        0     1823 2023-02-06 15:24:38.010752 rootmd-0.5.6/rootmd/data/css/prismjs/prism-lucario.css
+-rw-r--r--   0        0        0     2497 2023-02-06 15:24:38.000362 rootmd-0.5.6/rootmd/data/css/prismjs/prism-material-dark.css
+-rw-r--r--   0        0        0     2534 2023-02-06 15:24:38.000684 rootmd-0.5.6/rootmd/data/css/prismjs/prism-material-light.css
+-rw-r--r--   0        0        0     2556 2023-02-06 15:24:38.012028 rootmd-0.5.6/rootmd/data/css/prismjs/prism-material-oceanic.css
+-rw-r--r--   0        0        0     2589 2023-02-06 15:24:38.016816 rootmd-0.5.6/rootmd/data/css/prismjs/prism-night-owl.css
+-rw-r--r--   0        0        0     1814 2023-02-06 15:24:38.016491 rootmd-0.5.6/rootmd/data/css/prismjs/prism-nord.css
+-rw-r--r--   0        0        0     1812 2023-02-06 15:24:38.001312 rootmd-0.5.6/rootmd/data/css/prismjs/prism-okaidia.css
+-rw-r--r--   0        0        0     1380 2023-02-06 15:24:38.014831 rootmd-0.5.6/rootmd/data/css/prismjs/prism-okaidia.min.css
+-rw-r--r--   0        0        0    12132 2023-02-06 15:24:38.014101 rootmd-0.5.6/rootmd/data/css/prismjs/prism-one-dark.css
+-rw-r--r--   0        0        0    11915 2023-02-06 15:24:38.017810 rootmd-0.5.6/rootmd/data/css/prismjs/prism-one-light.css
+-rw-r--r--   0        0        0     3839 2023-02-06 15:24:38.017152 rootmd-0.5.6/rootmd/data/css/prismjs/prism-pojoaque.css
+-rw-r--r--   0        0        0     3246 2023-02-06 15:24:38.008435 rootmd-0.5.6/rootmd/data/css/prismjs/prism-shades-of-purple.css
+-rw-r--r--   0        0        0     1968 2023-02-06 15:24:38.003224 rootmd-0.5.6/rootmd/data/css/prismjs/prism-solarized-dark-atom.css
+-rw-r--r--   0        0        0     2606 2023-02-06 15:24:38.014446 rootmd-0.5.6/rootmd/data/css/prismjs/prism-solarizedlight.css
+-rw-r--r--   0        0        0     1589 2023-02-06 15:24:38.009417 rootmd-0.5.6/rootmd/data/css/prismjs/prism-solarizedlight.min.css
+-rw-r--r--   0        0        0     2456 2023-02-06 15:24:38.009005 rootmd-0.5.6/rootmd/data/css/prismjs/prism-synthwave84.css
+-rw-r--r--   0        0        0     1766 2023-02-06 15:24:38.003588 rootmd-0.5.6/rootmd/data/css/prismjs/prism-tomorrow.css
+-rw-r--r--   0        0        0     1313 2023-02-06 15:24:38.010322 rootmd-0.5.6/rootmd/data/css/prismjs/prism-tomorrow.min.css
+-rw-r--r--   0        0        0     3620 2023-02-06 15:24:38.017485 rootmd-0.5.6/rootmd/data/css/prismjs/prism-twilight.css
+-rw-r--r--   0        0        0     2440 2023-02-06 15:24:38.005672 rootmd-0.5.6/rootmd/data/css/prismjs/prism-twilight.min.css
+-rw-r--r--   0        0        0     3070 2023-02-06 15:24:38.013066 rootmd-0.5.6/rootmd/data/css/prismjs/prism-vs.css
+-rw-r--r--   0        0        0     4178 2023-02-06 15:24:38.002892 rootmd-0.5.6/rootmd/data/css/prismjs/prism-vsc-dark-plus.css
+-rw-r--r--   0        0        0     2703 2023-02-06 15:24:38.007145 rootmd-0.5.6/rootmd/data/css/prismjs/prism-xonokai.css
+-rw-r--r--   0        0        0     2520 2023-02-06 15:24:38.008097 rootmd-0.5.6/rootmd/data/css/prismjs/prism-z-touch.css
+-rw-r--r--   0        0        0     2335 2023-02-06 15:24:38.015488 rootmd-0.5.6/rootmd/data/css/prismjs/prism.css
+-rw-r--r--   0        0        0     1789 2023-02-06 15:24:38.007670 rootmd-0.5.6/rootmd/data/css/prismjs/prism.min.css
+-rw-r--r--   0        0        0     5472 2023-02-06 15:24:38.042782 rootmd-0.5.6/rootmd/data/js/prism-1.26.0-autoloader.min.js
+-rw-r--r--   0        0        0    18650 2023-02-06 15:24:38.042093 rootmd-0.5.6/rootmd/data/js/prism-1.26.0.min.js
+-rw-r--r--   0        0        0     3272 2023-02-06 15:24:38.043544 rootmd-0.5.6/rootmd/data/template.html
+-rw-r--r--   0        0        0     7354 1970-01-01 00:00:00.000000 rootmd-0.5.6/PKG-INFO
```

### Comparing `rootmd-0.5.5/LICENSE` & `rootmd-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/pyproject.toml` & `rootmd-0.5.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "rootmd"
-version = "0.5.5"
+version = "0.5.6"
 description = "RootMD is a markdown processor for markdown with ROOT-flavored c++ code. RootMD can execute c++ code and inject the output (from stdout, stderr) and link or embed image outputs"
 authors = ["Daniel Brandenburg <hello@jdbburg.com>"]
 include = ["rootmd/data"]
-
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^11.0.0"
 mistletoe = "^0.8.1"
 watchdog = "^2.1.6"
 pyyaml = "^5.4.1"
```

### Comparing `rootmd-0.5.5/rootmd/Executor.py` & `rootmd-0.5.6/rootmd/Executor.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/Md2MacroRenderer.py` & `rootmd-0.5.6/rootmd/Md2MacroRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/RootBaseRenderer.py` & `rootmd-0.5.6/rootmd/RootBaseRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/RootHtmlRenderer.py` & `rootmd-0.5.6/rootmd/RootHtmlRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/RootMdRenderer.py` & `rootmd-0.5.6/rootmd/RootMdRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/YamlBlock.py` & `rootmd-0.5.6/rootmd/YamlBlock.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/__init__.py` & `rootmd-0.5.6/rootmd/__init__.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/__main__.py` & `rootmd-0.5.6/rootmd/__main__.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/core.css` & `rootmd-0.5.6/rootmd/data/css/core.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-a11y-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-a11y-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-atom-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-atom-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-cb.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-cb.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-coldark-cold.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-coldark-cold.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-coldark-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-coldark-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-coy-without-shadows.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-coy-without-shadows.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-coy.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-coy.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-coy.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-coy.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-darcula.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-darcula.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-dark.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-dark.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-dracula.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-dracula.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-earth.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-earth.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-forest.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-forest.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-light.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-sea.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-sea.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-duotone-space.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-duotone-space.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-funky.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-funky.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-funky.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-funky.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-ghcolors.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-ghcolors.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-gruvbox-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-gruvbox-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-gruvbox-light.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-gruvbox-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-holi-theme.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-holi-theme.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-hopscotch.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-hopscotch.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-lucario.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-lucario.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-material-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-material-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-material-light.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-material-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-material-oceanic.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-material-oceanic.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-night-owl.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-night-owl.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-nord.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-nord.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-okaidia.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-okaidia.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-okaidia.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-okaidia.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-one-dark.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-one-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-one-light.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-one-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-pojoaque.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-pojoaque.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-shades-of-purple.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-shades-of-purple.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-solarized-dark-atom.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-solarized-dark-atom.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-solarizedlight.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-solarizedlight.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-solarizedlight.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-solarizedlight.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-synthwave84.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-synthwave84.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-tomorrow.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-tomorrow.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-tomorrow.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-tomorrow.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-twilight.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-twilight.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-twilight.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-twilight.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-vs.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-vs.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-vsc-dark-plus.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-vsc-dark-plus.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-xonokai.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-xonokai.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism-z-touch.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism-z-touch.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/css/prismjs/prism.min.css` & `rootmd-0.5.6/rootmd/data/css/prismjs/prism.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/js/prism-1.26.0-autoloader.min.js` & `rootmd-0.5.6/rootmd/data/js/prism-1.26.0-autoloader.min.js`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/js/prism-1.26.0.min.js` & `rootmd-0.5.6/rootmd/data/js/prism-1.26.0.min.js`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.5/rootmd/data/template.html` & `rootmd-0.5.6/rootmd/data/template.html`

 * *Files identical despite different names*

