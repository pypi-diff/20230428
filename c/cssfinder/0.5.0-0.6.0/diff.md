# Comparing `tmp/cssfinder-0.5.0.tar.gz` & `tmp/cssfinder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssfinder-0.5.0.tar", max compression
+gzip compressed data, was "cssfinder-0.6.0.tar", max compression
```

## Comparing `cssfinder-0.5.0.tar` & `cssfinder-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,85 @@
--rw-r--r--   0        0        0     1069 2023-03-22 00:32:36.723300 cssfinder-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     8870 2023-03-22 00:32:36.723300 cssfinder-0.5.0/README.md
--rw-r--r--   0        0        0     1417 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/__init__.py
--rw-r--r--   0        0        0     1280 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/__main__.py
--rw-r--r--   0        0        0     1224 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/algorithm/__init__.py
--rw-r--r--   0        0        0     1308 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/algorithm/backend/__init__.py
--rw-r--r--   0        0        0     3951 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/algorithm/backend/base.py
--rw-r--r--   0        0        0     6456 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/algorithm/backend/loader.py
--rw-r--r--   0        0        0     6934 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/algorithm/gilbert.py
--rw-r--r--   0        0        0     6166 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/algorithm/mode_util.py
--rw-r--r--   0        0        0     8771 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/api.py
--rw-r--r--   0        0        0     1676 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/base_model.py
--rw-r--r--   0        0        0    12606 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/cli.py
--rw-r--r--   0        0        0     4259 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/constants.py
--rw-r--r--   0        0        0     4915 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/crossplatform.py
--rw-r--r--   0        0        0    23376 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/cssfproject.py
--rw-r--r--   0        0        0     2169 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/enums.py
--rw-r--r--   0        0        0       10 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/.gitignore
--rw-r--r--   0        0        0     1192 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/5qubits_json/5qubits_in.mtx
--rw-r--r--   0        0        0     1816 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/5qubits_json/cssfproject.json
--rw-r--r--   0        0        0     1192 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/5qubits_py/5qubits_in.mtx
--rw-r--r--   0        0        0     2667 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/5qubits_py/cssfproject.py
--rw-r--r--   0        0        0     1036 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx
--rw-r--r--   0        0        0     2101 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/cssfproject.json
--rw-r--r--   0        0        0      175 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_0.mtx
--rw-r--r--   0        0        0      175 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_1.mtx
--rw-r--r--   0        0        0      175 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_0.mtx
--rw-r--r--   0        0        0     1762 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx
--rw-r--r--   0        0        0      166 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_2.mtx
--rw-r--r--   0        0        0     1762 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx
--rw-r--r--   0        0        0      183 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_4.mtx
--rw-r--r--   0        0        0     1762 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx
--rw-r--r--   0        0        0      166 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_6.mtx
--rw-r--r--   0        0        0     1762 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx
--rw-r--r--   0        0        0     3638 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx
--rw-r--r--   0        0        0     1174 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/GHZ4_json/cssfproject.json
--rw-r--r--   0        0        0     2585 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/SBiPa_json/cssfproject.json
--rw-r--r--   0        0        0     1270 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/SBiPa_json/projection.mtx
--rw-r--r--   0        0        0     1270 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/SBiPa_json/state.mtx
--rw-r--r--   0        0        0     5059 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/examples/__init__.py
--rw-r--r--   0        0        0     1227 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/io/__init__.py
--rw-r--r--   0        0        0     6003 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/io/gilbert_io.py
--rw-r--r--   0        0        0     4182 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/io/matrix.py
--rwxr-xr-x   0        0        0    10244 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/log.py
--rw-r--r--   0        0        0     1547 2023-03-22 00:32:36.723300 cssfinder-0.5.0/cssfinder/reports/__init__.py
--rw-r--r--   0        0        0     1291 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/archive.py
--rw-r--r--   0        0        0     2200 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/html.py
--rw-r--r--   0        0        0     4292 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/manager.py
--rw-r--r--   0        0        0     9217 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/math.py
--rw-r--r--   0        0        0     2937 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/pdf.py
--rw-r--r--   0        0        0     8295 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/plotting.py
--rw-r--r--   0        0        0     4619 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/renderer.py
--rw-r--r--   0        0        0     1203 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/reports/txt.py
--rw-r--r--   0        0        0     3947 2023-03-22 00:32:36.727300 cssfinder-0.5.0/cssfinder/templates/report.html.jinja2
--rw-r--r--   0        0        0    16868 2023-03-22 00:32:36.731300 cssfinder-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10042 1970-01-01 00:00:00.000000 cssfinder-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 23:10:30.086484 cssfinder-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0    11275 2023-04-27 23:10:30.086484 cssfinder-0.6.0/README.md
+-rw-r--r--   0        0        0     1417 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/__init__.py
+-rw-r--r--   0        0        0     1280 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/__main__.py
+-rw-r--r--   0        0        0     1224 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/backend/__init__.py
+-rw-r--r--   0        0        0     3951 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/backend/base.py
+-rw-r--r--   0        0        0     6456 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/backend/loader.py
+-rw-r--r--   0        0        0     6934 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/gilbert.py
+-rw-r--r--   0        0        0     6166 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/mode_util.py
+-rw-r--r--   0        0        0     9651 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/api.py
+-rw-r--r--   0        0        0     1676 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/base_model.py
+-rw-r--r--   0        0        0    18270 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/cli.py
+-rw-r--r--   0        0        0     3875 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/constants.py
+-rw-r--r--   0        0        0     4915 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/crossplatform.py
+-rw-r--r--   0        0        0    23376 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/cssfproject.py
+-rw-r--r--   0        0        0     2169 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/enums.py
+-rw-r--r--   0        0        0       10 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/.gitignore
+-rw-r--r--   0        0        0     1192 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_json/5qubits_in.mtx
+-rw-r--r--   0        0        0     1819 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_json/cssfproject.json
+-rw-r--r--   0        0        0     1192 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_py/5qubits_in.mtx
+-rw-r--r--   0        0        0     2667 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_py/cssfproject.py
+-rw-r--r--   0        0        0     1036 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx
+-rw-r--r--   0        0        0     2101 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/cssfproject.json
+-rw-r--r--   0        0        0      175 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_0.mtx
+-rw-r--r--   0        0        0      175 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_1.mtx
+-rw-r--r--   0        0        0      175 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_0.mtx
+-rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx
+-rw-r--r--   0        0        0      166 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_2.mtx
+-rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx
+-rw-r--r--   0        0        0      183 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_4.mtx
+-rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx
+-rw-r--r--   0        0        0      166 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_6.mtx
+-rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx
+-rw-r--r--   0        0        0     3638 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx
+-rw-r--r--   0        0        0     1174 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ4_json/cssfproject.json
+-rw-r--r--   0        0        0     2593 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/SBiPa_json/cssfproject.json
+-rw-r--r--   0        0        0     1270 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/SBiPa_json/projection.mtx
+-rw-r--r--   0        0        0     1270 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/SBiPa_json/state.mtx
+-rw-r--r--   0        0        0     5139 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx
+-rw-r--r--   0        0        0     2957 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/benchmark_32x32/cssfproject.py
+-rw-r--r--   0        0        0    54182 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/10_in.mtx
+-rw-r--r--   0        0        0     3693 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/cssfproject.py
+-rw-r--r--   0        0        0     4265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx
+-rw-r--r--   0        0        0     4297 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx
+-rw-r--r--   0        0        0     4265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx
+-rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx
+-rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx
+-rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx
+-rw-r--r--   0        0        0     4281 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx
+-rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx
+-rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx
+-rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx
+-rw-r--r--   0        0        0     4265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx
+-rw-r--r--   0        0        0     4297 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx
+-rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx
+-rw-r--r--   0        0        0    14212 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/interactive.py
+-rw-r--r--   0        0        0     1227 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/io/__init__.py
+-rw-r--r--   0        0        0     6003 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/io/gilbert_io.py
+-rw-r--r--   0        0        0     4182 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/io/matrix.py
+-rwxr-xr-x   0        0        0    12147 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/log.py
+-rw-r--r--   0        0        0     1547 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/__init__.py
+-rw-r--r--   0        0        0     1291 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/archive.py
+-rw-r--r--   0        0        0     2200 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/html.py
+-rw-r--r--   0        0        0     4292 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/manager.py
+-rw-r--r--   0        0        0     9217 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/math.py
+-rw-r--r--   0        0        0     2937 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/pdf.py
+-rw-r--r--   0        0        0     8295 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/plotting.py
+-rw-r--r--   0        0        0     4619 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/renderer.py
+-rw-r--r--   0        0        0     1203 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/txt.py
+-rw-r--r--   0        0        0     3947 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/templates/report.html.jinja2
+-rw-r--r--   0        0        0    17232 2023-04-27 23:10:30.098484 cssfinder-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12779 1970-01-01 00:00:00.000000 cssfinder-0.6.0/PKG-INFO
```

### Comparing `cssfinder-0.5.0/LICENSE.md` & `cssfinder-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/README.md` & `cssfinder-0.6.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,32 @@
 
 To install CSSFinder from PyPI, use `pip` in terminal:
 
 ```
 pip install cssfinder
 ```
 
