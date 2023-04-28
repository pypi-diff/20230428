# Comparing `tmp/write_the-0.7.6.tar.gz` & `tmp/write_the-0.7.7.tar.gz`

## Comparing `write_the-0.7.6.tar` & `write_the-0.7.7.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.6/mkdocs.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.7.6/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.7.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.7.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/CNAME
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/tests.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.6/docs/reference/utils.md
--rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.7.6/images/docs-help.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.6/images/logo-black.svg
--rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.7.6/images/logo.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.6/images/mkdocs-help.png
--rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.6/images/multiply-docs-tests.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.6/images/tests-help.png
--rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.7.6/images/untitled.blend
--rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.7.6/images/untitled.blend1
--rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.7.6/images/write-the-docs.gif
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.6/images/write-the-icon.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.6/images/write-the.svg
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cli_main.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_cst_utils.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/test_utils.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/calculate.py
--rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/expected.dat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.6/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/__main__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/llm.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cli/main.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cli/tasks.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/__init__.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/docs.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/prompts.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/docs/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/mkdocs/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/mkdocs/mkdocs.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/mkdocs/templates.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/tests/prompts.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/commands/tests/tests.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.6/write_the/cst/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 write_the-0.7.6/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.6/LICENSE.txt
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 write_the-0.7.6/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 write_the-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 write_the-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.7/mkdocs.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.7.7/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.7.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.7.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/CNAME
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/index.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/cli.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/commands.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/cst.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/llm.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/utils.md
+-rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.7.7/images/docs-help.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.7/images/logo-black.svg
+-rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.7.7/images/logo.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.7/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.7/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.7/images/tests-help.png
+-rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.7.7/images/untitled.blend
+-rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.7.7/images/untitled.blend1
+-rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.7.7/images/write-the-docs.gif
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.7/images/write-the-icon.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.7/images/write-the.svg
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cli_main.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_utils.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_utils.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/calculate.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/expected.dat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/multiply.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/__main__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/llm.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cli/main.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cli/tasks.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/__init__.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/docs.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/prompts.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/mkdocs/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/mkdocs/mkdocs.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/mkdocs/templates.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/tests/prompts.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/tests/tests.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 write_the-0.7.7/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.7/LICENSE.txt
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 write_the-0.7.7/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 write_the-0.7.7/PKG-INFO
```

### Comparing `write_the-0.7.6/mkdocs.yml` & `write_the-0.7.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/.github/workflows/publish.yml` & `write_the-0.7.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/.github/workflows/tests.yml` & `write_the-0.7.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/docs/index.md` & `write_the-0.7.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/docs-help.png` & `write_the-0.7.7/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/logo-black.svg` & `write_the-0.7.7/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/logo.png` & `write_the-0.7.7/images/logo.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/mkdocs-help.png` & `write_the-0.7.7/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/multiply-docs-tests.png` & `write_the-0.7.7/images/multiply-docs-tests.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/tests-help.png` & `write_the-0.7.7/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/untitled.blend` & `write_the-0.7.7/images/untitled.blend`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/untitled.blend1` & `write_the-0.7.7/images/untitled.blend1`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/write-the-docs.gif` & `write_the-0.7.7/images/write-the-docs.gif`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/write-the-icon.svg` & `write_the-0.7.7/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/images/write-the.svg` & `write_the-0.7.7/images/write-the.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cli_main.py` & `write_the-0.7.7/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cst_docstring_adder.py` & `write_the-0.7.7/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cst_docstring_remover.py` & `write_the-0.7.7/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cst_function_and_class_collector.py` & `write_the-0.7.7/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cst_node_extractor.py` & `write_the-0.7.7/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cst_node_remover.py` & `write_the-0.7.7/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_cst_utils.py` & `write_the-0.7.7/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/test_utils.py` & `write_the-0.7.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/tests/data/expected.dat` & `write_the-0.7.7/tests/data/expected.dat`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/llm.py` & `write_the-0.7.7/write_the/llm.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/utils.py` & `write_the-0.7.7/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cli/main.py` & `write_the-0.7.7/write_the/cli/main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cli/tasks.py` & `write_the-0.7.7/write_the/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/commands/docs/docs.py` & `write_the-0.7.7/write_the/commands/docs/docs.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/commands/docs/prompts.py` & `write_the-0.7.7/write_the/commands/docs/prompts.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/commands/docs/utils.py` & `write_the-0.7.7/write_the/commands/docs/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/commands/mkdocs/mkdocs.py` & `write_the-0.7.7/write_the/commands/mkdocs/mkdocs.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/commands/mkdocs/templates.py` & `write_the-0.7.7/write_the/commands/mkdocs/templates.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/commands/tests/tests.py` & `write_the-0.7.7/write_the/commands/tests/tests.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cst/docstring_adder.py` & `write_the-0.7.7/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cst/docstring_remover.py` & `write_the-0.7.7/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cst/function_and_class_collector.py` & `write_the-0.7.7/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cst/node_extractor.py` & `write_the-0.7.7/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cst/node_remover.py` & `write_the-0.7.7/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/write_the/cst/utils.py` & `write_the-0.7.7/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/LICENSE.txt` & `write_the-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/README.md` & `write_the-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `write_the-0.7.6/pyproject.toml` & `write_the-0.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "typer[all]",
   "langchain",
   "openai",
+  "pyexpect",
   "tiktoken",
   "black",
   "libcst",
   "mkdocstrings[python]",
   "mkdocs-material"
 ]
 dynamic = ["version"]
```

### Comparing `write_the-0.7.6/PKG-INFO` & `write_the-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.7.6
+Version: 0.7.7
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,14 +18,15 @@
 Requires-Python: >=3.9
 Requires-Dist: black
 Requires-Dist: langchain
 Requires-Dist: libcst
 Requires-Dist: mkdocs-material
 Requires-Dist: mkdocstrings[python]
 Requires-Dist: openai
+Requires-Dist: pyexpect
 Requires-Dist: tiktoken
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/logo.png)
 
 AI-powered Documentation and Test Generation Tool
```

