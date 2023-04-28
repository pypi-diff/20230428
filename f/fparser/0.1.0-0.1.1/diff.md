# Comparing `tmp/fparser-0.1.0.tar.gz` & `tmp/fparser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fparser-0.1.0.tar", last modified: Tue Apr 18 07:31:30 2023, max compression
+gzip compressed data, was "fparser-0.1.1.tar", last modified: Fri Apr 28 16:00:39 2023, max compression
```

## Comparing `fparser-0.1.0.tar` & `fparser-0.1.1.tar`

### file list

```diff
@@ -1,241 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.915221 fparser-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 07:31:15.000000 fparser-0.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.863220 fparser-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.871220 fparser-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 07:31:15.000000 fparser-0.1.0/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-18 07:31:15.000000 fparser-0.1.0/.github/workflows/unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 07:31:15.000000 fparser-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-18 07:31:15.000000 fparser-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-18 07:31:15.000000 fparser-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-18 07:31:15.000000 fparser-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-18 07:31:30.915221 fparser-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-18 07:31:15.000000 fparser-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.871220 fparser-0.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   114630 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/doxygen.config
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/pip_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.871220 fparser-0.1.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    42926 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/developers_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/fparser.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/fparser2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-18 07:31:15.000000 fparser-0.1.0/doc/source/reference_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.871220 fparser-0.1.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-18 07:31:15.000000 fparser-0.1.0/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-18 07:31:15.000000 fparser-0.1.0/example/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     6102 2023-04-18 07:31:15.000000 fparser-0.1.0/example/create_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-18 07:31:15.000000 fparser-0.1.0/example/fparser2_f2008.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.875220 fparser-0.1.0/example/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 07:31:15.000000 fparser-0.1.0/example/test_files/a.f90
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 07:31:15.000000 fparser-0.1.0/example/test_files/b.f90
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 07:31:15.000000 fparser-0.1.0/example/test_files/c.f90
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-18 07:31:15.000000 fparser-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 07:31:30.915221 fparser-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-04-18 07:31:15.000000 fparser-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.863220 fparser-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.875220 fparser-0.1.0/src/fparser/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.879220 fparser-0.1.0/src/fparser/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35934 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    62920 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/readfortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/splitline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.879220 fparser-0.1.0/src/fparser/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/modfile.f95
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/test_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    48185 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/test_readfortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/test_sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/test_splitline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/utf.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/tests/utf_in_code.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.879220 fparser-0.1.0/src/fparser/one/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51336 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/block_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/parsefortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    78902 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.883220 fparser-0.1.0/src/fparser/one/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/bad_char.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/test_block_stmts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/test_do_block_r814.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/test_parsefortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    38497 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    24502 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/one/typedecl_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.883220 fparser-0.1.0/src/fparser/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5268 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/fparser2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3985 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/fparser2_bench.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4640 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/parse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4934 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/script_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.883220 fparser-0.1.0/src/fparser/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/tests/test_fparser2_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/scripts/tests/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.887220 fparser-0.1.0/src/fparser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/funcfile.f95
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/modfile.f95
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_blank_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_f90comment_f77source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_fparser_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue10.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue23.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue25.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue26.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue33.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue7.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_issue9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/tests/test_mod_private.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.891220 fparser-0.1.0/src/fparser/two/
--rw-r--r--   0 runner    (1001) docker     (123)    24469 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/C99Preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)   379425 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/Fortran2003.py
--rw-r--r--   0 runner    (1001) docker     (123)    53562 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/Fortran2008.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/pattern_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/symbol_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.895221 fparser-0.1.0/src/fparser/two/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.907221 fparser-0.1.0/src/fparser/two/tests/fortran2003/
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_add_operand_r705.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_case_construct_r808.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_char_expr_r725.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_component_part_r438.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_data_ref_r612.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_designator_r603.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_forall_header_r754.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_item_c1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_item_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_item_r1003.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_hollerith_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_if_construct_r802.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_include_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_include_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_int_expr_r727.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_kindselector_r404.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_main_program_r1101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_module_r1104.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_name_r304.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_prefix_r1227.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_primary_r701.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_program_r201.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_rename_r1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_where_construct_r744.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.915221 fparser-0.1.0/src/fparser/two/tests/fortran2008/
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_critical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_program_unit_r202.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_submodule_r1116.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_bases.py
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_c99preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)   100844 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_fortran2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_module_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_pattern_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_symbol_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.915221 fparser-0.1.0/src/fparser/two/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_binaryopbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_blockbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_bracket_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_call_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_get_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_sequencebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_stringbase_upper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/tests/utils/test_wordclsbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    70927 2023-04-18 07:31:15.000000 fparser-0.1.0/src/fparser/two/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:31:30.875220 fparser-0.1.0/src/fparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 07:31:30.000000 fparser-0.1.0/src/fparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.167790 fparser-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 16:00:25.000000 fparser-0.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.131790 fparser-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.135790 fparser-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-28 16:00:25.000000 fparser-0.1.1/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-28 16:00:25.000000 fparser-0.1.1/.github/workflows/unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-28 16:00:25.000000 fparser-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-04-28 16:00:25.000000 fparser-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-28 16:00:25.000000 fparser-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-28 16:00:25.000000 fparser-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 16:00:39.167790 fparser-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-28 16:00:25.000000 fparser-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.135790 fparser-0.1.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   114630 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/doxygen.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/pip_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42926 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/developers_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/fparser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/fparser2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/reference_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 16:00:25.000000 fparser-0.1.1/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-28 16:00:25.000000 fparser-0.1.1/example/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6102 2023-04-28 16:00:25.000000 fparser-0.1.1/example/create_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-28 16:00:25.000000 fparser-0.1.1/example/fparser2_f2008.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/example/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 16:00:25.000000 fparser-0.1.1/example/test_files/a.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 16:00:25.000000 fparser-0.1.1/example/test_files/b.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 16:00:25.000000 fparser-0.1.1/example/test_files/c.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 16:00:25.000000 fparser-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-28 16:00:39.167790 fparser-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-04-28 16:00:25.000000 fparser-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.131790 fparser-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/src/fparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/src/fparser/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35934 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62920 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/readfortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/splitline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.143790 fparser-0.1.1/src/fparser/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/modfile.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48185 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_readfortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_splitline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/utf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/utf_in_code.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.143790 fparser-0.1.1/src/fparser/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51336 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/block_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/parsefortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78902 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.143790 fparser-0.1.1/src/fparser/one/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/bad_char.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_block_stmts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_do_block_r814.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_parsefortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38497 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24502 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/typedecl_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.147790 fparser-0.1.1/src/fparser/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5268 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/fparser2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3985 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/fparser2_bench.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4640 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4934 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/script_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.147790 fparser-0.1.1/src/fparser/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/tests/test_fparser2_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.151790 fparser-0.1.1/src/fparser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/funcfile.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/modfile.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_blank_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_f90comment_f77source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_fparser_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue26.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_mod_private.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.151790 fparser-0.1.1/src/fparser/two/
+-rw-r--r--   0 runner    (1001) docker     (123)    24469 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/C99Preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   379425 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/Fortran2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55113 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/Fortran2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/pattern_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/symbol_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.151790 fparser-0.1.1/src/fparser/two/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.163790 fparser-0.1.1/src/fparser/two/tests/fortran2003/
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_add_operand_r705.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_case_construct_r808.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_expr_r725.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_component_part_r438.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_ref_r612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_designator_r603.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_header_r754.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_c1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_r1003.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_hollerith_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_construct_r802.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_int_expr_r727.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_kindselector_r404.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_main_program_r1101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_module_r1104.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_name_r304.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_prefix_r1227.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_primary_r701.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_r201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_rename_r1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_where_construct_r744.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.167790 fparser-0.1.1/src/fparser/two/tests/fortran2008/
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_critical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_program_unit_r202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_r1116.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_c99preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100962 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_fortran2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_module_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_pattern_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_symbol_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.167790 fparser-0.1.1/src/fparser/two/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_binaryopbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_blockbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_bracket_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_call_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_get_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_sequencebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_stringbase_upper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_wordclsbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70927 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/src/fparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/top_level.txt
```

### Comparing `fparser-0.1.0/.github/workflows/python_publish.yml` & `fparser-0.1.1/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/.github/workflows/unit-tests.yml` & `fparser-0.1.1/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/.gitignore` & `fparser-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/CHANGELOG.md` & `fparser-0.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 * A. R. Porter, Science & Technology Facilities Council, UK
 * B. Reuter, ECMWF, UK
 * S. Siso, Science & Technology Facilities Council, UK
 * J. Tiira, University of Helsinki, Finland
 * P. Vitt, University of Siegen, Germany
 * A. Voysey, UK Met Office
 