+Because CSSFinder is a modular tool, you will have to also install a `backend`
+package, which contains concrete implementation of algorithms. Simples way is
+to just install `numpy` or `rust` extras set:
+
+```
+pip install cssfinder[numpy]
+```
+
+```
+pip install cssfinder[rust]
+```
+
+You don't need both, one will be perfectly fine. Alternatively, you may find
+`cssfinder-backend-numpy` and `cssfinder-backend-rust` on PyPI and install them
+manually, with exact same effect. Backends are dynamically detected from all
+locations, Python can import modules, thus any valid way of making backend code
+reachable for interpreter will work.
+
 If you want to use development version, traverse `Development` and `Packaging`
 sections below.
 
 ### But there is a catch!
 
 CSSFinder can export PDF reports (and other formats too), but it uses
 `weasyprint` for that and `weasyprint` relies on `GTK3`. Unfortunately it is
@@ -23,14 +41,66 @@
 you can find official guidelines from `weasyprint`.
 [This repository](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer)
 may also help. Alternatively you can use WSL to install and run CSSFinder, as
 its seamless to do that.
 
 Its worth mentioning that other formats are not affected by this issue.
 
+## Examples
+
+Fortunately for all newcomers, CSSFinders comes in with some example projects,
+which may come in handy while starting to describe your first project.
+
+List of examples available with CSSFinder can be obtained with command:
+
+```
+cssfinder examples list
+```
+
+Afterwards you should be presented with table, within console window, similar
+to this one:
+
+![image](https://user-images.githubusercontent.com/56170852/233212801-6cd1fb3e-ae91-4878-81d7-d972431850ed.png)
+
+For sake of example, let's assume that name `5qubits_json` caught our eye, and
+now we are willing to spend some of our precious time diving deeper into what's
+inside. To do that, we have to clone this example somewhere with following
+command:
+
+```
+cssfinder examples clone --name 5qubits_json
+```
+
+> This command, similarly to all other commands of all other CSSFinder
+> commands, can be used with `--help` flag to inspect possible invocation
+> parameters.
+
+As result, you should find `5qubits_json` directory have been created in your
+current working directory.
+
+> Example `5qubits_json` relies on `numpy` backend, make sure to install it, if
+> you haven't done it before.
+
+![image](https://user-images.githubusercontent.com/56170852/233217324-9b51d732-18a6-4297-91d7-b277c73edfd6.png)
+
+Now we can proceed with running tasks defined within the project. That can be
+achieved with following command:
+
+```
+cssfinder project -p ./5qubits_json/ task run
+```
+
+This command will run all tasks, which may take something in between of few
+seconds and few minutes, depending on your hardware.
+
+Result of calculations can be inspected in `output/` directory in project
+folder (`5qubits_json/`).
+
+![image](https://user-images.githubusercontent.com/56170852/233218942-ac47a923-21f7-4b3a-af02-7a7961360abc.png)
+
 ## Development
 
 This project uses `Python` programming language and requires at least python
 `3.8` for development and distribution. Development dependencies
 [`poetry`](https://pypi.org/project/poetry/) for managing dependencies and
 distribution building. It is necessary to perform any operations in development
 environment.
@@ -81,35 +151,35 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder-0.5.0` or alike inside.
+This will create `dist/` directory with `cssfinder-0.6.0` or alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder-0.5.0
+pip install ./dist/cssfinder-0.6.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder-0.5.0
+Successfully installed cssfinder-0.6.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder-0.5.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder-0.6.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder-0.5.0` should be included in this list.
+But `cssfinder-0.6.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
```

### Comparing `cssfinder-0.5.0/cssfinder/__init__.py` & `cssfinder-0.6.0/cssfinder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 """CSSFinder (Closest Separable State Finder) is a package containing implementation of
 Gilbert algorithm for finding an upper bound on the Hilbert-Schmidt distance between a
 given state and the set of separable states.
 """
 
 from __future__ import annotations
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `cssfinder-0.5.0/cssfinder/__main__.py` & `cssfinder-0.6.0/cssfinder/__main__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/algorithm/__init__.py` & `cssfinder-0.6.0/cssfinder/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/algorithm/backend/__init__.py` & `cssfinder-0.6.0/cssfinder/algorithm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/algorithm/backend/base.py` & `cssfinder-0.6.0/cssfinder/algorithm/backend/base.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/algorithm/backend/loader.py` & `cssfinder-0.6.0/cssfinder/algorithm/backend/loader.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/algorithm/gilbert.py` & `cssfinder-0.6.0/cssfinder/algorithm/gilbert.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/algorithm/mode_util.py` & `cssfinder-0.6.0/cssfinder/algorithm/mode_util.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/api.py` & `cssfinder-0.6.0/cssfinder/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 """Module contains high level API of cssfinder."""
 
 from __future__ import annotations
 
 import logging
 import os
+from concurrent.futures import ProcessPoolExecutor
+from dataclasses import dataclass
+from itertools import repeat
 from typing import TYPE_CHECKING, Iterable
 
 import psutil
 
 from cssfinder.algorithm.gilbert import Gilbert
 from cssfinder.algorithm.mode_util import ModeUtil
 from cssfinder.crossplatform import IoPriority, Priority, set_priority
@@ -42,58 +45,94 @@
 
 
 def run_project_from(
     project_file_path: Path | str,
     tasks: list[str] | None = None,
     *,
     is_debug: bool = False,
+    force_sequential: bool = False,
+    max_parallel: int = -1,
 ) -> None:
     """Load project and run all tasks."""
     project = CSSFProject.load_project(project_file_path)
     logging.info(
         "Loaded project %r by %r <%r>.",
         project.meta.name,
         project.meta.author,
         project.meta.email,
     )
-    run_project(project, tasks, is_debug=is_debug)
+    run_project(
+        project,
+        tasks,
+        is_debug=is_debug,
+        force_sequential=force_sequential,
+        max_parallel=max_parallel,
+    )
 
 
 def run_project(
     project: CSSFProject,
     tasks: list[str] | None = None,
     *,
     is_debug: bool = False,
-) -> None:
+    force_sequential: bool = False,
+    max_parallel: int = -1,
+) -> list[Task]:
     """Run all tasks defined in project."""
     logging.debug("Running project %r", project.meta.name)
 
     message = "\n    |  ".join(project.json(indent=2).split("\n"))
     logging.info("%s", "\n    |  " + message)
 
-    for task in project.select_tasks(tasks):
-        run_task(task, is_debug=is_debug)
+    task_list = project.select_tasks(tasks)
+
+    if force_sequential:
+        for _ in map(
+            run_task,
+            task_list,
+            repeat(TaskOptions(is_debug=is_debug)),
+        ):
+            pass
+
+    else:
+        with ProcessPoolExecutor(
+            max_parallel if max_parallel > 0 else None
+        ) as executor:
+            executor.map(
+                run_task,
+                task_list,
+                repeat(TaskOptions(is_debug=is_debug)),
+            )
+
+    return task_list
+
+
+@dataclass
+class TaskOptions:
+    """Container for extra task options."""
+
+    is_debug: bool
 
 
-def run_task(task: Task, *, is_debug: bool = False) -> None:
+def run_task(task: Task, options: TaskOptions) -> None:
     """Run task until completed."""
     try:
         set_priority(os.getpid(), Priority.REALTIME, IoPriority.HIGH)
     except (OSError, psutil.AccessDenied):
         logging.warning(
             "Failed to elevate process priority. It can negatively affect program "
             "performance if there are more programs running in background. "
             "To allow automated priority elevation run this program as super user. "
             "You can change priority manually for process PID %r.",
             os.getpid(),
             stack_info=False,
         )
 
     if task.gilbert:
-        run_gilbert(task.gilbert, task.task_output_directory, is_debug=is_debug)
+        run_gilbert(task.gilbert, task.task_output_directory, is_debug=options.is_debug)
 
 
 def run_gilbert(
     config: GilbertCfg,
     task_output_directory: Path,
     *,
     is_debug: bool = False,
```

### Comparing `cssfinder-0.5.0/cssfinder/base_model.py` & `cssfinder-0.6.0/cssfinder/base_model.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/crossplatform.py` & `cssfinder-0.6.0/cssfinder/crossplatform.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/cssfproject.py` & `cssfinder-0.6.0/cssfinder/cssfproject.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/enums.py` & `cssfinder-0.6.0/cssfinder/enums.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/5qubits_json/5qubits_in.mtx` & `cssfinder-0.6.0/cssfinder/examples/5qubits_json/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/5qubits_json/cssfproject.json` & `cssfinder-0.6.0/cssfinder/examples/5qubits_json/cssfproject.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'tasks'": "{'test_fsnqd_5qubits': {'gilbert': {'runtime': {'iters_per_epoch': 1000, "*

 * *            "'max_corrections': 100}}}}"}*

```diff
@@ -39,16 +39,16 @@
                 "mode": {
                     "$ref": "#/tasks/main/gilbert/mode"
                 },
                 "resources": {
                     "$ref": "#/tasks/main/gilbert/resources"
                 },
                 "runtime": {
-                    "iters_per_epoch": 10,
-                    "max_corrections": 10,
+                    "iters_per_epoch": 1000,
+                    "max_corrections": 100,
                     "max_epochs": 10,
                     "visibility": 0.4
                 },
                 "state": {
                     "$ref": "#/tasks/main/gilbert/state"
                 }
             }
```

### Comparing `cssfinder-0.5.0/cssfinder/examples/5qubits_py/5qubits_in.mtx` & `cssfinder-0.6.0/cssfinder/examples/5qubits_py/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/5qubits_py/cssfproject.py` & `cssfinder-0.6.0/cssfinder/examples/5qubits_py/cssfproject.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx` & `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ3_json/cssfproject.json` & `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx` & `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx` & `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx` & `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx` & `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx` & `cssfinder-0.6.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/GHZ4_json/cssfproject.json` & `cssfinder-0.6.0/cssfinder/examples/GHZ4_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/SBiPa_json/cssfproject.json` & `cssfinder-0.6.0/cssfinder/examples/SBiPa_json/cssfproject.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99921875%*

 * *Differences: {"'tasks'": "{'test_sbipa_proj': {'gilbert': {'runtime': {'max_epochs': 100, 'iters_per_epoch': "*

 * *            "1000, 'max_corrections': 100}}}, 'test_sbipa_proj_with_projection': {'gilbert': "*

 * *            "{'runtime': {'max_epochs': 100, 'iters_per_epoch': 1000, 'max_corrections': 100}}}}"}*

```diff
@@ -42,17 +42,17 @@
                 "mode": {
                     "$ref": "#/tasks/main/gilbert/mode"
                 },
                 "resources": {
                     "$ref": "#/tasks/main/gilbert/resources"
                 },
                 "runtime": {
-                    "iters_per_epoch": 10,
-                    "max_corrections": 10,
-                    "max_epochs": 10,
+                    "iters_per_epoch": 1000,
+                    "max_corrections": 100,
+                    "max_epochs": 100,
                     "visibility": 0.4
                 },
                 "state": {
                     "$ref": "#/tasks/main/gilbert/state"
                 }
             }
         },
@@ -65,17 +65,17 @@
                     "$ref": "#/tasks/main/gilbert/mode"
                 },
                 "resources": {
                     "projection": "{project.project_directory}/projection.mtx",
                     "symmetries": null
                 },
                 "runtime": {
-                    "iters_per_epoch": 10,
-                    "max_corrections": 10,
-                    "max_epochs": 10,
+                    "iters_per_epoch": 1000,
+                    "max_corrections": 100,
+                    "max_epochs": 100,
                     "visibility": 0.4
                 },
                 "state": {
                     "$ref": "#/tasks/main/gilbert/state"
                 }
             }
         }
```

### Comparing `cssfinder-0.5.0/cssfinder/examples/SBiPa_json/projection.mtx` & `cssfinder-0.6.0/cssfinder/examples/SBiPa_json/projection.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/SBiPa_json/state.mtx` & `cssfinder-0.6.0/cssfinder/examples/SBiPa_json/state.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/examples/__init__.py` & `cssfinder-0.6.0/cssfinder/examples/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     """Enumeration of available examples."""
 
     e5qubits_json = "5qubits_json"
     e5qubits_py = "5qubits_py"
     GHZ3_json = "GHZ3_json"
     GHZ4_json = "GHZ4_json"
     SBiPa_json = "SBiPa_json"
+    benchmark_32x32 = "benchmark_32x32"
+    benchmark_64x64 = "benchmark_64x64"
 
     def get_sha256(self) -> hashlib._Hash:  # noqa: SLF001
         """Calculate and return SHA-256 of example project file."""
         source = self.get_project().project_file
         content = source.read_bytes()
         return hashlib.sha256(content)
```

### Comparing `cssfinder-0.5.0/cssfinder/io/__init__.py` & `cssfinder-0.6.0/cssfinder/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/io/gilbert_io.py` & `cssfinder-0.6.0/cssfinder/io/gilbert_io.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/io/matrix.py` & `cssfinder-0.6.0/cssfinder/io/matrix.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/log.py` & `cssfinder-0.6.0/cssfinder/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -68,24 +68,30 @@
 NoHighlightRichHandler(RichHandler)
     A subclass of RichHandler to remove all rich formatting from the logging messages.
 
 """
 
 from __future__ import annotations
 
+import json
 import logging
 import sys
 from logging import LogRecord, getLogger, handlers
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
+from unittest.mock import patch
 
+from filelock import FileLock
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.text import Text
 
+if TYPE_CHECKING:
+    from cssfinder.cssfproject import CSSFProject, Task
+
 LOGGER: logging.Logger
 VERBOSITY_MAP: dict[int, int] = {
     0: logging.CRITICAL,
     1: logging.WARNING,
     2: logging.INFO,
     3: logging.DEBUG,
 }
@@ -245,15 +251,15 @@
     logger_name: str,
     log_dir: Path,
     auto_rollover_sec: int,
     max_log_files: int,
 ) -> logging.Handler:
     # Create logging directory before trying to put files there.
     log_dir.mkdir(0o777, parents=True, exist_ok=True)
-    log_file = log_dir / logger_name
+    log_file = log_dir / f"{logger_name}.log"
     # If file already exists, logger may decide to start appending its logs to it,
     # which is not desired - preferably, one file for one session.
     log_file_already_exists = log_file.exists()
 
     file_handler = handlers.TimedRotatingFileHandler(
         log_file,
         # Only way to get full time stamp is to select "S" - seconds
@@ -282,10 +288,61 @@
     # rollover to get new file for logging after startup.
     if log_file_already_exists:
         file_handler.doRollover()
 
     return file_handler
 
 
+def enable_performance_logging() -> None:
+    """Enable run time measurement and logging for run_project() function."""
+    import time
+
+    from cssfinder.api import run_project
+
+    def run_project_wrapper(
+        project: CSSFProject,
+        tasks: list[str] | None = None,
+        *,
+        is_debug: bool = False,
+        force_sequential: bool = False,
+        max_parallel: int = -1,
+    ) -> list[Task]:
+        start_time = time.perf_counter()
+        task_list = run_project(
+            project,
+            tasks,
+            is_debug=is_debug,
+            force_sequential=force_sequential,
+            max_parallel=max_parallel,
+        )
+        end_time = time.perf_counter()
+        execution_time = end_time - start_time
+
+        perf_file = Path.cwd() / f"perf_{project.meta.name}.json"
+
+        with FileLock(perf_file.with_suffix(".lock").as_posix()):
+            if perf_file.exists():
+                raw_content = perf_file.read_text(encoding="utf-8")
+                try:
+                    perf_index = json.loads(raw_content)
+                except json.JSONDecodeError:
+                    perf_index = {}
+            else:
+                perf_index = {}
+
+            key = str.join("|", tasks) if tasks is not None else "None"
+            perf_results_list = perf_index.get(key, [])
+            perf_results_list.append(execution_time)
+            perf_index[key] = perf_results_list
+
+            serialized_perf_index = json.dumps(perf_index, indent=4)
+            perf_file.write_text(serialized_perf_index, encoding="utf-8")
+
+        print(f"Execution time: {execution_time:.6f} seconds")
+        return task_list
+
+    patch("cssfinder.api.run_project", new=run_project_wrapper).__enter__()
+
+
 if __name__ == "__main__":
     print(f"Decent log config ver. {__version__}")
     raise SystemExit(0)
```

### Comparing `cssfinder-0.5.0/cssfinder/reports/__init__.py` & `cssfinder-0.6.0/cssfinder/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/archive.py` & `cssfinder-0.6.0/cssfinder/reports/archive.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/html.py` & `cssfinder-0.6.0/cssfinder/reports/html.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/manager.py` & `cssfinder-0.6.0/cssfinder/reports/manager.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/math.py` & `cssfinder-0.6.0/cssfinder/reports/math.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/pdf.py` & `cssfinder-0.6.0/cssfinder/reports/pdf.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/plotting.py` & `cssfinder-0.6.0/cssfinder/reports/plotting.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/renderer.py` & `cssfinder-0.6.0/cssfinder/reports/renderer.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/reports/txt.py` & `cssfinder-0.6.0/cssfinder/reports/txt.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/cssfinder/templates/report.html.jinja2` & `cssfinder-0.6.0/cssfinder/templates/report.html.jinja2`

 * *Files identical despite different names*

### Comparing `cssfinder-0.5.0/pyproject.toml` & `cssfinder-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] # ANCHOR: tool.poetry
 name = "cssfinder"
-version = "0.5.0"
+version = "0.6.0"
 description = "Tool for Hilbert-Schmidt distance calculation with Gilbert algorithm."
 authors = [
     "Krzysztof Wiśniewski <argmaster.world@gmail.com>",
     "Marcin Wieśniak <marcin.wiesniak@ug.edu.pl>",
 ]
 repository = "https://github.com/argmaster/CSSFinder"
 readme = "README.md"
@@ -20,34 +20,43 @@
 typing-extensions = "^4.5.0"
 rich = "^13.3.1"
 jsonref = "^1.1.0"
 matplotlib = "^3.7.0"
 pandas = "^1.5.3"
 weasyprint = "^58.1"
 psutil = "^5.9.4"
+pytermgui = "^7.3.0"
+jinja2 = "^3.1.2"
+cssfinder-backend-numpy = { version = ">=0.3.0", optional = true }
+cssfinder-backend-rust = { version = ">=0.1.0", optional = true }
+filelock = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies] # ANCHOR: tool.poetry.dev-dependencies
 black = ">=22.12,<24.0"
 isort = "^5.11.4"
-docformatter = { extras = ["tomli"], version = "^1.5.1" }
+docformatter = { extras = ["tomli"], version = "==1.5.1" }
 pytest = "^7.2.0"
 autoflake = "^2.0.0"
 pre-commit = ">=2.20,<4.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.0.1"
 ptpython = "^3.0.22"
 typing-extensions = "^4.4.0"
 snakeviz = "^2.1.1"
-poethepoet = "^0.18.1"
+poethepoet = ">=0.18.1,<0.20.0"
 poetry = "^1.3.2"
 jinja2 = "^3.1.2"
-ruff = "^0.0.254"
+ruff = ">=0.0.254"
 ipykernel = "^6.21.3"
 cssfinder-backend-numpy = ">=0.3.0"
 
+[tool.poetry.extras]
+backend-numpy = ["cssfinder-backend-numpy"]
+backend-rust = ["cssfinder-backend-rust"]
+
 [tool.poetry.scripts]
 cssfinder = "cssfinder.cli:main"
 cssf = "cssfinder.cli:main"
 
 [tool.poe.tasks]
 release = { script = "scripts.release:main" }
 install-hooks = [
@@ -72,15 +81,23 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options] # ANCHOR: tool.pytest
 minversion = "7.2.0"
-norecursedirs = ["external", "data", ".venv", ".env", "env", "venv"]
+norecursedirs = [
+    "external",
+    "data",
+    ".venv",
+    ".env",
+    "env",
+    "venv",
+    "cssfinder/examples",
+]
 python_files = ["test_*.py", "*_test.py"]
 testpaths = ["cssfinder", "test"]
 addopts = """ -ra --strict-markers --doctest-modules --log-level=DEBUG --cov-report=term-missing:skip-covered"""
 filterwarnings = []
 
 [tool.isort] # ANCHOR: tool.isort
 # ---------------------------------------------------------------------------- #
@@ -93,15 +110,14 @@
 
 [tool.black] # ANCHOR: tool.black
 # https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format
 line-length = 88
 target-version = ['py38', 'py39', 'py310', 'py311']
 extend-exclude = "(external)"
 
-
 [tool.mypy] # ANCHOR: tool.mypy
 # ---------------------------------------------------------------------------- #
 #            https://mypy.readthedocs.io/en/stable/config_file.html            #
 #            https://mypy.readthedocs.io/en/stable/command_line.html           #
 #          https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html          #
 # ---------------------------------------------------------------------------- #
 python_version = "3.8"
```

### Comparing `cssfinder-0.5.0/PKG-INFO` & `cssfinder-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: cssfinder
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tool for Hilbert-Schmidt distance calculation with Gilbert algorithm.
 Home-page: https://github.com/argmaster/CSSFinder
 Author: Krzysztof Wiśniewski
 Author-email: argmaster.world@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: backend-numpy
+Provides-Extra: backend-rust
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cssfinder-backend-numpy (>=0.3.0) ; extra == "backend-numpy"
+Requires-Dist: cssfinder-backend-rust (>=0.1.0) ; extra == "backend-rust"
+Requires-Dist: filelock (>=3.12.0,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic[email] (>=1.10.5,<2.0.0)
+Requires-Dist: pytermgui (>=7.3.0,<8.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: weasyprint (>=58.1,<59.0)
 Project-URL: Repository, https://github.com/argmaster/CSSFinder
 Description-Content-Type: text/markdown
 
@@ -35,14 +42,32 @@
 
 To install CSSFinder from PyPI, use `pip` in terminal:
 
 ```
 pip install cssfinder
 ```
 
+Because CSSFinder is a modular tool, you will have to also install a `backend`
+package, which contains concrete implementation of algorithms. Simples way is
+to just install `numpy` or `rust` extras set:
+
+```
+pip install cssfinder[numpy]
+```
+
+```
+pip install cssfinder[rust]
+```
+
+You don't need both, one will be perfectly fine. Alternatively, you may find
+`cssfinder-backend-numpy` and `cssfinder-backend-rust` on PyPI and install them
+manually, with exact same effect. Backends are dynamically detected from all
+locations, Python can import modules, thus any valid way of making backend code
+reachable for interpreter will work.
+
 If you want to use development version, traverse `Development` and `Packaging`
 sections below.
 
 ### But there is a catch!
 
 CSSFinder can export PDF reports (and other formats too), but it uses
 `weasyprint` for that and `weasyprint` relies on `GTK3`. Unfortunately it is
@@ -52,14 +77,66 @@
 you can find official guidelines from `weasyprint`.
 [This repository](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer)
 may also help. Alternatively you can use WSL to install and run CSSFinder, as
 its seamless to do that.
 
 Its worth mentioning that other formats are not affected by this issue.
 
+## Examples
+
+Fortunately for all newcomers, CSSFinders comes in with some example projects,
+which may come in handy while starting to describe your first project.
+
+List of examples available with CSSFinder can be obtained with command:
+
+```
+cssfinder examples list
+```
+
+Afterwards you should be presented with table, within console window, similar
+to this one:
+
+![image](https://user-images.githubusercontent.com/56170852/233212801-6cd1fb3e-ae91-4878-81d7-d972431850ed.png)
+
+For sake of example, let's assume that name `5qubits_json` caught our eye, and
+now we are willing to spend some of our precious time diving deeper into what's
+inside. To do that, we have to clone this example somewhere with following
+command:
+
+```
+cssfinder examples clone --name 5qubits_json
+```
+
+> This command, similarly to all other commands of all other CSSFinder
+> commands, can be used with `--help` flag to inspect possible invocation
+> parameters.
+
+As result, you should find `5qubits_json` directory have been created in your
+current working directory.
+
+> Example `5qubits_json` relies on `numpy` backend, make sure to install it, if
+> you haven't done it before.
+
+![image](https://user-images.githubusercontent.com/56170852/233217324-9b51d732-18a6-4297-91d7-b277c73edfd6.png)
+
+Now we can proceed with running tasks defined within the project. That can be
+achieved with following command:
+
+```
+cssfinder project -p ./5qubits_json/ task run
+```
+
+This command will run all tasks, which may take something in between of few
+seconds and few minutes, depending on your hardware.
+
+Result of calculations can be inspected in `output/` directory in project
+folder (`5qubits_json/`).
+
+![image](https://user-images.githubusercontent.com/56170852/233218942-ac47a923-21f7-4b3a-af02-7a7961360abc.png)
+
 ## Development
 
 This project uses `Python` programming language and requires at least python
 `3.8` for development and distribution. Development dependencies
 [`poetry`](https://pypi.org/project/poetry/) for managing dependencies and
 distribution building. It is necessary to perform any operations in development
 environment.
@@ -110,35 +187,35 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder-0.5.0` or alike inside.
+This will create `dist/` directory with `cssfinder-0.6.0` or alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder-0.5.0
+pip install ./dist/cssfinder-0.6.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder-0.5.0
+Successfully installed cssfinder-0.6.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder-0.5.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder-0.6.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder-0.5.0` should be included in this list.
+But `cssfinder-0.6.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
```

