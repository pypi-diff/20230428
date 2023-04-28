# Comparing `tmp/brevitas-0.9.0.tar.gz` & `tmp/brevitas-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brevitas-0.9.0.tar", last modified: Fri Apr 21 17:52:33 2023, max compression
+gzip compressed data, was "brevitas-0.9.1.tar", last modified: Fri Apr 28 16:55:10 2023, max compression
```

## Comparing `brevitas-0.9.0.tar` & `brevitas-0.9.1.tar`

### file list

```diff
@@ -1,379 +1,378 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.742040 brevitas-0.9.0/
--rw-rw-rw-   0        0        0      824 2023-04-21 17:11:25.000000 brevitas-0.9.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     2137 2023-04-21 17:11:25.000000 brevitas-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      361 2023-01-10 09:12:31.000000 brevitas-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3844 2023-04-21 17:52:33.741040 brevitas-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3220 2023-04-21 17:12:45.000000 brevitas-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.700482 brevitas-0.9.0/notebooks/
--rw-rw-rw-   0        0        0    60778 2023-04-21 17:11:25.000000 brevitas-0.9.0/notebooks/01_quant_tensor_quant_conv2d_overview.ipynb
--rw-rw-rw-   0        0        0    35108 2023-04-21 17:11:25.000000 brevitas-0.9.0/notebooks/02_quant_activation_overview.ipynb
--rw-rw-rw-   0        0        0    70607 2023-04-21 17:11:25.000000 brevitas-0.9.0/notebooks/03_anatomy_of_a_quantizer.ipynb
--rw-rw-rw-   0        0        0    98682 2023-01-10 09:12:32.000000 brevitas-0.9.0/notebooks/Brevitas_TVMCon2021.ipynb
--rw-rw-rw-   0        0        0    52335 2023-04-21 17:11:25.000000 brevitas-0.9.0/notebooks/ONNX_export_tutorial.ipynb
--rw-rw-rw-   0        0        0    59257 2023-01-10 09:12:32.000000 brevitas-0.9.0/notebooks/quantized_recurrent.ipynb
--rw-rw-rw-   0        0        0      396 2023-04-21 17:11:25.000000 brevitas-0.9.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.745839 brevitas-0.9.0/requirements/
--rw-rw-rw-   0        0        0      145 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-docs.txt
--rw-rw-rw-   0        0        0       19 2023-01-10 09:12:32.000000 brevitas-0.9.0/requirements/requirements-export.txt
--rw-rw-rw-   0        0        0       56 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-finn-integration.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-hadamard.txt
--rw-rw-rw-   0        0        0       15 2023-01-10 09:12:32.000000 brevitas-0.9.0/requirements/requirements-notebook.txt
--rw-rw-rw-   0        0        0       21 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-nox.txt
--rw-rw-rw-   0        0        0       31 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-ort-integration.txt
--rw-rw-rw-   0        0        0       15 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-setup.txt
--rw-rw-rw-   0        0        0       97 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-stt.txt
--rw-rw-rw-   0        0        0       79 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-test.txt
--rw-rw-rw-   0        0        0       49 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-tts.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements-vision.txt
--rw-rw-rw-   0        0        0      126 2023-04-21 17:11:25.000000 brevitas-0.9.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 17:52:33.742040 brevitas-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2641 2023-04-21 17:11:25.000000 brevitas-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.627483 brevitas-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.758483 brevitas-0.9.0/src/brevitas/
--rw-rw-rw-   0        0        0     2796 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/common.py
--rw-rw-rw-   0        0        0      887 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/config.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.792482 brevitas-0.9.0/src/brevitas/core/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.801484 brevitas-0.9.0/src/brevitas/core/bit_width/
--rw-rw-rw-   0        0        0      463 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/bit_width/__init__.py
--rw-rw-rw-   0        0        0     3721 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/bit_width/const.py
--rw-rw-rw-   0        0        0     6202 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/bit_width/parameter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.821482 brevitas-0.9.0/src/brevitas/core/function_wrapper/
--rw-rw-rw-   0        0        0      803 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/function_wrapper/__init__.py
--rw-rw-rw-   0        0        0     2002 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/function_wrapper/clamp.py
--rw-rw-rw-   0        0        0     3115 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/function_wrapper/learned_round.py
--rw-rw-rw-   0        0        0     2047 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/function_wrapper/misc.py
--rw-rw-rw-   0        0        0     3137 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/function_wrapper/ops_ste.py
--rw-rw-rw-   0        0        0     3944 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/function_wrapper/shape.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.844482 brevitas-0.9.0/src/brevitas/core/quant/
--rw-rw-rw-   0        0        0      596 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/quant/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/quant/binary.py
--rw-rw-rw-   0        0        0     1776 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/quant/delay.py
--rw-rw-rw-   0        0        0    10619 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/quant/int.py
--rw-rw-rw-   0        0        0     6694 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/quant/int_base.py
--rw-rw-rw-   0        0        0     2475 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/quant/ternary.py
--rw-rw-rw-   0        0        0     5018 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/restrict_val.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.861482 brevitas-0.9.0/src/brevitas/core/scaling/
--rw-rw-rw-   0        0        0      571 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/scaling/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/scaling/int_scaling.py
--rw-rw-rw-   0        0        0    10521 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/scaling/pre_scaling.py
--rw-rw-rw-   0        0        0     5412 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/scaling/runtime.py
--rw-rw-rw-   0        0        0    14748 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/scaling/standalone.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.875485 brevitas-0.9.0/src/brevitas/core/stats/
--rw-rw-rw-   0        0        0      829 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/stats/__init__.py
--rw-rw-rw-   0        0        0    15934 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/stats/stats_op.py
--rw-rw-rw-   0        0        0     4500 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/stats/stats_wrapper.py
--rw-rw-rw-   0        0        0     2699 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/stats/view_wrapper.py
--rw-rw-rw-   0        0        0     2523 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/utils.py
--rw-rw-rw-   0        0        0     9053 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/core/zero_point.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.878485 brevitas-0.9.0/src/brevitas/csrc/
--rw-rw-rw-   0        0        0     7051 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/csrc/autograd_ste_ops.cpp
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.883483 brevitas-0.9.0/src/brevitas/export/
--rw-rw-rw-   0        0        0     1363 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.887483 brevitas-0.9.0/src/brevitas/export/common/
--rw-rw-rw-   0        0        0      425 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.896483 brevitas-0.9.0/src/brevitas/export/common/handler/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/common/handler/__init__.py
--rw-rw-rw-   0        0        0     5533 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/common/handler/base.py
--rw-rw-rw-   0        0        0    12025 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/common/handler/qcdq.py
--rw-rw-rw-   0        0        0    11884 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.913485 brevitas-0.9.0/src/brevitas/export/onnx/
--rw-rw-rw-   0        0        0      472 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/__init__.py
--rw-rw-rw-   0        0        0     1935 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/debug.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.926483 brevitas-0.9.0/src/brevitas/export/onnx/finn/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.938485 brevitas-0.9.0/src/brevitas/export/onnx/finn/function/
--rw-rw-rw-   0        0        0      154 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/function/__init__.py
--rw-rw-rw-   0        0        0      947 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/function/acc.py
--rw-rw-rw-   0        0        0     1347 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/function/act.py
--rw-rw-rw-   0        0        0     2607 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/function/parameter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.955484 brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/__init__.py
--rw-rw-rw-   0        0        0     2163 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/acc.py
--rw-rw-rw-   0        0        0     5692 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/act.py
--rw-rw-rw-   0        0        0     3096 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/base.py
--rw-rw-rw-   0        0        0     6371 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/parameter.py
--rw-rw-rw-   0        0        0     5803 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/manager.py
--rw-rw-rw-   0        0        0     2138 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/transform.py
--rw-rw-rw-   0        0        0      586 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/finn/utils.py
--rw-rw-rw-   0        0        0     1805 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/function.py
--rw-rw-rw-   0        0        0    10476 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/handler.py
--rw-rw-rw-   0        0        0     6871 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.968485 brevitas-0.9.0/src/brevitas/export/onnx/qonnx/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/qonnx/__init__.py
--rw-rw-rw-   0        0        0    13891 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/qonnx/function.py
--rw-rw-rw-   0        0        0     6196 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/qonnx/handler.py
--rw-rw-rw-   0        0        0     2179 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/qonnx/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.979483 brevitas-0.9.0/src/brevitas/export/onnx/standard/
--rw-rw-rw-   0        0        0      112 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/function.py
--rw-rw-rw-   0        0        0     1613 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.990485 brevitas-0.9.0/src/brevitas/export/onnx/standard/qcdq/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qcdq/__init__.py
--rw-rw-rw-   0        0        0     4002 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qcdq/handler.py
--rw-rw-rw-   0        0        0     2125 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qcdq/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.001484 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/__init__.py
--rw-rw-rw-   0        0        0     3231 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/function.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.020484 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/
--rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/__init__.py
--rw-rw-rw-   0        0        0     5759 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/act.py
--rw-rw-rw-   0        0        0     7390 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/base.py
--rw-rw-rw-   0        0        0     8186 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/parameter.py
--rw-rw-rw-   0        0        0     1370 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/pool.py
--rw-rw-rw-   0        0        0     3364 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.609964 brevitas-0.9.0/src/brevitas/export/torch/
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.030483 brevitas-0.9.0/src/brevitas/export/torch/qcdq/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qcdq/__init__.py
--rw-rw-rw-   0        0        0     4304 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qcdq/handler.py
--rw-rw-rw-   0        0        0     1361 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qcdq/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.037483 brevitas-0.9.0/src/brevitas/export/torch/qoperator/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.056483 brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/
--rw-rw-rw-   0        0        0      213 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/__init__.py
--rw-rw-rw-   0        0        0     2054 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/act.py
--rw-rw-rw-   0        0        0     2373 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/base.py
--rw-rw-rw-   0        0        0     4781 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/parameter.py
--rw-rw-rw-   0        0        0     1812 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/pool.py
--rw-rw-rw-   0        0        0     2509 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/export/torch/qoperator/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.070483 brevitas-0.9.0/src/brevitas/function/
--rw-rw-rw-   0        0        0      155 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/function/__init__.py
--rw-rw-rw-   0        0        0     5513 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/function/ops.py
--rw-rw-rw-   0        0        0    13010 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/function/ops_ste.py
--rw-rw-rw-   0        0        0     2314 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/function/shape.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.082482 brevitas-0.9.0/src/brevitas/fx/
--rw-rw-rw-   0        0        0     3549 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.121484 brevitas-0.9.0/src/brevitas/fx/backport/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/__init__.py
--rw-rw-rw-   0        0        0    39947 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/graph.py
--rw-rw-rw-   0        0        0    17454 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/graph_module.py
--rw-rw-rw-   0        0        0     3427 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/immutable_collections.py
--rw-rw-rw-   0        0        0    18108 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/interpreter.py
--rw-rw-rw-   0        0        0    14017 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/node.py
--rw-rw-rw-   0        0        0    11952 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/proxy.py
--rw-rw-rw-   0        0        0    16627 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/subgraph_rewriter.py
--rw-rw-rw-   0        0        0    28505 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/symbolic_trace.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.141484 brevitas-0.9.0/src/brevitas/fx/backport/torch_function/
--rw-rw-rw-   0        0        0      190 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/torch_function/__init__.py
--rw-rw-rw-   0        0        0     7731 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/torch_function/_overrides.py
--rw-rw-rw-   0        0        0     4319 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/torch_function/patch.py
--rw-rw-rw-   0        0        0    61914 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/backport/torch_function/signatures.py
--rw-rw-rw-   0        0        0     2274 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/brevitas_tracer.py
--rw-rw-rw-   0        0        0    21509 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/fx/value_tracer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.188485 brevitas-0.9.0/src/brevitas/graph/
--rw-rw-rw-   0        0        0      261 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/__init__.py
--rw-rw-rw-   0        0        0    10632 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/base.py
--rw-rw-rw-   0        0        0    11684 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/calibrate.py
--rw-rw-rw-   0        0        0    20501 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/equalize.py
--rw-rw-rw-   0        0        0     8309 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/fixed_point.py
--rw-rw-rw-   0        0        0     5021 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/per_input.py
--rw-rw-rw-   0        0        0    13412 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/quantize.py
--rw-rw-rw-   0        0        0    19261 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/quantize_impl.py
--rw-rw-rw-   0        0        0     5927 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/standardize.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.197483 brevitas-0.9.0/src/brevitas/graph/target/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/target/__init__.py
--rw-rw-rw-   0        0        0     6919 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/target/flexml.py
--rw-rw-rw-   0        0        0     4880 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/graph/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.210637 brevitas-0.9.0/src/brevitas/inject/
--rw-rw-rw-   0        0        0     7787 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/inject/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/inject/defaults.py
--rw-rw-rw-   0        0        0     1451 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/inject/enum.py
--rw-rw-rw-   0        0        0      788 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/jit.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.222485 brevitas-0.9.0/src/brevitas/loss/
--rw-rw-rw-   0        0        0      346 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/loss/__init__.py
--rw-rw-rw-   0        0        0      743 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/loss/base_loss.py
--rw-rw-rw-   0        0        0     3790 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/loss/weighted_bit_width.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.288483 brevitas-0.9.0/src/brevitas/nn/
--rw-rw-rw-   0        0        0     1516 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/__init__.py
--rw-rw-rw-   0        0        0     3439 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/hadamard_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.307483 brevitas-0.9.0/src/brevitas/nn/mixin/
--rw-rw-rw-   0        0        0      468 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/mixin/__init__.py
--rw-rw-rw-   0        0        0     1919 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/mixin/acc.py
--rw-rw-rw-   0        0        0     4085 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/mixin/act.py
--rw-rw-rw-   0        0        0    12643 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/mixin/base.py
--rw-rw-rw-   0        0        0     7083 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/mixin/parameter.py
--rw-rw-rw-   0        0        0      261 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/mixin/utils.py
--rw-rw-rw-   0        0        0     1828 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_accumulator.py
--rw-rw-rw-   0        0        0     3013 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_activation.py
--rw-rw-rw-   0        0        0     5880 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_avg_pool.py
--rw-rw-rw-   0        0        0     3823 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_bn.py
--rw-rw-rw-   0        0        0     8226 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_conv.py
--rw-rw-rw-   0        0        0     8260 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_convtranspose.py
--rw-rw-rw-   0        0        0      871 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_dropout.py
--rw-rw-rw-   0        0        0     3122 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_eltwise.py
--rw-rw-rw-   0        0        0     2485 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_embedding.py
--rw-rw-rw-   0        0        0    12986 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_layer.py
--rw-rw-rw-   0        0        0     2519 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_linear.py
--rw-rw-rw-   0        0        0     2457 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_max_pool.py
--rw-rw-rw-   0        0        0    36694 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_mha.py
--rw-rw-rw-   0        0        0    40303 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_rnn.py
--rw-rw-rw-   0        0        0     3077 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_scale_bias.py
--rw-rw-rw-   0        0        0     3627 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/quant_upsample.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.313483 brevitas-0.9.0/src/brevitas/nn/target/
--rw-rw-rw-   0        0        0      195 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/target/__init__.py
--rw-rw-rw-   0        0        0     5852 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/target/flexml.py
--rw-rw-rw-   0        0        0     6092 2023-04-21 17:11:25.000000 brevitas-0.9.0/src/brevitas/nn/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.316484 brevitas-0.9.0/src/brevitas/onnx/
--rw-rw-rw-   0        0        0      452 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/onnx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.322483 brevitas-0.9.0/src/brevitas/ops/
--rw-rw-rw-   0        0        0      418 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/ops/__init__.py
--rw-rw-rw-   0        0        0    14701 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/ops/autograd_ste_ops.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.339483 brevitas-0.9.0/src/brevitas/proxy/
--rw-rw-rw-   0        0        0      533 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/proxy/__init__.py
--rw-rw-rw-   0        0        0     7483 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/proxy/parameter_quant.py
--rw-rw-rw-   0        0        0     4943 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/proxy/quant_proxy.py
--rw-rw-rw-   0        0        0     7804 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/proxy/runtime_quant.py
--rw-rw-rw-   0        0        0     1572 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/proxy/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.367012 brevitas-0.9.0/src/brevitas/quant/
--rw-rw-rw-   0        0        0      265 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/__init__.py
--rw-rw-rw-   0        0        0    15008 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/base.py
--rw-rw-rw-   0        0        0     1237 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/binary.py
--rw-rw-rw-   0        0        0     6619 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/fixed_point.py
--rw-rw-rw-   0        0        0     1289 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/none.py
--rw-rw-rw-   0        0        0    13323 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/scaled_int.py
--rw-rw-rw-   0        0        0     3144 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/shifted_scaled_int.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.394012 brevitas-0.9.0/src/brevitas/quant/solver/
--rw-rw-rw-   0        0        0      289 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/__init__.py
--rw-rw-rw-   0        0        0     5181 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/act.py
--rw-rw-rw-   0        0        0     3591 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/bias.py
--rw-rw-rw-   0        0        0     2208 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/clamp.py
--rw-rw-rw-   0        0        0     6661 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/common.py
--rw-rw-rw-   0        0        0     4509 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/parameter.py
--rw-rw-rw-   0        0        0     1491 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/trunc.py
--rw-rw-rw-   0        0        0     4168 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/solver/weight.py
--rw-rw-rw-   0        0        0     1416 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant/ternary.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.401012 brevitas-0.9.0/src/brevitas/quant_tensor/
--rw-rw-rw-   0        0        0    17983 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant_tensor/__init__.py
--rw-rw-rw-   0        0        0     4117 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/quant_tensor/torch_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.421012 brevitas-0.9.0/src/brevitas/utils/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/utils/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/utils/jit_utils.py
--rw-rw-rw-   0        0        0     1668 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/utils/logging.py
--rw-rw-rw-   0        0        0      914 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/utils/python_utils.py
--rw-rw-rw-   0        0        0     1836 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/utils/quant_utils.py
--rw-rw-rw-   0        0        0      901 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:32.779484 brevitas-0.9.0/src/brevitas.egg-info/
--rw-rw-rw-   0        0        0     3844 2023-04-21 17:52:29.000000 brevitas-0.9.0/src/brevitas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13924 2023-04-21 17:52:32.000000 brevitas-0.9.0/src/brevitas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 17:52:29.000000 brevitas-0.9.0/src/brevitas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      699 2023-04-21 17:52:29.000000 brevitas-0.9.0/src/brevitas.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-10 09:14:58.000000 brevitas-0.9.0/src/brevitas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      751 2023-04-21 17:52:29.000000 brevitas-0.9.0/src/brevitas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-21 17:52:29.000000 brevitas-0.9.0/src/brevitas.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.427011 brevitas-0.9.0/src/brevitas_examples/
--rw-rw-rw-   0        0        0      413 2023-04-21 17:12:45.000000 brevitas-0.9.0/src/brevitas_examples/README.md
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.443013 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/
--rw-rw-rw-   0        0        0     2972 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/README.md
--rw-rw-rw-   0        0        0      330 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/bnn_pynq_train.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.483013 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/__init__.py
--rw-rw-rw-   0        0        0      337 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/cnv_1w1a.ini
--rw-rw-rw-   0        0        0      337 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/cnv_1w2a.ini
--rw-rw-rw-   0        0        0      337 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/cnv_2w2a.ini
--rw-rw-rw-   0        0        0      364 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/lfc_1w1a.ini
--rw-rw-rw-   0        0        0      364 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/lfc_1w2a.ini
--rw-rw-rw-   0        0        0      102 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/resnet18_3w3a.ini
--rw-rw-rw-   0        0        0      102 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/resnet18_4w4a.ini
--rw-rw-rw-   0        0        0      361 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/sfc_1w1a.ini
--rw-rw-rw-   0        0        0      361 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/sfc_1w2a.ini
--rw-rw-rw-   0        0        0      361 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/sfc_2w2a.ini
--rw-rw-rw-   0        0        0      358 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/tfc_1w1a.ini
--rw-rw-rw-   0        0        0      358 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/tfc_1w2a.ini
--rw-rw-rw-   0        0        0      358 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/cfg/tfc_2w2a.ini
--rw-rw-rw-   0        0        0     3318 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.504011 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/
--rw-rw-rw-   0        0        0     4226 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/CNV.py
--rw-rw-rw-   0        0        0     3032 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/FC.py
--rw-rw-rw-   0        0        0     2635 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/common.py
--rw-rw-rw-   0        0        0     1100 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/losses.py
--rw-rw-rw-   0        0        0     7535 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/resnet.py
--rw-rw-rw-   0        0        0     1468 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/tensor_norm.py
--rw-rw-rw-   0        0        0    12702 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/bnn_pynq/trainer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.513011 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/
--rw-rw-rw-   0        0        0     1735 2023-04-21 17:12:45.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/README.md
--rw-rw-rw-   0        0        0      135 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.534012 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/
--rw-rw-rw-   0        0        0     2464 2023-04-21 17:12:45.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/README.md
--rw-rw-rw-   0        0        0     3318 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.558014 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/__init__.py
--rw-rw-rw-   0        0        0      199 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_mobilenet_v1.ini
--rw-rw-rw-   0        0        0      438 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_mobilenet_v1_4b.ini
--rw-rw-rw-   0        0        0      437 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_mobilenet_v1_4b_round_avgpool.ini
--rw-rw-rw-   0        0        0      524 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b.ini
--rw-rw-rw-   0        0        0      528 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b5b.ini
--rw-rw-rw-   0        0        0      523 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b_round_avgpool.ini
--rw-rw-rw-   0        0        0      542 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_hadamard_4b.ini
--rw-rw-rw-   0        0        0     1387 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/common.py
--rw-rw-rw-   0        0        0     6859 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/mobilenetv1.py
--rw-rw-rw-   0        0        0    11786 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/proxylessnas.py
--rw-rw-rw-   0        0        0     6268 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/vgg.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.585011 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/
--rw-rw-rw-   0        0        0     9027 2023-04-21 17:12:45.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/README.md
--rw-rw-rw-   0        0        0      325 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/RESULTS_IMGCLSMOB.csv
--rw-rw-rw-   0        0        0    76880 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION.csv
--rw-rw-rw-   0        0        0     8983 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv
--rw-rw-rw-   0        0        0    12900 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/ptq_benchmark.py
--rw-rw-rw-   0        0        0     7437 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/ptq_common.py
--rw-rw-rw-   0        0        0     9803 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py
--rw-rw-rw-   0        0        0     1676 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.594012 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/qat/
--rw-rw-rw-   0        0        0     2973 2023-04-21 17:12:45.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/qat/README.md
--rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/qat/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/qat/imagenet_val.py
--rw-rw-rw-   0        0        0     3697 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/imagenet_classification/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.608013 brevitas-0.9.0/src/brevitas_examples/speech_to_text/
--rw-rw-rw-   0        0        0     3069 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/README.md
--rw-rw-rw-   0        0        0      138 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.622013 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/
--rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/__init__.py
--rw-rw-rw-   0        0        0      601 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_4b.ini
--rw-rw-rw-   0        0        0      603 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_8b.ini
--rw-rw-rw-   0        0        0      602 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_pertensorscaling_8b.ini
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.629012 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/topology/
--rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/topology/__init__.py
--rw-rw-rw-   0        0        0     3475 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/topology/quartznet15x5.yaml
--rw-rw-rw-   0        0        0     5304 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/get_librispeech_data.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.656012 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/
--rw-rw-rw-   0        0        0     3172 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/__init__.py
--rw-rw-rw-   0        0        0    19330 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/audio_preprocessing.py
--rw-rw-rw-   0        0        0     5995 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/data_layer.py
--rw-rw-rw-   0        0        0     1105 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/greedy_ctc_decoder.py
--rw-rw-rw-   0        0        0     7802 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/helpers.py
--rw-rw-rw-   0        0        0     1818 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/losses.py
--rw-rw-rw-   0        0        0     2634 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.690012 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/
--rw-rw-rw-   0        0        0      961 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/__init__.py
--rw-rw-rw-   0        0        0     6487 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/cleaners.py
--rw-rw-rw-   0        0        0     3501 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/common.py
--rw-rw-rw-   0        0        0     7744 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/dataset.py
--rw-rw-rw-   0        0        0    11831 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/features.py
--rw-rw-rw-   0        0        0     7658 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/manifest.py
--rw-rw-rw-   0        0        0     6652 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/perturb.py
--rw-rw-rw-   0        0        0    20949 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/quartznet.py
--rw-rw-rw-   0        0        0     8321 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/segment.py
--rw-rw-rw-   0        0        0     3634 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/spectr_augment.py
--rw-rw-rw-   0        0        0    11990 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/quartznet.py
--rw-rw-rw-   0        0        0     3823 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet_val.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.705011 brevitas-0.9.0/src/brevitas_examples/text_to_speech/
--rw-rw-rw-   0        0        0     2193 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/README.md
--rw-rw-rw-   0        0        0      135 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.710011 brevitas-0.9.0/src/brevitas_examples/text_to_speech/cfg/
--rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/cfg/__init__.py
--rw-rw-rw-   0        0        0      365 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/cfg/quant_melgan_8b.ini
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.727013 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/
--rw-rw-rw-   0        0        0      946 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/__init__.py
--rw-rw-rw-   0        0        0     4942 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/common.py
--rw-rw-rw-   0        0        0     4914 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/generator_brevitas.py
--rw-rw-rw-   0        0        0     1959 2023-01-10 09:12:32.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/melgan.py
--rw-rw-rw-   0        0        0     3588 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/res_stack_brevitas.py
--rw-rw-rw-   0        0        0     1969 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan_val.py
--rw-rw-rw-   0        0        0     2403 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/preprocess_dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:52:33.737040 brevitas-0.9.0/src/brevitas_examples/text_to_speech/utilities/
--rw-rw-rw-   0        0        0       73 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/utilities/__init__.py
--rw-rw-rw-   0        0        0     4614 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/utilities/audio_processing.py
--rw-rw-rw-   0        0        0     8078 2023-04-21 17:11:26.000000 brevitas-0.9.0/src/brevitas_examples/text_to_speech/utilities/stft.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.824547 brevitas-0.9.1/
+-rw-rw-rw-   0        0        0      824 2023-04-21 17:11:25.000000 brevitas-0.9.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     2137 2023-04-21 17:11:25.000000 brevitas-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      361 2023-01-10 09:12:31.000000 brevitas-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4754 2023-04-28 16:55:10.825547 brevitas-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4111 2023-04-28 11:37:43.000000 brevitas-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.880633 brevitas-0.9.1/notebooks/
+-rw-rw-rw-   0        0        0    60778 2023-04-21 17:11:25.000000 brevitas-0.9.1/notebooks/01_quant_tensor_quant_conv2d_overview.ipynb
+-rw-rw-rw-   0        0        0    35108 2023-04-21 17:11:25.000000 brevitas-0.9.1/notebooks/02_quant_activation_overview.ipynb
+-rw-rw-rw-   0        0        0    70607 2023-04-21 17:11:25.000000 brevitas-0.9.1/notebooks/03_anatomy_of_a_quantizer.ipynb
+-rw-rw-rw-   0        0        0    98682 2023-01-10 09:12:32.000000 brevitas-0.9.1/notebooks/Brevitas_TVMCon2021.ipynb
+-rw-rw-rw-   0        0        0    52335 2023-04-21 17:11:25.000000 brevitas-0.9.1/notebooks/ONNX_export_tutorial.ipynb
+-rw-rw-rw-   0        0        0    59257 2023-01-10 09:12:32.000000 brevitas-0.9.1/notebooks/quantized_recurrent.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.919633 brevitas-0.9.1/requirements/
+-rw-rw-rw-   0        0        0       11 2023-04-28 11:25:31.000000 brevitas-0.9.1/requirements/requirements-dev.txt
+-rw-rw-rw-   0        0        0      145 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-docs.txt
+-rw-rw-rw-   0        0        0       19 2023-01-10 09:12:32.000000 brevitas-0.9.1/requirements/requirements-export.txt
+-rw-rw-rw-   0        0        0       56 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-finn-integration.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-hadamard.txt
+-rw-rw-rw-   0        0        0       15 2023-01-10 09:12:32.000000 brevitas-0.9.1/requirements/requirements-notebook.txt
+-rw-rw-rw-   0        0        0       21 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-nox.txt
+-rw-rw-rw-   0        0        0       31 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-ort-integration.txt
+-rw-rw-rw-   0        0        0       15 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-setup.txt
+-rw-rw-rw-   0        0        0       97 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-stt.txt
+-rw-rw-rw-   0        0        0       86 2023-04-28 11:25:31.000000 brevitas-0.9.1/requirements/requirements-test.txt
+-rw-rw-rw-   0        0        0       49 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-tts.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 17:11:25.000000 brevitas-0.9.1/requirements/requirements-vision.txt
+-rw-rw-rw-   0        0        0       79 2023-04-28 16:51:19.000000 brevitas-0.9.1/requirements/requirements.txt
+-rw-rw-rw-   0        0        0      442 2023-04-28 16:55:10.827543 brevitas-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2696 2023-04-28 16:51:19.000000 brevitas-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.827632 brevitas-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.931151 brevitas-0.9.1/src/brevitas/
+-rw-rw-rw-   0        0        0     2796 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/common.py
+-rw-rw-rw-   0        0        0      887 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/config.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.963668 brevitas-0.9.1/src/brevitas/core/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.973669 brevitas-0.9.1/src/brevitas/core/bit_width/
+-rw-rw-rw-   0        0        0      463 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/bit_width/__init__.py
+-rw-rw-rw-   0        0        0     3721 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/bit_width/const.py
+-rw-rw-rw-   0        0        0     6202 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/bit_width/parameter.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.993669 brevitas-0.9.1/src/brevitas/core/function_wrapper/
+-rw-rw-rw-   0        0        0      803 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/function_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     2002 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/function_wrapper/clamp.py
+-rw-rw-rw-   0        0        0     3115 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/core/function_wrapper/learned_round.py
+-rw-rw-rw-   0        0        0     2047 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/function_wrapper/misc.py
+-rw-rw-rw-   0        0        0     3137 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/function_wrapper/ops_ste.py
+-rw-rw-rw-   0        0        0     3944 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/function_wrapper/shape.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.011185 brevitas-0.9.1/src/brevitas/core/quant/
+-rw-rw-rw-   0        0        0      596 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/quant/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/quant/binary.py
+-rw-rw-rw-   0        0        0     1776 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/quant/delay.py
+-rw-rw-rw-   0        0        0    10619 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/core/quant/int.py
+-rw-rw-rw-   0        0        0     6694 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/quant/int_base.py
+-rw-rw-rw-   0        0        0     2475 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/quant/ternary.py
+-rw-rw-rw-   0        0        0     5018 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/restrict_val.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.028699 brevitas-0.9.1/src/brevitas/core/scaling/
+-rw-rw-rw-   0        0        0      571 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/scaling/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/scaling/int_scaling.py
+-rw-rw-rw-   0        0        0    10521 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/scaling/pre_scaling.py
+-rw-rw-rw-   0        0        0     5412 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/scaling/runtime.py
+-rw-rw-rw-   0        0        0    14748 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/scaling/standalone.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.041697 brevitas-0.9.1/src/brevitas/core/stats/
+-rw-rw-rw-   0        0        0      829 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/stats/__init__.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 11:23:51.000000 brevitas-0.9.1/src/brevitas/core/stats/stats_op.py
+-rw-rw-rw-   0        0        0     4500 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/stats/stats_wrapper.py
+-rw-rw-rw-   0        0        0     2699 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/stats/view_wrapper.py
+-rw-rw-rw-   0        0        0     2523 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/utils.py
+-rw-rw-rw-   0        0        0     9053 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/core/zero_point.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.045223 brevitas-0.9.1/src/brevitas/csrc/
+-rw-rw-rw-   0        0        0     7051 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/csrc/autograd_ste_ops.cpp
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.052220 brevitas-0.9.1/src/brevitas/export/
+-rw-rw-rw-   0        0        0     1363 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.055221 brevitas-0.9.1/src/brevitas/export/common/
+-rw-rw-rw-   0        0        0      425 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.063736 brevitas-0.9.1/src/brevitas/export/common/handler/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/common/handler/__init__.py
+-rw-rw-rw-   0        0        0     5533 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/common/handler/base.py
+-rw-rw-rw-   0        0        0    12025 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/export/common/handler/qcdq.py
+-rw-rw-rw-   0        0        0    11884 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.080258 brevitas-0.9.1/src/brevitas/export/onnx/
+-rw-rw-rw-   0        0        0      472 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/__init__.py
+-rw-rw-rw-   0        0        0     1935 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/debug.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.092775 brevitas-0.9.1/src/brevitas/export/onnx/finn/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.104775 brevitas-0.9.1/src/brevitas/export/onnx/finn/function/
+-rw-rw-rw-   0        0        0      154 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/function/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/function/acc.py
+-rw-rw-rw-   0        0        0     1347 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/function/act.py
+-rw-rw-rw-   0        0        0     2607 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/function/parameter.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.121293 brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/__init__.py
+-rw-rw-rw-   0        0        0     2163 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/acc.py
+-rw-rw-rw-   0        0        0     5692 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/act.py
+-rw-rw-rw-   0        0        0     3096 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/base.py
+-rw-rw-rw-   0        0        0     6371 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/parameter.py
+-rw-rw-rw-   0        0        0     5803 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/manager.py
+-rw-rw-rw-   0        0        0     2138 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/transform.py
+-rw-rw-rw-   0        0        0      586 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/finn/utils.py
+-rw-rw-rw-   0        0        0     1805 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/function.py
+-rw-rw-rw-   0        0        0    10476 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/handler.py
+-rw-rw-rw-   0        0        0     6871 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.132291 brevitas-0.9.1/src/brevitas/export/onnx/qonnx/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/qonnx/__init__.py
+-rw-rw-rw-   0        0        0    13891 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/qonnx/function.py
+-rw-rw-rw-   0        0        0     6196 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/qonnx/handler.py
+-rw-rw-rw-   0        0        0     2179 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/qonnx/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.142290 brevitas-0.9.1/src/brevitas/export/onnx/standard/
+-rw-rw-rw-   0        0        0      112 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/function.py
+-rw-rw-rw-   0        0        0     1613 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.152291 brevitas-0.9.1/src/brevitas/export/onnx/standard/qcdq/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qcdq/__init__.py
+-rw-rw-rw-   0        0        0     4002 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qcdq/handler.py
+-rw-rw-rw-   0        0        0     2125 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qcdq/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.160805 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/__init__.py
+-rw-rw-rw-   0        0        0     3231 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/function.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.175322 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/
+-rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/__init__.py
+-rw-rw-rw-   0        0        0     5759 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/act.py
+-rw-rw-rw-   0        0        0     7390 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/base.py
+-rw-rw-rw-   0        0        0     8186 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/parameter.py
+-rw-rw-rw-   0        0        0     1370 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.812634 brevitas-0.9.1/src/brevitas/export/torch/
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.184321 brevitas-0.9.1/src/brevitas/export/torch/qcdq/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qcdq/__init__.py
+-rw-rw-rw-   0        0        0     4304 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qcdq/handler.py
+-rw-rw-rw-   0        0        0     1361 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qcdq/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.192321 brevitas-0.9.1/src/brevitas/export/torch/qoperator/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.207322 brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/
+-rw-rw-rw-   0        0        0      213 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/act.py
+-rw-rw-rw-   0        0        0     2373 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/base.py
+-rw-rw-rw-   0        0        0     4781 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/parameter.py
+-rw-rw-rw-   0        0        0     1812 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/pool.py
+-rw-rw-rw-   0        0        0     2509 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/export/torch/qoperator/manager.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.219852 brevitas-0.9.1/src/brevitas/function/
+-rw-rw-rw-   0        0        0      155 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/function/__init__.py
+-rw-rw-rw-   0        0        0     5513 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/function/ops.py
+-rw-rw-rw-   0        0        0    13010 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/function/ops_ste.py
+-rw-rw-rw-   0        0        0     2314 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/function/shape.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.228851 brevitas-0.9.1/src/brevitas/fx/
+-rw-rw-rw-   0        0        0     3549 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.260886 brevitas-0.9.1/src/brevitas/fx/backport/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/__init__.py
+-rw-rw-rw-   0        0        0    39947 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/graph.py
+-rw-rw-rw-   0        0        0    17454 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/graph_module.py
+-rw-rw-rw-   0        0        0     3427 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/immutable_collections.py
+-rw-rw-rw-   0        0        0    18108 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/interpreter.py
+-rw-rw-rw-   0        0        0    14017 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/node.py
+-rw-rw-rw-   0        0        0    11952 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/proxy.py
+-rw-rw-rw-   0        0        0    16627 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/subgraph_rewriter.py
+-rw-rw-rw-   0        0        0    28505 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/symbolic_trace.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.274401 brevitas-0.9.1/src/brevitas/fx/backport/torch_function/
+-rw-rw-rw-   0        0        0      190 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/torch_function/__init__.py
+-rw-rw-rw-   0        0        0     7731 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/torch_function/_overrides.py
+-rw-rw-rw-   0        0        0     4319 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/torch_function/patch.py
+-rw-rw-rw-   0        0        0    61914 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/backport/torch_function/signatures.py
+-rw-rw-rw-   0        0        0     2274 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/brevitas_tracer.py
+-rw-rw-rw-   0        0        0    21509 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/fx/value_tracer.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.308446 brevitas-0.9.1/src/brevitas/graph/
+-rw-rw-rw-   0        0        0      261 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/__init__.py
+-rw-rw-rw-   0        0        0    10632 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/base.py
+-rw-rw-rw-   0        0        0    11684 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/calibrate.py
+-rw-rw-rw-   0        0        0    20501 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/equalize.py
+-rw-rw-rw-   0        0        0     8309 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/fixed_point.py
+-rw-rw-rw-   0        0        0     5021 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/per_input.py
+-rw-rw-rw-   0        0        0    13412 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/graph/quantize.py
+-rw-rw-rw-   0        0        0    19261 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/graph/quantize_impl.py
+-rw-rw-rw-   0        0        0     5927 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/standardize.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.314442 brevitas-0.9.1/src/brevitas/graph/target/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/target/__init__.py
+-rw-rw-rw-   0        0        0     6919 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/graph/target/flexml.py
+-rw-rw-rw-   0        0        0     4880 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/graph/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.323960 brevitas-0.9.1/src/brevitas/inject/
+-rw-rw-rw-   0        0        0     7787 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/inject/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/inject/defaults.py
+-rw-rw-rw-   0        0        0     1451 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/inject/enum.py
+-rw-rw-rw-   0        0        0      788 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/jit.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.331959 brevitas-0.9.1/src/brevitas/loss/
+-rw-rw-rw-   0        0        0      346 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/loss/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/loss/base_loss.py
+-rw-rw-rw-   0        0        0     3790 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/loss/weighted_bit_width.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.392997 brevitas-0.9.1/src/brevitas/nn/
+-rw-rw-rw-   0        0        0     1516 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/__init__.py
+-rw-rw-rw-   0        0        0     3439 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/hadamard_classifier.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.411997 brevitas-0.9.1/src/brevitas/nn/mixin/
+-rw-rw-rw-   0        0        0      468 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/mixin/__init__.py
+-rw-rw-rw-   0        0        0     1919 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/mixin/acc.py
+-rw-rw-rw-   0        0        0     4085 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/mixin/act.py
+-rw-rw-rw-   0        0        0    12643 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/mixin/base.py
+-rw-rw-rw-   0        0        0     7083 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/mixin/parameter.py
+-rw-rw-rw-   0        0        0      261 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/mixin/utils.py
+-rw-rw-rw-   0        0        0     1828 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_accumulator.py
+-rw-rw-rw-   0        0        0     3013 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_activation.py
+-rw-rw-rw-   0        0        0     5880 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_avg_pool.py
+-rw-rw-rw-   0        0        0     3823 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_bn.py
+-rw-rw-rw-   0        0        0     8226 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_conv.py
+-rw-rw-rw-   0        0        0     8260 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_convtranspose.py
+-rw-rw-rw-   0        0        0      871 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_dropout.py
+-rw-rw-rw-   0        0        0     3122 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_eltwise.py
+-rw-rw-rw-   0        0        0     2485 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_embedding.py
+-rw-rw-rw-   0        0        0    12986 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_layer.py
+-rw-rw-rw-   0        0        0     2519 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_linear.py
+-rw-rw-rw-   0        0        0     2457 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_max_pool.py
+-rw-rw-rw-   0        0        0    36694 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_mha.py
+-rw-rw-rw-   0        0        0    40303 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_rnn.py
+-rw-rw-rw-   0        0        0     3077 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_scale_bias.py
+-rw-rw-rw-   0        0        0     3627 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/quant_upsample.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.417997 brevitas-0.9.1/src/brevitas/nn/target/
+-rw-rw-rw-   0        0        0      195 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/target/__init__.py
+-rw-rw-rw-   0        0        0     5852 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/target/flexml.py
+-rw-rw-rw-   0        0        0     6092 2023-04-21 17:11:25.000000 brevitas-0.9.1/src/brevitas/nn/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.420997 brevitas-0.9.1/src/brevitas/onnx/
+-rw-rw-rw-   0        0        0      452 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/onnx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.426998 brevitas-0.9.1/src/brevitas/ops/
+-rw-rw-rw-   0        0        0      418 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/ops/__init__.py
+-rw-rw-rw-   0        0        0    14701 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/ops/autograd_ste_ops.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.442997 brevitas-0.9.1/src/brevitas/proxy/
+-rw-rw-rw-   0        0        0      533 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/proxy/__init__.py
+-rw-rw-rw-   0        0        0     7483 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/proxy/parameter_quant.py
+-rw-rw-rw-   0        0        0     4943 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/proxy/quant_proxy.py
+-rw-rw-rw-   0        0        0     7804 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/proxy/runtime_quant.py
+-rw-rw-rw-   0        0        0     1572 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.469039 brevitas-0.9.1/src/brevitas/quant/
+-rw-rw-rw-   0        0        0      265 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/__init__.py
+-rw-rw-rw-   0        0        0    15008 2023-04-28 11:25:40.000000 brevitas-0.9.1/src/brevitas/quant/base.py
+-rw-rw-rw-   0        0        0     1237 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/binary.py
+-rw-rw-rw-   0        0        0     6619 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/fixed_point.py
+-rw-rw-rw-   0        0        0     1289 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/none.py
+-rw-rw-rw-   0        0        0    13323 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/scaled_int.py
+-rw-rw-rw-   0        0        0     3144 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/quant/shifted_scaled_int.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.493577 brevitas-0.9.1/src/brevitas/quant/solver/
+-rw-rw-rw-   0        0        0      289 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/__init__.py
+-rw-rw-rw-   0        0        0     5181 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/act.py
+-rw-rw-rw-   0        0        0     3591 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/bias.py
+-rw-rw-rw-   0        0        0     2208 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/clamp.py
+-rw-rw-rw-   0        0        0     6661 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/quant/solver/common.py
+-rw-rw-rw-   0        0        0     4509 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/parameter.py
+-rw-rw-rw-   0        0        0     1491 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/trunc.py
+-rw-rw-rw-   0        0        0     4168 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/solver/weight.py
+-rw-rw-rw-   0        0        0     1416 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant/ternary.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.500577 brevitas-0.9.1/src/brevitas/quant_tensor/
+-rw-rw-rw-   0        0        0    17983 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/quant_tensor/__init__.py
+-rw-rw-rw-   0        0        0     4117 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas/quant_tensor/torch_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.520092 brevitas-0.9.1/src/brevitas/utils/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/utils/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/utils/jit_utils.py
+-rw-rw-rw-   0        0        0     1668 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/utils/logging.py
+-rw-rw-rw-   0        0        0      914 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/utils/python_utils.py
+-rw-rw-rw-   0        0        0     1836 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/utils/quant_utils.py
+-rw-rw-rw-   0        0        0      901 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:09.950669 brevitas-0.9.1/src/brevitas.egg-info/
+-rw-rw-rw-   0        0        0     4754 2023-04-28 16:55:07.000000 brevitas-0.9.1/src/brevitas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13900 2023-04-28 16:55:09.000000 brevitas-0.9.1/src/brevitas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:55:07.000000 brevitas-0.9.1/src/brevitas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      699 2023-04-28 16:55:07.000000 brevitas-0.9.1/src/brevitas.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-01-10 09:14:58.000000 brevitas-0.9.1/src/brevitas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      726 2023-04-28 16:55:07.000000 brevitas-0.9.1/src/brevitas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-28 16:55:07.000000 brevitas-0.9.1/src/brevitas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.525093 brevitas-0.9.1/src/brevitas_examples/
+-rw-rw-rw-   0        0        0      413 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/README.md
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.540633 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/
+-rw-rw-rw-   0        0        0     2972 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/README.md
+-rw-rw-rw-   0        0        0      330 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/bnn_pynq_train.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.578547 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/
+-rw-rw-rw-   0        0        0      112 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/__init__.py
+-rw-rw-rw-   0        0        0      337 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/cnv_1w1a.ini
+-rw-rw-rw-   0        0        0      337 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/cnv_1w2a.ini
+-rw-rw-rw-   0        0        0      337 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/cnv_2w2a.ini
+-rw-rw-rw-   0        0        0      364 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/lfc_1w1a.ini
+-rw-rw-rw-   0        0        0      364 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/lfc_1w2a.ini
+-rw-rw-rw-   0        0        0      210 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/resnet18_4w4a.ini
+-rw-rw-rw-   0        0        0      361 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/sfc_1w1a.ini
+-rw-rw-rw-   0        0        0      361 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/sfc_1w2a.ini
+-rw-rw-rw-   0        0        0      361 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/sfc_2w2a.ini
+-rw-rw-rw-   0        0        0      358 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/tfc_1w1a.ini
+-rw-rw-rw-   0        0        0      358 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/tfc_1w2a.ini
+-rw-rw-rw-   0        0        0      358 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/cfg/tfc_2w2a.ini
+-rw-rw-rw-   0        0        0     3318 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.601543 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/
+-rw-rw-rw-   0        0        0     4226 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/CNV.py
+-rw-rw-rw-   0        0        0     3032 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/FC.py
+-rw-rw-rw-   0        0        0     2519 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/__init__.py
+-rw-rw-rw-   0        0        0     1346 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/common.py
+-rw-rw-rw-   0        0        0     1100 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/losses.py
+-rw-rw-rw-   0        0        0     7535 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/resnet.py
+-rw-rw-rw-   0        0        0     1468 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/tensor_norm.py
+-rw-rw-rw-   0        0        0    13286 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/bnn_pynq/trainer.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.609547 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/
+-rw-rw-rw-   0        0        0     1735 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/README.md
+-rw-rw-rw-   0        0        0      135 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.629543 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/
+-rw-rw-rw-   0        0        0     2464 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/README.md
+-rw-rw-rw-   0        0        0     3318 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.652543 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/
+-rw-rw-rw-   0        0        0        0 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/__init__.py
+-rw-rw-rw-   0        0        0      199 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_mobilenet_v1.ini
+-rw-rw-rw-   0        0        0      438 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_mobilenet_v1_4b.ini
+-rw-rw-rw-   0        0        0      437 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_mobilenet_v1_4b_round_avgpool.ini
+-rw-rw-rw-   0        0        0      524 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b.ini
+-rw-rw-rw-   0        0        0      528 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b5b.ini
+-rw-rw-rw-   0        0        0      523 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b_round_avgpool.ini
+-rw-rw-rw-   0        0        0      542 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_hadamard_4b.ini
+-rw-rw-rw-   0        0        0     1387 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/common.py
+-rw-rw-rw-   0        0        0     6859 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/mobilenetv1.py
+-rw-rw-rw-   0        0        0    11786 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/proxylessnas.py
+-rw-rw-rw-   0        0        0     6268 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/vgg.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.679543 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/
+-rw-rw-rw-   0        0        0    11104 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/README.md
+-rw-rw-rw-   0        0        0      325 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/RESULTS_IMGCLSMOB.csv
+-rw-rw-rw-   0        0        0    76880 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION.csv
+-rw-rw-rw-   0        0        0     8983 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv
+-rw-rw-rw-   0        0        0    12900 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/ptq_benchmark.py
+-rw-rw-rw-   0        0        0     7437 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/ptq_common.py
+-rw-rw-rw-   0        0        0     9803 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py
+-rw-rw-rw-   0        0        0     1676 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.689543 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/qat/
+-rw-rw-rw-   0        0        0     2973 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/qat/README.md
+-rw-rw-rw-   0        0        0      112 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/qat/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/qat/imagenet_val.py
+-rw-rw-rw-   0        0        0     3697 2023-04-28 11:25:31.000000 brevitas-0.9.1/src/brevitas_examples/imagenet_classification/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.702543 brevitas-0.9.1/src/brevitas_examples/speech_to_text/
+-rw-rw-rw-   0        0        0     3069 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/README.md
+-rw-rw-rw-   0        0        0      138 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.713547 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/
+-rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/__init__.py
+-rw-rw-rw-   0        0        0      601 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_4b.ini
+-rw-rw-rw-   0        0        0      603 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_8b.ini
+-rw-rw-rw-   0        0        0      602 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_pertensorscaling_8b.ini
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.719543 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/topology/
+-rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/topology/__init__.py
+-rw-rw-rw-   0        0        0     3475 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/topology/quartznet15x5.yaml
+-rw-rw-rw-   0        0        0     5304 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/get_librispeech_data.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.745542 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/
+-rw-rw-rw-   0        0        0     3172 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/__init__.py
+-rw-rw-rw-   0        0        0    19330 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/audio_preprocessing.py
+-rw-rw-rw-   0        0        0     5995 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/data_layer.py
+-rw-rw-rw-   0        0        0     1105 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/greedy_ctc_decoder.py
+-rw-rw-rw-   0        0        0     7802 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/helpers.py
+-rw-rw-rw-   0        0        0     1818 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/losses.py
+-rw-rw-rw-   0        0        0     2634 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.778541 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/
+-rw-rw-rw-   0        0        0      961 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/__init__.py
+-rw-rw-rw-   0        0        0     6487 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/cleaners.py
+-rw-rw-rw-   0        0        0     3501 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/common.py
+-rw-rw-rw-   0        0        0     7744 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/dataset.py
+-rw-rw-rw-   0        0        0    11831 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/features.py
+-rw-rw-rw-   0        0        0     7658 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/manifest.py
+-rw-rw-rw-   0        0        0     6652 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/perturb.py
+-rw-rw-rw-   0        0        0    20949 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/quartznet.py
+-rw-rw-rw-   0        0        0     8321 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/segment.py
+-rw-rw-rw-   0        0        0     3634 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/spectr_augment.py
+-rw-rw-rw-   0        0        0    11990 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/quartznet.py
+-rw-rw-rw-   0        0        0     3823 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet_val.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.790547 brevitas-0.9.1/src/brevitas_examples/text_to_speech/
+-rw-rw-rw-   0        0        0     2193 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/README.md
+-rw-rw-rw-   0        0        0      135 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.796544 brevitas-0.9.1/src/brevitas_examples/text_to_speech/cfg/
+-rw-rw-rw-   0        0        0        0 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/cfg/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/cfg/quant_melgan_8b.ini
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.812545 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/
+-rw-rw-rw-   0        0        0      946 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/__init__.py
+-rw-rw-rw-   0        0        0     4942 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/common.py
+-rw-rw-rw-   0        0        0     4914 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/generator_brevitas.py
+-rw-rw-rw-   0        0        0     1959 2023-01-10 09:12:32.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/melgan.py
+-rw-rw-rw-   0        0        0     3588 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/res_stack_brevitas.py
+-rw-rw-rw-   0        0        0     1969 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan_val.py
+-rw-rw-rw-   0        0        0     2403 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/preprocess_dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:55:10.822543 brevitas-0.9.1/src/brevitas_examples/text_to_speech/utilities/
+-rw-rw-rw-   0        0        0       73 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/utilities/__init__.py
+-rw-rw-rw-   0        0        0     4614 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/utilities/audio_processing.py
+-rw-rw-rw-   0        0        0     8078 2023-04-21 17:11:26.000000 brevitas-0.9.1/src/brevitas_examples/text_to_speech/utilities/stft.py
```

### Comparing `brevitas-0.9.0/.pre-commit-config.yaml` & `brevitas-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/LICENSE` & `brevitas-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/PKG-INFO` & `brevitas-0.9.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,65 @@
-Metadata-Version: 2.1
-Name: brevitas
-Version: 0.9.0
-Summary: Quantization-aware training in PyTorch
-Home-page: https://github.com/Xilinx/brevitas
-Author: Alessandro Pappalardo
-Author-email: alessand@xilinx.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: notebook
-Provides-Extra: docs
-Provides-Extra: export
-Provides-Extra: hadamard
-Provides-Extra: test
-Provides-Extra: tts
-Provides-Extra: stt
-Provides-Extra: vision
-Provides-Extra: finn_integration
-Provides-Extra: ort_integration
-License-File: LICENSE
-
-# Brevitas
-
-[![Downloads](https://pepy.tech/badge/brevitas)](https://pepy.tech/project/brevitas)
-[![Gitter](https://badges.gitter.im/xilinx-brevitas/community.svg)](https://gitter.im/xilinx-brevitas/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-![Pytest](https://github.com/Xilinx/brevitas/workflows/Pytest/badge.svg?branch=master)
-![Examples Pytest](https://github.com/Xilinx/brevitas/workflows/Examples%20Pytest/badge.svg?branch=master)
-[![DOI](https://zenodo.org/badge/140494324.svg)](https://zenodo.org/badge/latestdoi/140494324)
-
-Brevitas is a PyTorch library for neural network quantization, with support for both *post-training quantization (PTQ)* and *quantization-aware training (QAT)*.
-
-**Please note that Brevitas is a research project and not an official Xilinx product.**
-
-If you like this project please consider ⭐ this repo, as it is the simplest and best way to support it.
-
-If you have issues, comments, or are just looking for advices on training quantized neural networks, open an issue or a discussion.
-
-## Cite as
-
-If you adopt Brevitas in your work, please cite it as:
-```
-@software{brevitas,
-  author       = {Alessandro Pappalardo},
-  title        = {Xilinx/brevitas},
-  year         = {2022},
-  publisher    = {Zenodo},
-  doi          = {10.5281/zenodo.3333552},
-  url          = {https://doi.org/10.5281/zenodo.3333552}
-}
-```
-
-
-## History
-
-- *2023/04/21* - Release version 0.9.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.9.0).
-- *2023/01/10* - Release version 0.8.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.8.0).
-- *2021/12/13* - Release version 0.7.1, fix a bunch of issues. Added TVMCon 2021 tutorial notebook.
-- *2021/11/03* - Re-release version 0.7.0 (build 1) on PyPI to fix a packaging issue.
-- *2021/10/29* - Release version 0.7.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.7.0).
-- *2021/06/04* - Release version 0.6.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.6.0).
-- *2021/05/24* - Release version 0.5.1, fix a bunch of minor issues. See [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.1).
-- *2021/05/06* - Release version 0.5.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.0).
-- *2021/03/15* - Release version 0.4.0, add support for \_\_torch_function\_\_ to QuantTensor.
-- *2021/03/04* - Release version 0.3.1, fix bug w/ act initialization from statistics w/ IGNORE_MISSING_KEYS=1.
-- *2021/03/01* - Release version 0.3.0, implements enum and shape solvers within extended dependency injectors. This allows declarative quantizers to be self-contained.
-- *2021/02/04* - Release version 0.2.1, includes various bugfixes of QuantTensor w/ zero-point.
-- *2021/01/30* - First release version 0.2.0 on PyPI.
-
-## Requirements
-
-* Python >= 3.7 .
-* [Pytorch](https://pytorch.org) >= 1.5.1 .
-* Windows, Linux or macOS.
-* GPU training-time acceleration (*Optional* but recommended).
-
-## Installation
-
-You can install the latest release from PyPI:
-```bash
-pip install brevitas
-```
-
-## Getting started
-
-Check out available info at https://xilinx.github.io/brevitas/getting_started .
+# Brevitas
+
+[![Downloads](https://pepy.tech/badge/brevitas)](https://pepy.tech/project/brevitas)
+![Pytest](https://github.com/Xilinx/brevitas/workflows/Pytest/badge.svg?branch=master)
+![Examples Pytest](https://github.com/Xilinx/brevitas/workflows/Examples%20Pytest/badge.svg?branch=master)
+[![DOI](https://zenodo.org/badge/140494324.svg)](https://zenodo.org/badge/latestdoi/140494324)
+
+Brevitas is a PyTorch library for neural network quantization, with support for both *post-training quantization (PTQ)* and *quantization-aware training (QAT)*.
+
+**Please note that Brevitas is a research project and not an official Xilinx product.**
+
+If you like this project please consider ⭐ this repo, as it is the simplest and best way to support it.
+
+## Requirements
+
+* Python >= 3.7 .
+* [Pytorch](https://pytorch.org) >= 1.5.1 .
+* Windows, Linux or macOS.
+* GPU training-time acceleration (*Optional* but recommended).
+
+## Installation
+
+You can install the latest release from PyPI:
+```bash
+pip install brevitas
+```
+
+## Getting Started
+
+Brevitas currently offers quantized implementations of the most common PyTorch layers used in DNN under `brevitas.nn`, such as `QuantConv1d`, `QuantConv2d`, `QuantConvTranspose1d`, `QuantConvTranspose2d`, `QuantMultiheadAttention`, `QuantRNN`, `QuantLSTM` etc., for adoption within PTQ and/or QAT.
+For each one of these layers, quantization of different tensors (inputs, weights, bias, outputs, etc) can be individually tuned according to a wide range of quantization settings.
+
+As a reference for PTQ, Brevitas provides an example user flow for ImageNet classification models under [`brevitas_examples.imagenet_classification.ptq`](https://github.com/Xilinx/brevitas/blob/master/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py) that quantizes an input torchvision model using PTQ under different quantization configurations (e.g. bit-width, granularity of scale, etc). Sample accuracy results are available [here](https://github.com/Xilinx/brevitas/blob/master/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv) for a selection of three reference topologies (ResNet18, MobileNet V2, ViT), under a variety of different quantization settings.
+
+For more info, checkout https://xilinx.github.io/brevitas/getting_started .
+
+## Cite as
+
+If you adopt Brevitas in your work, please cite it as:
+```
+@software{brevitas,
+  author       = {Alessandro Pappalardo},
+  title        = {Xilinx/brevitas},
+  year         = {2022},
+  publisher    = {Zenodo},
+  doi          = {10.5281/zenodo.3333552},
+  url          = {https://doi.org/10.5281/zenodo.3333552}
+}
+```
+
+## History
+
+- *2023/04/21* - Release version 0.9.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.9.0).
+- *2023/01/10* - Release version 0.8.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.8.0).
+- *2021/12/13* - Release version 0.7.1, fix a bunch of issues. Added TVMCon 2021 tutorial notebook.
+- *2021/11/03* - Re-release version 0.7.0 (build 1) on PyPI to fix a packaging issue.
+- *2021/10/29* - Release version 0.7.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.7.0).
+- *2021/06/04* - Release version 0.6.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.6.0).
+- *2021/05/24* - Release version 0.5.1, fix a bunch of minor issues. See [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.1).
+- *2021/05/06* - Release version 0.5.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.0).
+- *2021/03/15* - Release version 0.4.0, add support for \_\_torch_function\_\_ to QuantTensor.
+- *2021/03/04* - Release version 0.3.1, fix bug w/ act initialization from statistics w/ IGNORE_MISSING_KEYS=1.
+- *2021/03/01* - Release version 0.3.0, implements enum and shape solvers within extended dependency injectors. This allows declarative quantizers to be self-contained.
+- *2021/02/04* - Release version 0.2.1, includes various bugfixes of QuantTensor w/ zero-point.
+- *2021/01/30* - First release version 0.2.0 on PyPI.
```

### Comparing `brevitas-0.9.0/README.md` & `brevitas-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,87 @@
-# Brevitas
-
-[![Downloads](https://pepy.tech/badge/brevitas)](https://pepy.tech/project/brevitas)
-[![Gitter](https://badges.gitter.im/xilinx-brevitas/community.svg)](https://gitter.im/xilinx-brevitas/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-![Pytest](https://github.com/Xilinx/brevitas/workflows/Pytest/badge.svg?branch=master)
-![Examples Pytest](https://github.com/Xilinx/brevitas/workflows/Examples%20Pytest/badge.svg?branch=master)
-[![DOI](https://zenodo.org/badge/140494324.svg)](https://zenodo.org/badge/latestdoi/140494324)
-
-Brevitas is a PyTorch library for neural network quantization, with support for both *post-training quantization (PTQ)* and *quantization-aware training (QAT)*.
-
-**Please note that Brevitas is a research project and not an official Xilinx product.**
-
-If you like this project please consider ⭐ this repo, as it is the simplest and best way to support it.
-
-If you have issues, comments, or are just looking for advices on training quantized neural networks, open an issue or a discussion.
-
-## Cite as
-
-If you adopt Brevitas in your work, please cite it as:
-```
-@software{brevitas,
-  author       = {Alessandro Pappalardo},
-  title        = {Xilinx/brevitas},
-  year         = {2022},
-  publisher    = {Zenodo},
-  doi          = {10.5281/zenodo.3333552},
-  url          = {https://doi.org/10.5281/zenodo.3333552}
-}
-```
-
-
-## History
-
-- *2023/04/21* - Release version 0.9.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.9.0).
-- *2023/01/10* - Release version 0.8.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.8.0).
-- *2021/12/13* - Release version 0.7.1, fix a bunch of issues. Added TVMCon 2021 tutorial notebook.
-- *2021/11/03* - Re-release version 0.7.0 (build 1) on PyPI to fix a packaging issue.
-- *2021/10/29* - Release version 0.7.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.7.0).
-- *2021/06/04* - Release version 0.6.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.6.0).
-- *2021/05/24* - Release version 0.5.1, fix a bunch of minor issues. See [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.1).
-- *2021/05/06* - Release version 0.5.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.0).
-- *2021/03/15* - Release version 0.4.0, add support for \_\_torch_function\_\_ to QuantTensor.
-- *2021/03/04* - Release version 0.3.1, fix bug w/ act initialization from statistics w/ IGNORE_MISSING_KEYS=1.
-- *2021/03/01* - Release version 0.3.0, implements enum and shape solvers within extended dependency injectors. This allows declarative quantizers to be self-contained.
-- *2021/02/04* - Release version 0.2.1, includes various bugfixes of QuantTensor w/ zero-point.
-- *2021/01/30* - First release version 0.2.0 on PyPI.
-
-## Requirements
-
-* Python >= 3.7 .
-* [Pytorch](https://pytorch.org) >= 1.5.1 .
-* Windows, Linux or macOS.
-* GPU training-time acceleration (*Optional* but recommended).
-
-## Installation
-
-You can install the latest release from PyPI:
-```bash
-pip install brevitas
-```
-
-## Getting started
-
-Check out available info at https://xilinx.github.io/brevitas/getting_started .
+Metadata-Version: 2.1
+Name: brevitas
+Version: 0.9.1
+Summary: Quantization-aware training in PyTorch
+Home-page: https://github.com/Xilinx/brevitas
+Author: Alessandro Pappalardo
+Author-email: alessand@amd.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: notebook
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: export
+Provides-Extra: hadamard
+Provides-Extra: test
+Provides-Extra: tts
+Provides-Extra: stt
+Provides-Extra: vision
+Provides-Extra: finn_integration
+Provides-Extra: ort_integration
+License-File: LICENSE
+
+# Brevitas
+
+[![Downloads](https://pepy.tech/badge/brevitas)](https://pepy.tech/project/brevitas)
+![Pytest](https://github.com/Xilinx/brevitas/workflows/Pytest/badge.svg?branch=master)
+![Examples Pytest](https://github.com/Xilinx/brevitas/workflows/Examples%20Pytest/badge.svg?branch=master)
+[![DOI](https://zenodo.org/badge/140494324.svg)](https://zenodo.org/badge/latestdoi/140494324)
+
+Brevitas is a PyTorch library for neural network quantization, with support for both *post-training quantization (PTQ)* and *quantization-aware training (QAT)*.
+
+**Please note that Brevitas is a research project and not an official Xilinx product.**
+
+If you like this project please consider ⭐ this repo, as it is the simplest and best way to support it.
+
+## Requirements
+
+* Python >= 3.7 .
+* [Pytorch](https://pytorch.org) >= 1.5.1 .
+* Windows, Linux or macOS.
+* GPU training-time acceleration (*Optional* but recommended).
+
+## Installation
+
+You can install the latest release from PyPI:
+```bash
+pip install brevitas
+```
+
+## Getting Started
+
+Brevitas currently offers quantized implementations of the most common PyTorch layers used in DNN under `brevitas.nn`, such as `QuantConv1d`, `QuantConv2d`, `QuantConvTranspose1d`, `QuantConvTranspose2d`, `QuantMultiheadAttention`, `QuantRNN`, `QuantLSTM` etc., for adoption within PTQ and/or QAT.
+For each one of these layers, quantization of different tensors (inputs, weights, bias, outputs, etc) can be individually tuned according to a wide range of quantization settings.
+
+As a reference for PTQ, Brevitas provides an example user flow for ImageNet classification models under [`brevitas_examples.imagenet_classification.ptq`](https://github.com/Xilinx/brevitas/blob/master/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py) that quantizes an input torchvision model using PTQ under different quantization configurations (e.g. bit-width, granularity of scale, etc). Sample accuracy results are available [here](https://github.com/Xilinx/brevitas/blob/master/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv) for a selection of three reference topologies (ResNet18, MobileNet V2, ViT), under a variety of different quantization settings.
+
+For more info, checkout https://xilinx.github.io/brevitas/getting_started .
+
+## Cite as
+
+If you adopt Brevitas in your work, please cite it as:
+```
+@software{brevitas,
+  author       = {Alessandro Pappalardo},
+  title        = {Xilinx/brevitas},
+  year         = {2022},
+  publisher    = {Zenodo},
+  doi          = {10.5281/zenodo.3333552},
+  url          = {https://doi.org/10.5281/zenodo.3333552}
+}
+```
+
+## History
+
+- *2023/04/21* - Release version 0.9.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.9.0).
+- *2023/01/10* - Release version 0.8.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.8.0).
+- *2021/12/13* - Release version 0.7.1, fix a bunch of issues. Added TVMCon 2021 tutorial notebook.
+- *2021/11/03* - Re-release version 0.7.0 (build 1) on PyPI to fix a packaging issue.
+- *2021/10/29* - Release version 0.7.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.7.0).
+- *2021/06/04* - Release version 0.6.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.6.0).
+- *2021/05/24* - Release version 0.5.1, fix a bunch of minor issues. See [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.1).
+- *2021/05/06* - Release version 0.5.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.0).
+- *2021/03/15* - Release version 0.4.0, add support for \_\_torch_function\_\_ to QuantTensor.
+- *2021/03/04* - Release version 0.3.1, fix bug w/ act initialization from statistics w/ IGNORE_MISSING_KEYS=1.
+- *2021/03/01* - Release version 0.3.0, implements enum and shape solvers within extended dependency injectors. This allows declarative quantizers to be self-contained.
+- *2021/02/04* - Release version 0.2.1, includes various bugfixes of QuantTensor w/ zero-point.
+- *2021/01/30* - First release version 0.2.0 on PyPI.
```

### Comparing `brevitas-0.9.0/notebooks/01_quant_tensor_quant_conv2d_overview.ipynb` & `brevitas-0.9.1/notebooks/01_quant_tensor_quant_conv2d_overview.ipynb`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/notebooks/02_quant_activation_overview.ipynb` & `brevitas-0.9.1/notebooks/02_quant_activation_overview.ipynb`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/notebooks/03_anatomy_of_a_quantizer.ipynb` & `brevitas-0.9.1/notebooks/03_anatomy_of_a_quantizer.ipynb`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/notebooks/Brevitas_TVMCon2021.ipynb` & `brevitas-0.9.1/notebooks/Brevitas_TVMCon2021.ipynb`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/notebooks/ONNX_export_tutorial.ipynb` & `brevitas-0.9.1/notebooks/ONNX_export_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/notebooks/quantized_recurrent.ipynb` & `brevitas-0.9.1/notebooks/quantized_recurrent.ipynb`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/setup.py` & `brevitas-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,22 @@
     name="brevitas",
     use_scm_version=True,
     setup_requires=read_requirements('requirements-setup.txt'),
     description="Quantization-aware training in PyTorch",
     long_description=read(PROJECT_ROOT, 'README.md'),
     long_description_content_type="text/markdown",
     author="Alessandro Pappalardo",
-    author_email="alessand@xilinx.com",
+    author_email="alessand@amd.com",
     url="https://github.com/Xilinx/brevitas",
     python_requires=">=3.7",
     install_requires=read_requirements('requirements.txt'),
     extras_require={
         "notebook": read_requirements('requirements-notebook.txt'),
-        "docs": read_requirements("requirements-docs.txt"),
+        "dev": read_requirements('requirements-dev.txt'),
+        "docs": read_requirements('requirements-docs.txt'),
         "export": read_requirements('requirements-export.txt'),
         "hadamard": read_requirements('requirements-hadamard.txt'),
         "test": read_requirements('requirements-test.txt'),
         "tts": read_requirements('requirements-tts.txt'),
         "stt": read_requirements('requirements-stt.txt'),
         "vision": read_requirements('requirements-vision.txt'),
         "finn_integration": read_requirements('requirements-finn-integration.txt'),
```

### Comparing `brevitas-0.9.0/src/brevitas/__init__.py` & `brevitas-0.9.1/src/brevitas/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/common.py` & `brevitas-0.9.1/src/brevitas/common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/config.py` & `brevitas-0.9.1/src/brevitas/config.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/bit_width/const.py` & `brevitas-0.9.1/src/brevitas/core/bit_width/const.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/bit_width/parameter.py` & `brevitas-0.9.1/src/brevitas/core/bit_width/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/function_wrapper/__init__.py` & `brevitas-0.9.1/src/brevitas/core/function_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/function_wrapper/clamp.py` & `brevitas-0.9.1/src/brevitas/core/function_wrapper/clamp.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/function_wrapper/learned_round.py` & `brevitas-0.9.1/src/brevitas/core/function_wrapper/learned_round.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/function_wrapper/misc.py` & `brevitas-0.9.1/src/brevitas/core/function_wrapper/misc.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/function_wrapper/ops_ste.py` & `brevitas-0.9.1/src/brevitas/core/function_wrapper/ops_ste.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/function_wrapper/shape.py` & `brevitas-0.9.1/src/brevitas/core/function_wrapper/shape.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/quant/__init__.py` & `brevitas-0.9.1/src/brevitas/core/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/quant/binary.py` & `brevitas-0.9.1/src/brevitas/core/quant/binary.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/quant/delay.py` & `brevitas-0.9.1/src/brevitas/core/quant/delay.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/quant/int.py` & `brevitas-0.9.1/src/brevitas/core/quant/int.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/quant/int_base.py` & `brevitas-0.9.1/src/brevitas/core/quant/int_base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/quant/ternary.py` & `brevitas-0.9.1/src/brevitas/core/quant/ternary.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/restrict_val.py` & `brevitas-0.9.1/src/brevitas/core/restrict_val.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/scaling/__init__.py` & `brevitas-0.9.1/src/brevitas/core/scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/scaling/int_scaling.py` & `brevitas-0.9.1/src/brevitas/core/scaling/int_scaling.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/scaling/pre_scaling.py` & `brevitas-0.9.1/src/brevitas/core/scaling/pre_scaling.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/scaling/runtime.py` & `brevitas-0.9.1/src/brevitas/core/scaling/runtime.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/scaling/standalone.py` & `brevitas-0.9.1/src/brevitas/core/scaling/standalone.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/stats/__init__.py` & `brevitas-0.9.1/src/brevitas/core/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/stats/stats_op.py` & `brevitas-0.9.1/src/brevitas/core/stats/stats_op.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/stats/stats_wrapper.py` & `brevitas-0.9.1/src/brevitas/core/stats/stats_wrapper.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/stats/view_wrapper.py` & `brevitas-0.9.1/src/brevitas/core/stats/view_wrapper.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/utils.py` & `brevitas-0.9.1/src/brevitas/core/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/core/zero_point.py` & `brevitas-0.9.1/src/brevitas/core/zero_point.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/csrc/autograd_ste_ops.cpp` & `brevitas-0.9.1/src/brevitas/csrc/autograd_ste_ops.cpp`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/__init__.py` & `brevitas-0.9.1/src/brevitas/export/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/common/handler/base.py` & `brevitas-0.9.1/src/brevitas/export/common/handler/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/common/handler/qcdq.py` & `brevitas-0.9.1/src/brevitas/export/common/handler/qcdq.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/manager.py` & `brevitas-0.9.1/src/brevitas/export/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/debug.py` & `brevitas-0.9.1/src/brevitas/export/onnx/debug.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/function/acc.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/function/acc.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/function/act.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/function/act.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/function/parameter.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/function/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/acc.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/acc.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/act.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/act.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/base.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/handler/parameter.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/handler/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/manager.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/transform.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/transform.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/finn/utils.py` & `brevitas-0.9.1/src/brevitas/export/onnx/finn/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/function.py` & `brevitas-0.9.1/src/brevitas/export/onnx/function.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/handler.py` & `brevitas-0.9.1/src/brevitas/export/onnx/handler.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/manager.py` & `brevitas-0.9.1/src/brevitas/export/onnx/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/qonnx/function.py` & `brevitas-0.9.1/src/brevitas/export/onnx/qonnx/function.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/qonnx/handler.py` & `brevitas-0.9.1/src/brevitas/export/onnx/qonnx/handler.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/qonnx/manager.py` & `brevitas-0.9.1/src/brevitas/export/onnx/qonnx/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/function.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/function.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/manager.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qcdq/handler.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qcdq/handler.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qcdq/manager.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qcdq/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/function.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/function.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/act.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/act.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/base.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/parameter.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/handler/pool.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/handler/pool.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/onnx/standard/qoperator/manager.py` & `brevitas-0.9.1/src/brevitas/export/onnx/standard/qoperator/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qcdq/handler.py` & `brevitas-0.9.1/src/brevitas/export/torch/qcdq/handler.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qcdq/manager.py` & `brevitas-0.9.1/src/brevitas/export/torch/qcdq/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/act.py` & `brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/act.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/base.py` & `brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/parameter.py` & `brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qoperator/handler/pool.py` & `brevitas-0.9.1/src/brevitas/export/torch/qoperator/handler/pool.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/export/torch/qoperator/manager.py` & `brevitas-0.9.1/src/brevitas/export/torch/qoperator/manager.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/function/ops.py` & `brevitas-0.9.1/src/brevitas/function/ops.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/function/ops_ste.py` & `brevitas-0.9.1/src/brevitas/function/ops_ste.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/function/shape.py` & `brevitas-0.9.1/src/brevitas/function/shape.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/__init__.py` & `brevitas-0.9.1/src/brevitas/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/graph.py` & `brevitas-0.9.1/src/brevitas/fx/backport/graph.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/graph_module.py` & `brevitas-0.9.1/src/brevitas/fx/backport/graph_module.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/immutable_collections.py` & `brevitas-0.9.1/src/brevitas/fx/backport/immutable_collections.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/interpreter.py` & `brevitas-0.9.1/src/brevitas/fx/backport/interpreter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/node.py` & `brevitas-0.9.1/src/brevitas/fx/backport/node.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/proxy.py` & `brevitas-0.9.1/src/brevitas/fx/backport/proxy.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/subgraph_rewriter.py` & `brevitas-0.9.1/src/brevitas/fx/backport/subgraph_rewriter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/symbolic_trace.py` & `brevitas-0.9.1/src/brevitas/fx/backport/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/torch_function/_overrides.py` & `brevitas-0.9.1/src/brevitas/fx/backport/torch_function/_overrides.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/torch_function/patch.py` & `brevitas-0.9.1/src/brevitas/fx/backport/torch_function/patch.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/backport/torch_function/signatures.py` & `brevitas-0.9.1/src/brevitas/fx/backport/torch_function/signatures.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/brevitas_tracer.py` & `brevitas-0.9.1/src/brevitas/fx/brevitas_tracer.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/fx/value_tracer.py` & `brevitas-0.9.1/src/brevitas/fx/value_tracer.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/base.py` & `brevitas-0.9.1/src/brevitas/graph/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/calibrate.py` & `brevitas-0.9.1/src/brevitas/graph/calibrate.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/equalize.py` & `brevitas-0.9.1/src/brevitas/graph/equalize.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/fixed_point.py` & `brevitas-0.9.1/src/brevitas/graph/fixed_point.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/per_input.py` & `brevitas-0.9.1/src/brevitas/graph/per_input.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/quantize.py` & `brevitas-0.9.1/src/brevitas/graph/quantize.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/quantize_impl.py` & `brevitas-0.9.1/src/brevitas/graph/quantize_impl.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/standardize.py` & `brevitas-0.9.1/src/brevitas/graph/standardize.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/target/flexml.py` & `brevitas-0.9.1/src/brevitas/graph/target/flexml.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/graph/utils.py` & `brevitas-0.9.1/src/brevitas/graph/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/inject/__init__.py` & `brevitas-0.9.1/src/brevitas/inject/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/inject/enum.py` & `brevitas-0.9.1/src/brevitas/inject/enum.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/jit.py` & `brevitas-0.9.1/src/brevitas/jit.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/loss/base_loss.py` & `brevitas-0.9.1/src/brevitas/loss/base_loss.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/loss/weighted_bit_width.py` & `brevitas-0.9.1/src/brevitas/loss/weighted_bit_width.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/__init__.py` & `brevitas-0.9.1/src/brevitas/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/hadamard_classifier.py` & `brevitas-0.9.1/src/brevitas/nn/hadamard_classifier.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/mixin/acc.py` & `brevitas-0.9.1/src/brevitas/nn/mixin/acc.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/mixin/act.py` & `brevitas-0.9.1/src/brevitas/nn/mixin/act.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/mixin/base.py` & `brevitas-0.9.1/src/brevitas/nn/mixin/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/mixin/parameter.py` & `brevitas-0.9.1/src/brevitas/nn/mixin/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_accumulator.py` & `brevitas-0.9.1/src/brevitas/nn/quant_accumulator.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_activation.py` & `brevitas-0.9.1/src/brevitas/nn/quant_activation.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_avg_pool.py` & `brevitas-0.9.1/src/brevitas/nn/quant_avg_pool.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_bn.py` & `brevitas-0.9.1/src/brevitas/nn/quant_bn.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_conv.py` & `brevitas-0.9.1/src/brevitas/nn/quant_conv.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_convtranspose.py` & `brevitas-0.9.1/src/brevitas/nn/quant_convtranspose.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_dropout.py` & `brevitas-0.9.1/src/brevitas/nn/quant_dropout.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_eltwise.py` & `brevitas-0.9.1/src/brevitas/nn/quant_eltwise.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_embedding.py` & `brevitas-0.9.1/src/brevitas/nn/quant_embedding.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_layer.py` & `brevitas-0.9.1/src/brevitas/nn/quant_layer.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_linear.py` & `brevitas-0.9.1/src/brevitas/nn/quant_linear.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_max_pool.py` & `brevitas-0.9.1/src/brevitas/nn/quant_max_pool.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_mha.py` & `brevitas-0.9.1/src/brevitas/nn/quant_mha.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_rnn.py` & `brevitas-0.9.1/src/brevitas/nn/quant_rnn.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_scale_bias.py` & `brevitas-0.9.1/src/brevitas/nn/quant_scale_bias.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/quant_upsample.py` & `brevitas-0.9.1/src/brevitas/nn/quant_upsample.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/target/flexml.py` & `brevitas-0.9.1/src/brevitas/nn/target/flexml.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/nn/utils.py` & `brevitas-0.9.1/src/brevitas/nn/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/ops/autograd_ste_ops.py` & `brevitas-0.9.1/src/brevitas/ops/autograd_ste_ops.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/proxy/__init__.py` & `brevitas-0.9.1/src/brevitas/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/proxy/parameter_quant.py` & `brevitas-0.9.1/src/brevitas/proxy/parameter_quant.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/proxy/quant_proxy.py` & `brevitas-0.9.1/src/brevitas/proxy/quant_proxy.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/proxy/runtime_quant.py` & `brevitas-0.9.1/src/brevitas/proxy/runtime_quant.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/proxy/utils.py` & `brevitas-0.9.1/src/brevitas/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/base.py` & `brevitas-0.9.1/src/brevitas/quant/base.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/binary.py` & `brevitas-0.9.1/src/brevitas/quant/binary.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/fixed_point.py` & `brevitas-0.9.1/src/brevitas/quant/fixed_point.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/none.py` & `brevitas-0.9.1/src/brevitas/quant/none.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/scaled_int.py` & `brevitas-0.9.1/src/brevitas/quant/scaled_int.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/shifted_scaled_int.py` & `brevitas-0.9.1/src/brevitas/quant/shifted_scaled_int.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/act.py` & `brevitas-0.9.1/src/brevitas/quant/solver/act.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/bias.py` & `brevitas-0.9.1/src/brevitas/quant/solver/bias.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/clamp.py` & `brevitas-0.9.1/src/brevitas/quant/solver/clamp.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/common.py` & `brevitas-0.9.1/src/brevitas/quant/solver/common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/parameter.py` & `brevitas-0.9.1/src/brevitas/quant/solver/parameter.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/trunc.py` & `brevitas-0.9.1/src/brevitas/quant/solver/trunc.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/solver/weight.py` & `brevitas-0.9.1/src/brevitas/quant/solver/weight.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant/ternary.py` & `brevitas-0.9.1/src/brevitas/quant/ternary.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant_tensor/__init__.py` & `brevitas-0.9.1/src/brevitas/quant_tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/quant_tensor/torch_handler.py` & `brevitas-0.9.1/src/brevitas/quant_tensor/torch_handler.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/utils/jit_utils.py` & `brevitas-0.9.1/src/brevitas/utils/jit_utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/utils/logging.py` & `brevitas-0.9.1/src/brevitas/utils/logging.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/utils/python_utils.py` & `brevitas-0.9.1/src/brevitas/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/utils/quant_utils.py` & `brevitas-0.9.1/src/brevitas/utils/quant_utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas/utils/torch_utils.py` & `brevitas-0.9.1/src/brevitas/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas.egg-info/PKG-INFO` & `brevitas-0.9.1/src/brevitas.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 Metadata-Version: 2.1
 Name: brevitas
-Version: 0.9.0
+Version: 0.9.1
 Summary: Quantization-aware training in PyTorch
 Home-page: https://github.com/Xilinx/brevitas
 Author: Alessandro Pappalardo
-Author-email: alessand@xilinx.com
+Author-email: alessand@amd.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: export
 Provides-Extra: hadamard
 Provides-Extra: test
 Provides-Extra: tts
 Provides-Extra: stt
 Provides-Extra: vision
 Provides-Extra: finn_integration
 Provides-Extra: ort_integration
 License-File: LICENSE
 
 # Brevitas
 
 [![Downloads](https://pepy.tech/badge/brevitas)](https://pepy.tech/project/brevitas)
-[![Gitter](https://badges.gitter.im/xilinx-brevitas/community.svg)](https://gitter.im/xilinx-brevitas/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 ![Pytest](https://github.com/Xilinx/brevitas/workflows/Pytest/badge.svg?branch=master)
 ![Examples Pytest](https://github.com/Xilinx/brevitas/workflows/Examples%20Pytest/badge.svg?branch=master)
 [![DOI](https://zenodo.org/badge/140494324.svg)](https://zenodo.org/badge/latestdoi/140494324)
 
 Brevitas is a PyTorch library for neural network quantization, with support for both *post-training quantization (PTQ)* and *quantization-aware training (QAT)*.
 
 **Please note that Brevitas is a research project and not an official Xilinx product.**
 
 If you like this project please consider ⭐ this repo, as it is the simplest and best way to support it.
 
-If you have issues, comments, or are just looking for advices on training quantized neural networks, open an issue or a discussion.
+## Requirements
+
+* Python >= 3.7 .
+* [Pytorch](https://pytorch.org) >= 1.5.1 .
+* Windows, Linux or macOS.
+* GPU training-time acceleration (*Optional* but recommended).
+
+## Installation
+
+You can install the latest release from PyPI:
+```bash
+pip install brevitas
+```
+
+## Getting Started
+
+Brevitas currently offers quantized implementations of the most common PyTorch layers used in DNN under `brevitas.nn`, such as `QuantConv1d`, `QuantConv2d`, `QuantConvTranspose1d`, `QuantConvTranspose2d`, `QuantMultiheadAttention`, `QuantRNN`, `QuantLSTM` etc., for adoption within PTQ and/or QAT.
+For each one of these layers, quantization of different tensors (inputs, weights, bias, outputs, etc) can be individually tuned according to a wide range of quantization settings.
+
+As a reference for PTQ, Brevitas provides an example user flow for ImageNet classification models under [`brevitas_examples.imagenet_classification.ptq`](https://github.com/Xilinx/brevitas/blob/master/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py) that quantizes an input torchvision model using PTQ under different quantization configurations (e.g. bit-width, granularity of scale, etc). Sample accuracy results are available [here](https://github.com/Xilinx/brevitas/blob/master/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv) for a selection of three reference topologies (ResNet18, MobileNet V2, ViT), under a variety of different quantization settings.
+
+For more info, checkout https://xilinx.github.io/brevitas/getting_started .
 
 ## Cite as
 
 If you adopt Brevitas in your work, please cite it as:
 ```
 @software{brevitas,
   author       = {Alessandro Pappalardo},
@@ -45,15 +66,14 @@
   year         = {2022},
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.3333552},
   url          = {https://doi.org/10.5281/zenodo.3333552}
 }
 ```
 
-
 ## History
 
 - *2023/04/21* - Release version 0.9.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.9.0).
 - *2023/01/10* - Release version 0.8.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.8.0).
 - *2021/12/13* - Release version 0.7.1, fix a bunch of issues. Added TVMCon 2021 tutorial notebook.
 - *2021/11/03* - Re-release version 0.7.0 (build 1) on PyPI to fix a packaging issue.
 - *2021/10/29* - Release version 0.7.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.7.0).
@@ -61,25 +81,7 @@
 - *2021/05/24* - Release version 0.5.1, fix a bunch of minor issues. See [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.1).
 - *2021/05/06* - Release version 0.5.0, see the [release notes](https://github.com/Xilinx/brevitas/releases/tag/v0.5.0).
 - *2021/03/15* - Release version 0.4.0, add support for \_\_torch_function\_\_ to QuantTensor.
 - *2021/03/04* - Release version 0.3.1, fix bug w/ act initialization from statistics w/ IGNORE_MISSING_KEYS=1.
 - *2021/03/01* - Release version 0.3.0, implements enum and shape solvers within extended dependency injectors. This allows declarative quantizers to be self-contained.
 - *2021/02/04* - Release version 0.2.1, includes various bugfixes of QuantTensor w/ zero-point.
 - *2021/01/30* - First release version 0.2.0 on PyPI.
-
-## Requirements
-
-* Python >= 3.7 .
-* [Pytorch](https://pytorch.org) >= 1.5.1 .
-* Windows, Linux or macOS.
-* GPU training-time acceleration (*Optional* but recommended).
-
-## Installation
-
-You can install the latest release from PyPI:
-```bash
-pip install brevitas
-```
-
-## Getting started
-
-Check out available info at https://xilinx.github.io/brevitas/getting_started .
```

### Comparing `brevitas-0.9.0/src/brevitas.egg-info/SOURCES.txt` & `brevitas-0.9.1/src/brevitas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
+setup.cfg
 setup.py
 notebooks/01_quant_tensor_quant_conv2d_overview.ipynb
 notebooks/02_quant_activation_overview.ipynb
 notebooks/03_anatomy_of_a_quantizer.ipynb
 notebooks/Brevitas_TVMCon2021.ipynb
 notebooks/ONNX_export_tutorial.ipynb
 notebooks/quantized_recurrent.ipynb
+requirements/requirements-dev.txt
 requirements/requirements-docs.txt
 requirements/requirements-export.txt
 requirements/requirements-finn-integration.txt
 requirements/requirements-hadamard.txt
 requirements/requirements-notebook.txt
 requirements/requirements-nox.txt
 requirements/requirements-ort-integration.txt
@@ -221,15 +222,14 @@
 src/brevitas_examples/bnn_pynq/trainer.py
 src/brevitas_examples/bnn_pynq/cfg/__init__.py
 src/brevitas_examples/bnn_pynq/cfg/cnv_1w1a.ini
 src/brevitas_examples/bnn_pynq/cfg/cnv_1w2a.ini
 src/brevitas_examples/bnn_pynq/cfg/cnv_2w2a.ini
 src/brevitas_examples/bnn_pynq/cfg/lfc_1w1a.ini
 src/brevitas_examples/bnn_pynq/cfg/lfc_1w2a.ini
-src/brevitas_examples/bnn_pynq/cfg/resnet18_3w3a.ini
 src/brevitas_examples/bnn_pynq/cfg/resnet18_4w4a.ini
 src/brevitas_examples/bnn_pynq/cfg/sfc_1w1a.ini
 src/brevitas_examples/bnn_pynq/cfg/sfc_1w2a.ini
 src/brevitas_examples/bnn_pynq/cfg/sfc_2w2a.ini
 src/brevitas_examples/bnn_pynq/cfg/tfc_1w1a.ini
 src/brevitas_examples/bnn_pynq/cfg/tfc_1w2a.ini
 src/brevitas_examples/bnn_pynq/cfg/tfc_2w2a.ini
```

### Comparing `brevitas-0.9.0/src/brevitas.egg-info/entry_points.txt` & `brevitas-0.9.1/src/brevitas.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas.egg-info/requires.txt` & `brevitas-0.9.1/src/brevitas.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 dependencies==2.0.1
 packaging
-pre-commit
 setuptools
 torch>=1.5.1
 typing-extensions>=3.7.4
 
-[:python_version < "3.7"]
-dataclasses
+[dev]
+pre-commit
 
 [docs]
 m2r2
 nbsphinx
 nbsphinx-link
 pydata-sphinx-theme
 sphinx==5.3.0
@@ -55,14 +54,15 @@
 torch-stft
 tqdm
 unidecode
 
 [test]
 hypothesis
 mock
+psutil
 pytest
 pytest-mock
 pytest-xdist
 pytest_cases
 scipy
 torchvision
```

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/README.md` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/README.md`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/bnn_pynq_train.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/bnn_pynq_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     parser.add_argument("--weight_decay", default=0, type=float, help="Weight decay")
     parser.add_argument("--epochs", default=1000, type=int, help="Number of epochs")
     parser.add_argument("--random_seed", default=1, type=int, help="Random seed")
     # Neural network Architecture
     parser.add_argument("--network", default="LFC_1W1A", type=str, help="neural network")
     parser.add_argument("--pretrained", action='store_true', help="Load pretrained model")
     parser.add_argument("--strict", action='store_true', help="Strict state dictionary loading")
+    parser.add_argument(
+        "--state_dict_to_pth",
+        action='store_true',
+        help="Saves a model state_dict into a pth and then exits")
     return parser.parse_args(args)
 
 
 class objdict(dict):
 
     def __getattr__(self, name):
         if name in self:
```

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/logger.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/logger.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/CNV.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/CNV.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/FC.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/FC.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/__init__.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,10 @@
 
 
 def lfc_1w2a(pretrained=True):
     model, _ = model_with_cfg('lfc_1w2a', pretrained)
     return model
 
 
-def resnet18_4w4a(pretrained=False):
+def resnet18_4w4a(pretrained=True):
     model, _ = model_with_cfg('resnet18_4w4a', pretrained)
     return model
-
-
-def resnet18_3w3a(pretrained=False):
-    model, _ = model_with_cfg('resnet18_3w3a', pretrained)
-    return model
```

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/common.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/losses.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/losses.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/resnet.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/resnet.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/models/tensor_norm.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/models/tensor_norm.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/bnn_pynq/trainer.py` & `brevitas-0.9.1/src/brevitas_examples/bnn_pynq/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (C) 2023, Advanced Micro Devices, Inc. All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 
 from datetime import datetime
+from hashlib import sha256
 import os
 import random
 import time
 
 from packaging.version import parse
 import torch
 from torch import nn
@@ -131,14 +132,27 @@
         # Resume checkpoint, if any
         if args.resume:
             print('Loading model checkpoint at: {}'.format(args.resume))
             package = torch.load(args.resume, map_location='cpu')
             model_state_dict = package['state_dict']
             model.load_state_dict(model_state_dict, strict=args.strict)
 
+        if args.state_dict_to_pth:
+            state_dict = model.state_dict()
+            name = args.network.lower()
+            path = os.path.join(self.checkpoints_dir_path, name)
+            torch.save(state_dict, path)
+            with open(path, "rb") as f:
+                bytes = f.read()
+                readable_hash = sha256(bytes).hexdigest()[:8]
+            new_path = path + '-' + readable_hash + '.pth'
+            os.rename(path, new_path)
+            self.logger.info("Saving checkpoint model to {}".format(new_path))
+            exit(0)
+
         if args.gpus is not None and len(args.gpus) == 1:
             model = model.to(device=self.device)
         if args.gpus is not None and len(args.gpus) > 1:
             model = nn.DataParallel(model, args.gpus)
         self.model = model
 
         # Loss function
```

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/README.md` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/README.md`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/README.md` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/README.md`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/__init__.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b.ini` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b5b.ini` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b5b.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b_round_avgpool.ini` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_4b_round_avgpool.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_hadamard_4b.ini` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/cfg/quant_proxylessnas_mobile14_hadamard_4b.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/common.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/mobilenetv1.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/proxylessnas.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/proxylessnas.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/models/vgg.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/models/vgg.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/README.md` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 
 We provide two workflows:
 - An evaluation script that, given a model name and a quantization configuration, performs PTQ on the model, evaluates its ImageNet top1 accuracy, and optionally exports it to either ONNX or TorchScript QCDQ.
 - A benchmark suite that tests several quantization configurations on a few selected models.
 
 Three types of target backend are exposed for programmatic quantization. Different backends dictate different structural policies for how a network should be quantized:
-- `generic`
+- *generic*:
   - The number of re-quantization ops is minimized by re-quantizing only when necessary, avoiding consecutive quantization ops if possible.
-  - Adds are quantized with the scale at the input, but allows for different signs.
+  - Adds are quantized to have the same scale at the input, but allows for different signs.
   - Concats are quantized to have the same scale, zero-point, sign and bit-width.
   - Activation quantization is performed earlier rather than later, so e.g. activation functions are quantized at their output.
-  - Activations are quantized to unsigned when possible, even with symmetric quantization.
-- `layerwise` - Quantizes only the input and the weights to compute-heavy layers. Other layers are left unquantized.
-- `flexml` - An internal backend.
+  - Activations are quantized to unsigned when possible during symmetric quantization (e.g. ReLU).
+- *layerwise* - Quantizes only the input and the weights to compute-heavy layers. Other layers are left unquantized.
+- *flexml* - An internal backend.
+
+
 The implementation for programmatic quantization is still experimental and might break on certain input models with certain configurations.
 
 
 For both these flows, the following options are exposed:
 - Bit-width of weight and activations.
 - Scales can be either float32 or power-of-two (po2) numbers.
 - Weights' scale factors can be either per-tensor or per-channel.
@@ -35,20 +37,47 @@
 
 
 Internally, when defining a quantized model programmatically, Brevitas leverages `torch.fx` and its `symbolic_trace` functionality, meaning that an input model is required to pass symbolic tracing for it to work.
 
 For more information about what are the currently supported quantized layers in Brevitas, check the [following file](https://github.com/Xilinx/brevitas/blob/dev/src/brevitas/graph/quantize.py),
 where we map the torch compute layers and activations with their corresponding quantized version.
 
+Pre-computed accuracy results for torchvision can be found under `RESULTS_TORCHVISION.csv` with several quantization combinations evaluated on three different torchvision models (ResNet18, MobileNet V2, ViT B32), while results on the hand defined quantized MobileNet V1 can be found under `RESULTS_IMGCLSMOB.csv`.
+Furthemore, for the torchvision models, we provide a `RESULTS_TORCHVISION_BEST_CONFIGS.csv`, where, for each combination of hardware-related features (e.g., support of per-channel scaling factors), we report the best configurations and their results.
+
 ## Evaluation flow
 
 This flow allows to specify which pre-trained torchvision model to quantize and apply PTQ to with the desired quantization configuration.
 It also gives the possibility to export the model to either ONNX QCDQ format or in torch QCDQ format.
 The quantization and export options to specify are:
 ```bash
+usage: ptq_evaluate.py [-h] --calibration-dir CALIBRATION_DIR --validation-dir
+                       VALIDATION_DIR [--workers WORKERS]
+                       [--batch-size-calibration BATCH_SIZE_CALIBRATION]
+                       [--batch-size-validation BATCH_SIZE_VALIDATION]
+                       [--export-dir EXPORT_DIR] [--gpu GPU]
+                       [--calibration-samples CALIBRATION_SAMPLES]
+                       [--model-name ARCH]
+                       [--target-backend {generic,layerwise,flexml}]
+                       [--scale-factor-type {float32,po2}]
+                       [--act-bit-width ACT_BIT_WIDTH]
+                       [--weight-bit-width WEIGHT_BIT_WIDTH]
+                       [--bias-bit-width {int32,int16}]
+                       [--act-quant-type {symmetric,asymmetric}]
+                       [--graph-eq-iterations GRAPH_EQ_ITERATIONS]
+                       [--act-quant-percentile ACT_QUANT_PERCENTILE]
+                       [--export-onnx-qcdq] [--export-torch-qcdq]
+                       [--scaling-per-output-channel | --no-scaling-per-output-channel]
+                       [--bias-corr | --no-bias-corr]
+                       [--graph-eq-merge-bias | --no-graph-eq-merge-bias]
+                       [--weight-narrow-range | --no-weight-narrow-range]
+
+PyTorch ImageNet PTQ Validation
+
+optional arguments:
   -h, --help            show this help message and exit
   --calibration-dir CALIBRATION_DIR
                         Path to folder containing Imagenet calibration folder
   --validation-dir VALIDATION_DIR
                         Path to folder containing Imagenet validation folder
   --workers WORKERS     Number of data loading workers (default: 8)
   --batch-size-calibration BATCH_SIZE_CALIBRATION
@@ -61,33 +90,36 @@
   --calibration-samples CALIBRATION_SAMPLES
                         Calibration size (default: 1000)
   --model-name ARCH     model architecture: alexnet | convnext_base |
                         convnext_large | convnext_small | convnext_tiny |
                         densenet121 | densenet161 | densenet169 | densenet201
                         | efficientnet_b0 | efficientnet_b1 | efficientnet_b2
                         | efficientnet_b3 | efficientnet_b4 | efficientnet_b5
+                        | efficientnet_b6 | efficientnet_b7 |
+                        efficientnet_v2_l | efficientnet_v2_m |
                         efficientnet_v2_s | googlenet | inception_v3 |
                         list_models | maxvit_t | mnasnet0_5 | mnasnet0_75 |
                         mnasnet1_0 | mnasnet1_3 | mobilenet_v2 |
                         mobilenet_v3_large | mobilenet_v3_small |
                         regnet_x_16gf | regnet_x_1_6gf | regnet_x_32gf |
                         regnet_x_3_2gf | regnet_x_400mf | regnet_x_800mf |
                         regnet_x_8gf | regnet_y_128gf | regnet_y_16gf |
                         regnet_y_1_6gf | regnet_y_32gf | regnet_y_3_2gf |
                         regnet_y_400mf | regnet_y_800mf | regnet_y_8gf |
                         resnet101 | resnet152 | resnet18 | resnet34 | resnet50
                         | resnext101_32x8d | resnext101_64x4d |
+                        resnext50_32x4d | shufflenet_v2_x0_5 |
                         shufflenet_v2_x1_0 | shufflenet_v2_x1_5 |
                         shufflenet_v2_x2_0 | squeezenet1_0 | squeezenet1_1 |
                         swin_b | swin_s | swin_t | swin_v2_b | swin_v2_s |
                         swin_v2_t | vgg11 | vgg11_bn | vgg13 | vgg13_bn |
                         vgg16 | vgg16_bn | vgg19 | vgg19_bn | vit_b_16 |
                         vit_b_32 | vit_h_14 | vit_l_16 | vit_l_32 |
                         wide_resnet101_2 | wide_resnet50_2 (default: resnet18)
-  --target-backend {generic,flexml}
+  --target-backend {generic,layerwise,flexml}
                         Backend to target for quantization (default: generic)
   --scale-factor-type {float32,po2}
                         Type for scale factors (default: float32)
   --act-bit-width ACT_BIT_WIDTH
                         Activations bit width (default: 8)
   --weight-bit-width WEIGHT_BIT_WIDTH
                         Weights bit width (default: 8)
@@ -115,27 +147,31 @@
                         Enable Narrow range for weight quantization (default: enabled)
   --no-weight-narrow-range
                         Disable Narrow range for weight quantization (default: enabled)
 ```
 
 The script requires to specify the calibration folder (`--calibration-dir`), from which the calibration samples will be taken (configurable with the `--calibration-samples` argument), and a validation folder (`--validation-dir`).
 
+For example, to run the script on the GPU 0:
+```bash
+brevitas_ptq_imagenet_val --calibration-dir /path/to/imagenet/calibration/folder --validation-dir /path/to/imagenet/validation/folder --gpu 0
+```
+
+
 ## Benchmark flow
 
 This scripts evaluate a variety of quantization configurations on different models.
 
 For example, to run the script on the GPU 0:
 ```bash
 brevitas_ptq_imagenet_benchmark --calibration-dir /path/to/imagenet/calibration/folder --validation-dir /path/to/imagenet/validation/folder --gpu 0
 ```
 
-After launching the script, a `RESULT_TORCHVISION.md` markdown file will be generated with the results on the torchvision models,
-and a `RESULTS_IMGCLSMOB.md` with the results on manually quantized models starting from floating point weights.
+After launching the script, a `RESULTS_TORCHVISION.csv` markdown file will be generated with the results on the torchvision models,
+and a `RESULTS_IMGCLSMOB.csv` with the results on manually quantized models starting from floating point weights.
 
-In this folder it is possible to find a pre-computed `RESULT_TORCHVISION.md` file all combinations evaluated on three different torchvision models (ResNet18, MobileNet V2, ViT B32),
-as well as the results on the hand defined quantized MobileNet V1 (`RESULTS_IMGCLSMOB.md`).
 
 
 [<sup>1 </sup>]: https://arxiv.org/abs/1906.04721
 [<sup>2 </sup>]: https://github.com/Xilinx/Vitis-AI/blob/50da04ddae396d10a1545823aca30b3abb24a276/src/vai_quantizer/vai_q_pytorch/nndct_shared/optimization/commander.py#L450
 [<sup>3 </sup>]: https://github.com/openppl-public/ppq/blob/master/ppq/quantization/algorithm/equalization.py
 [<sup>4 </sup>]: https://github.com/osmr/imgclsmob
```

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION.csv` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION.csv`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/RESULTS_TORCHVISION_BEST_CONFIGS.csv`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/ptq_benchmark.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/ptq_benchmark.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/ptq_common.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/ptq_common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/ptq_evaluate.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/ptq/utils.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/ptq/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/qat/README.md` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/qat/README.md`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/qat/imagenet_val.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/qat/imagenet_val.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/imagenet_classification/utils.py` & `brevitas-0.9.1/src/brevitas_examples/imagenet_classification/utils.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/README.md` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/README.md`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_4b.ini` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_4b.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_8b.ini` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_perchannelscaling_8b.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_pertensorscaling_8b.ini` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/quant_quartznet_pertensorscaling_8b.ini`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/cfg/topology/quartznet15x5.yaml` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/cfg/topology/quartznet15x5.yaml`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/get_librispeech_data.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/get_librispeech_data.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/__init__.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/audio_preprocessing.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/data_layer.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/data_layer.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/greedy_ctc_decoder.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/greedy_ctc_decoder.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/helpers.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/helpers.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/losses.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/losses.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/metrics.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/metrics.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/__init__.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/cleaners.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/cleaners.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/common.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/dataset.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/dataset.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/features.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/features.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/manifest.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/manifest.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/perturb.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/perturb.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/quartznet.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/quartznet.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/segment.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/segment.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/parts/spectr_augment.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/parts/spectr_augment.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet/quartznet.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet/quartznet.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/speech_to_text/quartznet_val.py` & `brevitas-0.9.1/src/brevitas_examples/speech_to_text/quartznet_val.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/README.md` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/README.md`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/__init__.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/__init__.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/common.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/common.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/generator_brevitas.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/generator_brevitas.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/melgan.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/melgan.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan/res_stack_brevitas.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan/res_stack_brevitas.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/melgan_val.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/melgan_val.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/preprocess_dataset.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/utilities/audio_processing.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/utilities/audio_processing.py`

 * *Files identical despite different names*

### Comparing `brevitas-0.9.0/src/brevitas_examples/text_to_speech/utilities/stft.py` & `brevitas-0.9.1/src/brevitas_examples/text_to_speech/utilities/stft.py`

 * *Files identical despite different names*