+26/04/2023 PR #406 for #405. Add support for F2008 optional "::" in PROCEDURE
+           statement.
+
 03/04/2023 PR #392 for #326. Add support for F2008 block and critical constructs.
 
 30/03/2023 PR #396 for #395. Fix trailing whitespace bug in CallBase.
 
 13/03/2023 PR #391 for #324. Add GH workfow to automate a pypi upload during
            GH releases.
```

### Comparing `fparser-0.1.0/LICENSE` & `fparser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/MANIFEST.in` & `fparser-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/PKG-INFO` & `fparser-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fparser
-Version: 0.1.0
+Version: 0.1.1
 Summary: The fparser project
 Home-page: https://github.com/stfc/fparser
 Author: Pearu Peterson, Rupert Ford, Andrew Porter
 Author-email: andrew.porter@stfc.ac.uk
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/stfc/fparser
 Project-URL: Tracker, https://github.com/stfc/fparser/issues
@@ -25,14 +25,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
 License-File: LICENSE
 
 # News #
 
+  * 18/04/2023 Version 0.1.0 released and status changed from `alpha` to `beta`. See the [CHANGELOG](CHANGELOG.md) for more details.
   * 16/06/2022 Version 0.0.16 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 30/05/2022 Version 0.0.15 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 10/03/2022 Version 0.0.14 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 02/11/2021 Version 0.0.13 released. See the [CHANGELOG](CHANGELOG.md)
```

### Comparing `fparser-0.1.0/README.md` & `fparser-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # News #
 
+  * 18/04/2023 Version 0.1.0 released and status changed from `alpha` to `beta`. See the [CHANGELOG](CHANGELOG.md) for more details.
   * 16/06/2022 Version 0.0.16 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 30/05/2022 Version 0.0.15 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 10/03/2022 Version 0.0.14 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 02/11/2021 Version 0.0.13 released. See the [CHANGELOG](CHANGELOG.md)
```

### Comparing `fparser-0.1.0/doc/Makefile` & `fparser-0.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/doxygen.config` & `fparser-0.1.1/doc/doxygen.config`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/pip_requirements.txt` & `fparser-0.1.1/doc/pip_requirements.txt`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/conf.py` & `fparser-0.1.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/developers_guide.rst` & `fparser-0.1.1/doc/source/developers_guide.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/fparser.rst` & `fparser-0.1.1/doc/source/fparser.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/fparser2.rst` & `fparser-0.1.1/doc/source/fparser2.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,18 @@
 ========
 
 Fparser2 provides support for parsing Fortran up to and including
 Fortran 2003. This is implemented in the Fortran2003.py `file`__ and
 contains an entirely separate parser to fparser1 that includes rules
 for Fortran 2003 syntax. Support for Fortran 2008 is being added in
 the Fortran2008.py `file`__ which extends the Fortran2003 rules
-appropriately. At this time fparser2 supports submodules, co-arrays,
-the 'mold' argument to allocate and the 'contiguous' keyword in Fortran2008.
+appropriately. At this time fparser2 supports the following
+Fortran2008 features: submodules, co-arrays, the 'mold' argument to
+allocate, the 'contiguous' keyword, the 'BLOCK' construct, the
+'CRITICAL' construct and the optional '::' for a procedure statement.
 
 __ https://github.com/stfc/fparser/blob/master/src/fparser/two/Fortran2003.py
 __ https://github.com/stfc/fparser/blob/master/src/fparser/two/Fortran2008.py
 
 
 Getting Going : Script
 ----------------------
```

### Comparing `fparser-0.1.0/doc/source/index.rst` & `fparser-0.1.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/introduction.rst` & `fparser-0.1.1/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/license.rst` & `fparser-0.1.1/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/doc/source/reference_guide.rst` & `fparser-0.1.1/doc/source/reference_guide.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/example/Makefile` & `fparser-0.1.1/example/Makefile`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/example/README.md` & `fparser-0.1.1/example/README.md`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/example/create_dependencies.py` & `fparser-0.1.1/example/create_dependencies.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/example/fparser2_f2008.py` & `fparser-0.1.1/example/fparser2_f2008.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/setup.cfg` & `fparser-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/setup.py` & `fparser-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/.pylintrc` & `fparser-0.1.1/src/fparser/.pylintrc`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/__init__.py` & `fparser-0.1.1/src/fparser/__init__.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/api.py` & `fparser-0.1.1/src/fparser/api.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/base_classes.py` & `fparser-0.1.1/src/fparser/common/base_classes.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/readfortran.py` & `fparser-0.1.1/src/fparser/common/readfortran.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/sourceinfo.py` & `fparser-0.1.1/src/fparser/common/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/splitline.py` & `fparser-0.1.1/src/fparser/common/splitline.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/conftest.py` & `fparser-0.1.1/src/fparser/common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/logging_utils.py` & `fparser-0.1.1/src/fparser/common/tests/logging_utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/modfile.f95` & `fparser-0.1.1/src/fparser/common/tests/modfile.f95`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/test_base_classes.py` & `fparser-0.1.1/src/fparser/common/tests/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/test_readfortran.py` & `fparser-0.1.1/src/fparser/common/tests/test_readfortran.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/test_sourceinfo.py` & `fparser-0.1.1/src/fparser/common/tests/test_sourceinfo.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/test_splitline.py` & `fparser-0.1.1/src/fparser/common/tests/test_splitline.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/test_utils.py` & `fparser-0.1.1/src/fparser/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/utf.f90` & `fparser-0.1.1/src/fparser/common/tests/utf.f90`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/tests/utf_in_code.f90` & `fparser-0.1.1/src/fparser/common/tests/utf_in_code.f90`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/common/utils.py` & `fparser-0.1.1/src/fparser/common/utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/conftest.py` & `fparser-0.1.1/src/fparser/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/block_statements.py` & `fparser-0.1.1/src/fparser/one/block_statements.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/parsefortran.py` & `fparser-0.1.1/src/fparser/one/parsefortran.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/statements.py` & `fparser-0.1.1/src/fparser/one/statements.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/bad_char.f90` & `fparser-0.1.1/src/fparser/one/tests/bad_char.f90`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/test_block_stmts.py` & `fparser-0.1.1/src/fparser/one/tests/test_block_stmts.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/test_do_block_r814.py` & `fparser-0.1.1/src/fparser/one/tests/test_do_block_r814.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/test_parsefortran.py` & `fparser-0.1.1/src/fparser/one/tests/test_parsefortran.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/test_parser.py` & `fparser-0.1.1/src/fparser/one/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/test_scripts.py` & `fparser-0.1.1/src/fparser/one/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/tests/test_select.py` & `fparser-0.1.1/src/fparser/one/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/one/typedecl_statements.py` & `fparser-0.1.1/src/fparser/one/typedecl_statements.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/README.md` & `fparser-0.1.1/src/fparser/scripts/README.md`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/fparser2.py` & `fparser-0.1.1/src/fparser/scripts/fparser2.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/fparser2_bench.py` & `fparser-0.1.1/src/fparser/scripts/fparser2_bench.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/parse.py` & `fparser-0.1.1/src/fparser/scripts/parse.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/read.py` & `fparser-0.1.1/src/fparser/scripts/read.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/script_options.py` & `fparser-0.1.1/src/fparser/scripts/script_options.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/tests/test_fparser2_bench.py` & `fparser-0.1.1/src/fparser/scripts/tests/test_fparser2_bench.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/scripts/tests/test_scripts.py` & `fparser-0.1.1/src/fparser/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/funcfile.f95` & `fparser-0.1.1/src/fparser/tests/funcfile.f95`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/modfile.f95` & `fparser-0.1.1/src/fparser/tests/modfile.f95`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_api.py` & `fparser-0.1.1/src/fparser/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_blank_lines.py` & `fparser-0.1.1/src/fparser/tests/test_blank_lines.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_comment.py` & `fparser-0.1.1/src/fparser/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_f90comment_f77source.py` & `fparser-0.1.1/src/fparser/tests/test_f90comment_f77source.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_fparser_module.py` & `fparser-0.1.1/src/fparser/tests/test_fparser_module.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_functional.py` & `fparser-0.1.1/src/fparser/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue10.py` & `fparser-0.1.1/src/fparser/tests/test_issue10.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue11.py` & `fparser-0.1.1/src/fparser/tests/test_issue11.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue23.py` & `fparser-0.1.1/src/fparser/tests/test_issue23.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue25.py` & `fparser-0.1.1/src/fparser/tests/test_issue25.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue26.py` & `fparser-0.1.1/src/fparser/tests/test_issue26.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue33.py` & `fparser-0.1.1/src/fparser/tests/test_issue33.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue4.py` & `fparser-0.1.1/src/fparser/tests/test_issue4.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue5.py` & `fparser-0.1.1/src/fparser/tests/test_issue5.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue7.py` & `fparser-0.1.1/src/fparser/tests/test_issue7.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue8.py` & `fparser-0.1.1/src/fparser/tests/test_issue8.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_issue9.py` & `fparser-0.1.1/src/fparser/tests/test_issue9.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/tests/test_mod_private.py` & `fparser-0.1.1/src/fparser/tests/test_mod_private.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/C99Preprocessor.py` & `fparser-0.1.1/src/fparser/two/C99Preprocessor.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/Fortran2003.py` & `fparser-0.1.1/src/fparser/two/Fortran2003.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/Fortran2008.py` & `fparser-0.1.1/src/fparser/two/Fortran2008.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     Connect_Spec as Connect_Spec_2003,
     Data_Component_Def_Stmt as Data_Component_Def_Stmt_2003,
     Do_Term_Action_Stmt as Do_Term_Action_Stmt_2003,
     Executable_Construct as Executable_Construct_2003,
     Executable_Construct_C201 as Executable_Construct_C201_2003,
     If_Stmt as If_Stmt_2003,
     Open_Stmt as Open_Stmt_2003,
+    Procedure_Stmt as Procedure_Stmt_2003,
     Program_Unit as Program_Unit_2003,
     Type_Declaration_Stmt as Type_Declaration_Stmt_2003,
 )
 
 
 class Program_Unit(Program_Unit_2003):  # R202
     """
@@ -161,15 +162,15 @@
     subclass_names = Program_Unit_2003.subclass_names[:]
     subclass_names.append("Submodule")
 
 
 class Executable_Construct(Executable_Construct_2003):  # R213
     # pylint: disable=invalid-name
     """
-    Fortran 2003 rule R213.
+    Fortran 2008 rule R213.
 
     .. code-block:: fortran
 
         executable-construct is action-stmt
                              or associate-construct
                              or block-construct
                              or case-construct
@@ -1574,14 +1575,62 @@
 
         """
         return EndStmtBase.match(
             "CRITICAL", Critical_Construct_Name, string, require_stmt_type=True
         )
 
 
+class Procedure_Stmt(Procedure_Stmt_2003):  # R1206
+    """
+    Fortran 2008 Rule 1206.
+
+    procedure-stmt is [ MODULE ] PROCEDURE [ :: ] procedure-name-list
+
+    """
+
+    @staticmethod
+    def match(string):
+        """:param str string: Fortran code to check for a match
+
+        :returns: 3-tuple containing a boolean indicating whether the \
+            optional MODULE keyword is included, a boolean indicating \
+            whether the optional '::' is included and a Procedure_Name_List \
+            instance, or None if there is no match.
+        :rtype: Optional[Tuple[ \
+            bool, bool, \
+            :py:class:`fparser.two.Fortran2003.Procedure_Name_List`]]]
+
+        """
+        line = string.lstrip()
+        optional_module = None
+        if line[:6].upper() == "MODULE":
+            line = line[6:].lstrip()
+            optional_module = "MODULE"
+        if line[:9].upper() != "PROCEDURE":
+            return None
+        line = line[9:].lstrip()
+        optional_colons = None
+        if line[:2] == "::":
+            line = line[2:].lstrip()
+            optional_colons = "::"
+        return (Procedure_Name_List(line), optional_module, optional_colons)
+
+    def tostr(self):
+        """
+        :returns: the string representation of this node.
+        :rtype: str
+        """
+        result = "PROCEDURE"
+        if self.items[1]:
+            result = f"MODULE {result}"
+        if self.items[2]:
+            result = f"{result} ::"
+        return f"{result} {self.items[0]}"
+
+
 #
 # GENERATE Scalar_, _List, _Name CLASSES
 #
 
 
 ClassType = type(Base)
 _names = dir()
```

### Comparing `fparser-0.1.0/src/fparser/two/parser.py` & `fparser-0.1.1/src/fparser/two/parser.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/pattern_tools.py` & `fparser-0.1.1/src/fparser/two/pattern_tools.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/symbol_table.py` & `fparser-0.1.1/src/fparser/two/symbol_table.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/.pylintrc` & `fparser-0.1.1/src/fparser/two/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/conftest.py` & `fparser-0.1.1/src/fparser/two/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/conftest.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_add_operand_r705.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_add_operand_r705.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_case_construct_r808.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_case_construct_r808.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_char_expr_r725.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_expr_r725.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_component_part_r438.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_component_part_r438.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_data_ref_r612.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_ref_r612.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_designator_r603.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_designator_r603.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_forall_header_r754.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_header_r754.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_item_c1002.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_c1002.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_item_list.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_list.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_item_r1003.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_r1003.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_hollerith_item.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_hollerith_item.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_if_construct_r802.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_construct_r802.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_include_filename.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_filename.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_include_statement.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_statement.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_int_expr_r727.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_int_expr_r727.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_intrinsics.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_kindselector_r404.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_kindselector_r404.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_main_program_r1101.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_main_program_r1101.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_module_r1104.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_module_r1104.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_name_r304.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_name_r304.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_prefix_r1227.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_prefix_r1227.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_primary_r701.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_primary_r701.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_program_r201.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_r201.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_rename_r1111.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_rename_r1111.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_where_construct_r744.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_where_construct_r744.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/conftest.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_block.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_block.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_critical.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_critical.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_program_unit_r202.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_program_unit_r202.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_submodule_r1116.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_r1116.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py` & `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_bases.py` & `fparser-0.1.1/src/fparser/two/tests/test_bases.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_c99preprocessor.py` & `fparser-0.1.1/src/fparser/two/tests/test_c99preprocessor.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_comments.py` & `fparser-0.1.1/src/fparser/two/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_fortran2003.py` & `fparser-0.1.1/src/fparser/two/tests/test_fortran2003.py`

 * *Files 0% similar despite different names*

```diff
@@ -2960,14 +2960,18 @@
     assert isinstance(obj, tcls), repr(obj)
     assert str(obj) == "MODULE PROCEDURE a"
 
     obj = tcls("procedure a, b")
     assert isinstance(obj, tcls), repr(obj)
     assert str(obj) == "MODULE PROCEDURE a, b"
 
+    # '::' is only valid from F2008 onwards
+    with pytest.raises(NoMatchError):
+        _ = tcls("procedure :: a")
+
 
 def test_generic_spec():  # R1207
     tcls = Generic_Spec
     obj = tcls("a")
     assert isinstance(obj, Name), repr(obj)
     assert str(obj) == "a"
     obj = tcls("read(formatted)")
```

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_module_use.py` & `fparser-0.1.1/src/fparser/two/tests/test_module_use.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_parser.py` & `fparser-0.1.1/src/fparser/two/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_pattern_tools.py` & `fparser-0.1.1/src/fparser/two/tests/test_pattern_tools.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_symbol_table.py` & `fparser-0.1.1/src/fparser/two/tests/test_symbol_table.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_symbol_tables.py` & `fparser-0.1.1/src/fparser/two/tests/test_symbol_tables.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/test_utils.py` & `fparser-0.1.1/src/fparser/two/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_base.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_base.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_binaryopbase.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_binaryopbase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_blockbase.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_blockbase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_bracket_base.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_bracket_base.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_call_base.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_call_base.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_get_child.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_get_child.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_sequencebase.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_sequencebase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_stringbase_upper.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_stringbase_upper.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_walk.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_walk.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/tests/utils/test_wordclsbase.py` & `fparser-0.1.1/src/fparser/two/tests/utils/test_wordclsbase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser/two/utils.py` & `fparser-0.1.1/src/fparser/two/utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.0/src/fparser.egg-info/PKG-INFO` & `fparser-0.1.1/src/fparser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fparser
-Version: 0.1.0
+Version: 0.1.1
 Summary: The fparser project
 Home-page: https://github.com/stfc/fparser
 Author: Pearu Peterson, Rupert Ford, Andrew Porter
 Author-email: andrew.porter@stfc.ac.uk
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/stfc/fparser
 Project-URL: Tracker, https://github.com/stfc/fparser/issues
@@ -25,14 +25,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
 License-File: LICENSE
 
 # News #
 
+  * 18/04/2023 Version 0.1.0 released and status changed from `alpha` to `beta`. See the [CHANGELOG](CHANGELOG.md) for more details.
   * 16/06/2022 Version 0.0.16 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 30/05/2022 Version 0.0.15 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 10/03/2022 Version 0.0.14 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 02/11/2021 Version 0.0.13 released. See the [CHANGELOG](CHANGELOG.md)
```

### Comparing `fparser-0.1.0/src/fparser.egg-info/SOURCES.txt` & `fparser-0.1.1/src/fparser.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,15 @@
 src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py
 src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py
 src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py
 src/fparser/two/tests/fortran2008/test_if_stmt_r837.py
 src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py
 src/fparser/two/tests/fortran2008/test_open_stmt_r904.py
 src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py
+src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py
 src/fparser/two/tests/fortran2008/test_program_unit_r202.py
 src/fparser/two/tests/fortran2008/test_submodule_r1116.py
 src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py
 src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py
 src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py
 src/fparser/two/tests/utils/test_base.py
 src/fparser/two/tests/utils/test_binaryopbase.py
```

