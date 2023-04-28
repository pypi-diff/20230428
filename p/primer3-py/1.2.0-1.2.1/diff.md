# Comparing `tmp/primer3-py-1.2.0.tar.gz` & `tmp/primer3-py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primer3-py-1.2.0.tar", last modified: Wed Mar 22 11:41:48 2023, max compression
+gzip compressed data, was "primer3-py-1.2.1.tar", last modified: Fri Apr 28 15:44:56 2023, max compression
```

## Comparing `primer3-py-1.2.0.tar` & `primer3-py-1.2.1.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.820445 primer3-py-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-22 11:41:43.000000 primer3-py-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-22 11:41:43.000000 primer3-py-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-03-22 11:41:43.000000 primer3-py-1.2.0/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-03-22 11:41:43.000000 primer3-py-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-22 11:41:43.000000 primer3-py-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-22 11:41:48.820445 primer3-py-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-22 11:41:43.000000 primer3-py-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 11:41:43.000000 primer3-py-1.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.804445 primer3-py-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.804445 primer3-py-1.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/api/bindings.md
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/api/p3helpers.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/api/thermoanalysis.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/changes_link.md
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/cython_help.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/miscellany.md
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-03-22 11:41:43.000000 primer3-py-1.2.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.804445 primer3-py-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-03-22 11:41:43.000000 primer3-py-1.2.0/examples/basicprimerdesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-03-22 11:41:43.000000 primer3-py-1.2.0/examples/orthogonalprimers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.804445 primer3-py-1.2.0/primer3/
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/argdefaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/p3helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/p3helpers.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.800445 primer3-py-1.2.0/primer3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.808445 primer3-py-1.2.0/primer3/src/libprimer3/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/ABOUT.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/amplicontm.c
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/amplicontm.h
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/amplicontm_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    38114 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/dpal.c
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/dpal.h
--rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/format_output.c
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/format_output.h
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/gpl-2.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.808445 primer3-py-1.2.0/primer3/src/libprimer3/klib/
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/klib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/klib/khash.h
--rw-r--r--   0 runner    (1001) docker     (123)   349509 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/libprimer3.c
--rw-r--r--   0 runner    (1001) docker     (123)    58440 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/libprimer3.h
--rw-r--r--   0 runner    (1001) docker     (123)   342261 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/libprimer3flex.c
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/libprimer3flex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/long_seq_tm_test_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/masker.c
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/masker.h
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/masker_main.c
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/ntdpal_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/oligotm.c
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/oligotm.h
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/oligotm_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/p3_seq_lib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/p3_seq_lib.h
--rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_boulder_main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.812445 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/dangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/dangle.ds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.812445 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/loops.dh
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/loops.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stack.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stackmm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stackmm.ds
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tetraloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tetraloop.ds
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/triloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/triloop.ds
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack2.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack2.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds
--rw-r--r--   0 runner    (1001) docker     (123)    24711 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/print_boulder.c
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/print_boulder.h
--rw-r--r--   0 runner    (1001) docker     (123)    57177 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/read_boulder.c
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/read_boulder.h
--rw-r--r--   0 runner    (1001) docker     (123)   107486 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thal.c
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thal_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thal_parameters.c
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thal_parameters.h
--rw-r--r--   0 runner    (1001) docker     (123)    93448 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thalflex.c
--rw-r--r--   0 runner    (1001) docker     (123)    41139 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thalflex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/src/libprimer3/thalflexsignatures.h
--rw-r--r--   0 runner    (1001) docker     (123)    24071 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/thermoanalysis.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    79353 2023-03-22 11:41:43.000000 primer3-py-1.2.0/primer3/thermoanalysis.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.812445 primer3-py-1.2.0/primer3_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-22 11:41:48.000000 primer3-py-1.2.0/primer3_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-03-22 11:41:48.000000 primer3-py-1.2.0/primer3_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:41:48.000000 primer3-py-1.2.0/primer3_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:41:48.000000 primer3-py-1.2.0/primer3_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-22 11:41:48.000000 primer3-py-1.2.0/primer3_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-22 11:41:48.820445 primer3-py-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-03-22 11:41:43.000000 primer3-py-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.812445 primer3-py-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/_simulatedbindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/checkdatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:41:48.820445 primer3-py-1.2.0/tests/input_files/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/dv_conc_vs_dntp_conc_input
--rw-r--r--   0 runner    (1001) docker     (123)   119850 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/long_seq_input
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/p3-tmpl-mispriming_input
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/p3_3_prime_0_input
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/p3_3_prime_n_input
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer1_input
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer1_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer3_v1_1_4_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer3web_v0_4_0_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer3web_v3_0_0_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer3web_v4_0_0_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_all_settingsfiles_input
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_annealing_temp_input
--rw-r--r--   0 runner    (1001) docker     (123)    41194 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_boundary1_input
--rw-r--r--   0 runner    (1001) docker     (123)    45207 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_boundary_input
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_check_input
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_dmso_formamide_input
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_end_pathology_input
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_first_base_index_input
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_gc_end_input
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_high_gc_load_set_input
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_high_tm_load_set_input
--rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_human_input
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_input
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_internal1_input
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_internal_input
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_internal_position_input
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_lib_amb_codes_input
--rw-r--r--   0 runner    (1001) docker     (123)    95632 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_masker_input
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_mispriming_boundary1_input
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_mispriming_boundary2_input
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_mispriming_input
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_mispriming_long_lib_input
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_mispriming_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_must_match_input
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_must_overlap_point_input
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_must_use_input
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_must_use_op_input
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_must_use_th_input
--rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_new_tasks_input
--rw-r--r--   0 runner    (1001) docker     (123)    32303 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_new_tasks_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_num_best_input
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_obj_fn_input
--rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_ok_regions2_input
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_ok_regions_input
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_overhang_input
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_overhang_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_overlap_junction_input
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_poly_x_input
--rw-r--r--   0 runner    (1001) docker     (123)    52293 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_position_penalty_input
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_quality_boundary_input
--rw-r--r--   0 runner    (1001) docker     (123)   141931 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_rat_input
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_renewed_tasks_input
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_sec_struct_dpal_input
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_sec_struct_thal_input
--rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_start_codon_input
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_syntax_input
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_task_input
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_task_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_thal_args_input
--rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_thal_max_seq_error_input
--rwxr-xr-x   0 runner    (1001) docker     (123)    12821 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_thermod_align_input
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_three_prime_distance_input
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_tm_lc_masking_input
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/primer_windows_newlines_input
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/test_compl_error_input
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/test_left_to_right_of_right_input
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/th-w-other-tasks_input
--rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/thal_input
--rwxr-xr-x   0 runner    (1001) docker     (123)    45696 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/input_files/thal_output
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/test_argdefaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/test_ntthal_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/test_p3helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16790 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/test_primerdesign.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/test_thermoanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/test_threadsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-03-22 11:41:43.000000 primer3-py-1.2.0/tests/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.783419 primer3-py-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-28 15:44:48.000000 primer3-py-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-28 15:44:48.000000 primer3-py-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-04-28 15:44:48.000000 primer3-py-1.2.1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-04-28 15:44:48.000000 primer3-py-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 15:44:48.000000 primer3-py-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-28 15:44:56.783419 primer3-py-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-28 15:44:48.000000 primer3-py-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 15:44:48.000000 primer3-py-1.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.763418 primer3-py-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.763418 primer3-py-1.2.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/api/bindings.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/api/p3helpers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/api/thermoanalysis.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/changes_link.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/cython_help.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/miscellany.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-04-28 15:44:48.000000 primer3-py-1.2.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.763418 primer3-py-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-28 15:44:48.000000 primer3-py-1.2.1/examples/basicprimerdesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-28 15:44:48.000000 primer3-py-1.2.1/examples/orthogonalprimers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.767418 primer3-py-1.2.1/primer3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/argdefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/p3helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/p3helpers.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.763418 primer3-py-1.2.1/primer3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.771418 primer3-py-1.2.1/primer3/src/libprimer3/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/ABOUT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/amplicontm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/amplicontm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/amplicontm_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38114 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/dpal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/dpal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/format_output.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/format_output.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/gpl-2.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.771418 primer3-py-1.2.1/primer3/src/libprimer3/klib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/klib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/klib/khash.h
+-rw-r--r--   0 runner    (1001) docker     (123)   349509 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/libprimer3.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58440 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/libprimer3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   342261 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/libprimer3flex.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/libprimer3flex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/long_seq_tm_test_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/masker.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/masker.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/masker_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/ntdpal_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/oligotm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/oligotm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/oligotm_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/p3_seq_lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/p3_seq_lib.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_boulder_main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.771418 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/dangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/dangle.ds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.775418 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/loops.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/loops.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stack.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stackmm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stackmm.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tetraloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tetraloop.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/triloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/triloop.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack2.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack2.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds
+-rw-r--r--   0 runner    (1001) docker     (123)    24711 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/print_boulder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/print_boulder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57177 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/read_boulder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/read_boulder.h
+-rw-r--r--   0 runner    (1001) docker     (123)   107486 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thal_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thal_parameters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thal_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93448 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thalflex.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41139 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thalflex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/src/libprimer3/thalflexsignatures.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24108 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/thermoanalysis.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    79394 2023-04-28 15:44:48.000000 primer3-py-1.2.1/primer3/thermoanalysis.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.775418 primer3-py-1.2.1/primer3_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-28 15:44:56.000000 primer3-py-1.2.1/primer3_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-28 15:44:56.000000 primer3-py-1.2.1/primer3_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:44:56.000000 primer3-py-1.2.1/primer3_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:44:56.000000 primer3-py-1.2.1/primer3_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 15:44:56.000000 primer3-py-1.2.1/primer3_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 15:44:56.783419 primer3-py-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-28 15:44:48.000000 primer3-py-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.775418 primer3-py-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/_simulatedbindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/checkdatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:44:56.783419 primer3-py-1.2.1/tests/input_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/dv_conc_vs_dntp_conc_input
+-rw-r--r--   0 runner    (1001) docker     (123)   119850 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/long_seq_input
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/p3-tmpl-mispriming_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/p3_3_prime_0_input
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/p3_3_prime_n_input
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer1_input
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer1_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer3_v1_1_4_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer3web_v0_4_0_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer3web_v3_0_0_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer3web_v4_0_0_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_all_settingsfiles_input
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_annealing_temp_input
+-rw-r--r--   0 runner    (1001) docker     (123)    41194 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_boundary1_input
+-rw-r--r--   0 runner    (1001) docker     (123)    45207 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_boundary_input
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_check_input
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_dmso_formamide_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_end_pathology_input
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_first_base_index_input
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_gc_end_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_high_gc_load_set_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_high_tm_load_set_input
+-rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_human_input
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_input
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_internal1_input
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_internal_input
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_internal_position_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_lib_amb_codes_input
+-rw-r--r--   0 runner    (1001) docker     (123)    95632 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_masker_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_mispriming_boundary1_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_mispriming_boundary2_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_mispriming_input
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_mispriming_long_lib_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_mispriming_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_must_match_input
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_must_overlap_point_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_must_use_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_must_use_op_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_must_use_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_new_tasks_input
+-rw-r--r--   0 runner    (1001) docker     (123)    32303 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_new_tasks_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_num_best_input
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_obj_fn_input
+-rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_ok_regions2_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_ok_regions_input
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_overhang_input
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_overhang_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_overlap_junction_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_poly_x_input
+-rw-r--r--   0 runner    (1001) docker     (123)    52293 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_position_penalty_input
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_quality_boundary_input
+-rw-r--r--   0 runner    (1001) docker     (123)   141931 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_rat_input
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_renewed_tasks_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_sec_struct_dpal_input
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_sec_struct_thal_input
+-rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_start_codon_input
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_syntax_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_task_input
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_task_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_thal_args_input
+-rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_thal_max_seq_error_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12821 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_thermod_align_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_three_prime_distance_input
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_tm_lc_masking_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/primer_windows_newlines_input
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/test_compl_error_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/test_left_to_right_of_right_input
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/th-w-other-tasks_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/thal_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45696 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/input_files/thal_output
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/test_argdefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/test_ntthal_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/test_p3helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19790 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/test_primerdesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/test_thermoanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/test_threadsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-04-28 15:44:48.000000 primer3-py-1.2.1/tests/wrappers.py
```

### Comparing `primer3-py-1.2.0/.pre-commit-config.yaml` & `primer3-py-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/AUTHORS` & `primer3-py-1.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/CHANGES` & `primer3-py-1.2.1/CHANGES`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## Version 1.2.1 (April 28, 2023)
+- Bug fixes for `pdh_create_seq_lib` to correct missing `seq_lib` datastructure allocation and variable name typos.
+- Increase test coverage to include `misprime_lib` and `mishyb_lib` arguments
+
 ## Version 1.2.0 (March 22, 2023)
 
 - Threadsafe changes made to `thal.c` resulting in new  `thalflex.c` and `thalflex.h` and `thalflexsignatures.h`.
 - Threadsafe changes made to `libprimer3.c` resulting in new  `libprimer3flex.c` and `ibprimer3flex.c.h`.
 - `libprimer3.seq_args` datatype is now renamed to `libprimer3.seq_args_t`
 - `test_threadsafe.py` add and `nogil` instituted for calls to `thal()` and `seqtm()` added `run_design` and `calc_heterodimer` threadsafe tests
 - `ThermoAnalysis` class no longer needs to be a `Singleton` so this was removed as a parent class
```

### Comparing `primer3-py-1.2.0/LICENSE` & `primer3-py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/MANIFEST.in` & `primer3-py-1.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/PKG-INFO` & `primer3-py-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primer3-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python bindings for Primer3
 Home-page: https://github.com/libnano/primer3-py
 Author: Ben Pruitt, Nick Conway
 Author-email: bpruittvt@gmail.com
 License: GPLv2
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: primer3-py Version: 1.2.0 Summary: Python bindings
+Metadata-Version: 2.1 Name: primer3-py Version: 1.2.1 Summary: Python bindings
 for Primer3 Home-page: https://github.com/libnano/primer3-py Author: Ben
 Pruitt, Nick Conway Author-email: bpruittvt@gmail.com License: GPLv2
 Classifier: Programming Language :: C Classifier: Programming Language ::
 Cython Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 4 - Beta
```

### Comparing `primer3-py-1.2.0/README.md` & `primer3-py-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/Makefile` & `primer3-py-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/conf.py` & `primer3-py-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/cython_help.md` & `primer3-py-1.2.1/docs/cython_help.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/index.md` & `primer3-py-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/make.bat` & `primer3-py-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/miscellany.md` & `primer3-py-1.2.1/docs/miscellany.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/docs/quickstart.md` & `primer3-py-1.2.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/examples/basicprimerdesign.py` & `primer3-py-1.2.1/examples/basicprimerdesign.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/examples/orthogonalprimers.py` & `primer3-py-1.2.1/examples/orthogonalprimers.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/__init__.py` & `primer3-py-1.2.1/primer3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 oligonucleotide thermodynamics library.
 
 '''
 import os
 from typing import List
 
 # Per PEP-440 https://peps.python.org/pep-0440/#public-version-identifiers
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 __author__ = 'Ben Pruitt, Nick Conway'
 __copyright__ = (
     'Copyright 2014-2023, Ben Pruitt & Nick Conway; 2014-2018 Wyss Institute'
 )
 __license__ = 'GPLv2'
 DESCRIPTION = 'Python bindings for Primer3'
```

### Comparing `primer3-py-1.2.0/primer3/argdefaults.py` & `primer3-py-1.2.1/primer3/argdefaults.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/bindings.py` & `primer3-py-1.2.1/primer3/bindings.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/p3helpers.h` & `primer3-py-1.2.1/primer3/p3helpers.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/p3helpers.pyx` & `primer3-py-1.2.1/primer3/p3helpers.pyx`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/LICENSE.txt` & `primer3-py-1.2.1/primer3/src/libprimer3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/Makefile` & `primer3-py-1.2.1/primer3/src/libprimer3/Makefile`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/amplicontm.c` & `primer3-py-1.2.1/primer3/src/libprimer3/amplicontm.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/amplicontm.h` & `primer3-py-1.2.1/primer3/src/libprimer3/amplicontm.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/amplicontm_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/amplicontm_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/dpal.c` & `primer3-py-1.2.1/primer3/src/libprimer3/dpal.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/dpal.h` & `primer3-py-1.2.1/primer3/src/libprimer3/dpal.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/format_output.c` & `primer3-py-1.2.1/primer3/src/libprimer3/format_output.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/format_output.h` & `primer3-py-1.2.1/primer3/src/libprimer3/format_output.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/gpl-2.0.txt` & `primer3-py-1.2.1/primer3/src/libprimer3/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/klib/README.md` & `primer3-py-1.2.1/primer3/src/libprimer3/klib/README.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/klib/khash.h` & `primer3-py-1.2.1/primer3/src/libprimer3/klib/khash.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/libprimer3.c` & `primer3-py-1.2.1/primer3/src/libprimer3/libprimer3.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/libprimer3.h` & `primer3-py-1.2.1/primer3/src/libprimer3/libprimer3.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/libprimer3flex.c` & `primer3-py-1.2.1/primer3/src/libprimer3/libprimer3flex.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/libprimer3flex.h` & `primer3-py-1.2.1/primer3/src/libprimer3/libprimer3flex.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/long_seq_tm_test_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/long_seq_tm_test_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/masker.c` & `primer3-py-1.2.1/primer3/src/libprimer3/masker.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/masker.h` & `primer3-py-1.2.1/primer3/src/libprimer3/masker.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/masker_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/masker_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/ntdpal_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/ntdpal_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/oligotm.c` & `primer3-py-1.2.1/primer3/src/libprimer3/oligotm.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/oligotm.h` & `primer3-py-1.2.1/primer3/src/libprimer3/oligotm.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/oligotm_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/oligotm_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/p3_seq_lib.c` & `primer3-py-1.2.1/primer3/src/libprimer3/p3_seq_lib.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/p3_seq_lib.h` & `primer3-py-1.2.1/primer3/src/libprimer3/p3_seq_lib.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_boulder_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_boulder_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/dangle.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/dangle.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/loops.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/loops.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stack.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stack.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stack.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stack.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stackmm.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stackmm.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/stackmm.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/stackmm.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tetraloop.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tetraloop.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tetraloop.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tetraloop.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack2.dh` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack2.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack2.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack2.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds` & `primer3-py-1.2.1/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/print_boulder.c` & `primer3-py-1.2.1/primer3/src/libprimer3/print_boulder.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/print_boulder.h` & `primer3-py-1.2.1/primer3/src/libprimer3/print_boulder.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/read_boulder.c` & `primer3-py-1.2.1/primer3/src/libprimer3/read_boulder.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/read_boulder.h` & `primer3-py-1.2.1/primer3/src/libprimer3/read_boulder.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thal.c` & `primer3-py-1.2.1/primer3/src/libprimer3/thal.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thal.h` & `primer3-py-1.2.1/primer3/src/libprimer3/thal.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thal_main.c` & `primer3-py-1.2.1/primer3/src/libprimer3/thal_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thal_parameters.c` & `primer3-py-1.2.1/primer3/src/libprimer3/thal_parameters.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thal_parameters.h` & `primer3-py-1.2.1/primer3/src/libprimer3/thal_parameters.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thalflex.c` & `primer3-py-1.2.1/primer3/src/libprimer3/thalflex.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thalflex.h` & `primer3-py-1.2.1/primer3/src/libprimer3/thalflex.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/src/libprimer3/thalflexsignatures.h` & `primer3-py-1.2.1/primer3/src/libprimer3/thalflexsignatures.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/primer3/thermoanalysis.pxd` & `primer3-py-1.2.1/primer3/thermoanalysis.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,16 @@
     ctypedef struct pr_append_str:
         int storage_size
         char* data
 
     ctypedef struct seq_lib:
         pass
 
+    seq_lib* create_empty_seq_lib()
+
     int seq_lib_num_seq(const seq_lib* lib)
 
     void destroy_seq_lib(seq_lib *lib)
     int add_seq_to_seq_lib(seq_lib *, char *, char *, const char *)
     void reverse_complement_seq_lib(seq_lib  *lib)
```

### Comparing `primer3-py-1.2.0/primer3/thermoanalysis.pyx` & `primer3-py-1.2.1/primer3/thermoanalysis.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1400,23 +1400,24 @@
 
     cdef:
         seq_lib* sl = NULL
         char* seq_name_c = NULL
         char* seq_c = NULL
         char* errfrag = NULL
 
+    sl = create_empty_seq_lib()
     if sl == NULL:
         raise OSError('Could not allocate memory for seq_lib')
 
     for seq_name_str, seq_str in seq_dict.items():
         if isinstance(seq_name_str, str):
             seq_name_b = seq_name_str.encode('utf8')
-            seq_name = seq_name_b
+            seq_name_c = seq_name_b
         elif isinstance(seq_name_str, bytes):
-            seq_name = seq_name
+            seq_name_c = seq_name_str
         else:
             destroy_seq_lib(sl)
             raise TypeError(
                 'Cannot add seq name with non-Unicode/Bytes type to seq_lib',
             )
 
         if isinstance(seq_str, str):
@@ -1431,14 +1432,15 @@
             )
 
         if add_seq_to_seq_lib(sl, seq_c, seq_name_c, errfrag) == 1:
             err_msg_b =  <bytes> errfrag
             destroy_seq_lib(sl)
             raise OSError(err_msg_b.decode('utf8'))
     reverse_complement_seq_lib(sl)
+
     return sl
 
 
 cdef object pdh_design_output_to_dict(
         const p3_global_settings* global_settings_data,
         const seq_args_t* sequence_args_data,
         const p3retval *retval,
```

### Comparing `primer3-py-1.2.0/primer3_py.egg-info/PKG-INFO` & `primer3-py-1.2.1/primer3_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primer3-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python bindings for Primer3
 Home-page: https://github.com/libnano/primer3-py
 Author: Ben Pruitt, Nick Conway
 Author-email: bpruittvt@gmail.com
 License: GPLv2
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: primer3-py Version: 1.2.0 Summary: Python bindings
+Metadata-Version: 2.1 Name: primer3-py Version: 1.2.1 Summary: Python bindings
 for Primer3 Home-page: https://github.com/libnano/primer3-py Author: Ben
 Pruitt, Nick Conway Author-email: bpruittvt@gmail.com License: GPLv2
 Classifier: Programming Language :: C Classifier: Programming Language ::
 Cython Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 4 - Beta
```

### Comparing `primer3-py-1.2.0/primer3_py.egg-info/SOURCES.txt` & `primer3-py-1.2.1/primer3_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/setup.py` & `primer3-py-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/_simulatedbindings.py` & `primer3-py-1.2.1/tests/_simulatedbindings.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/checkdatasets.py` & `primer3-py-1.2.1/tests/checkdatasets.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/long_seq_input` & `primer3-py-1.2.1/tests/input_files/long_seq_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/p3-tmpl-mispriming_input` & `primer3-py-1.2.1/tests/input_files/p3-tmpl-mispriming_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/p3_3_prime_0_input` & `primer3-py-1.2.1/tests/input_files/p3_3_prime_0_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/p3_3_prime_n_input` & `primer3-py-1.2.1/tests/input_files/p3_3_prime_n_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer1_input` & `primer3-py-1.2.1/tests/input_files/primer1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer1_th_input` & `primer3-py-1.2.1/tests/input_files/primer1_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer3_v1_1_4_default_settings_input` & `primer3-py-1.2.1/tests/input_files/primer3_v1_1_4_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer3web_v0_4_0_default_settings_input` & `primer3-py-1.2.1/tests/input_files/primer3web_v0_4_0_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer3web_v3_0_0_default_settings_input` & `primer3-py-1.2.1/tests/input_files/primer3web_v3_0_0_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer3web_v4_0_0_default_settings_input` & `primer3-py-1.2.1/tests/input_files/primer3web_v4_0_0_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_all_settingsfiles_input` & `primer3-py-1.2.1/tests/input_files/primer_all_settingsfiles_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_annealing_temp_input` & `primer3-py-1.2.1/tests/input_files/primer_annealing_temp_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_boundary1_input` & `primer3-py-1.2.1/tests/input_files/primer_boundary1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_boundary_input` & `primer3-py-1.2.1/tests/input_files/primer_boundary_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_check_input` & `primer3-py-1.2.1/tests/input_files/primer_check_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_dmso_formamide_input` & `primer3-py-1.2.1/tests/input_files/primer_dmso_formamide_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_end_pathology_input` & `primer3-py-1.2.1/tests/input_files/primer_end_pathology_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_first_base_index_input` & `primer3-py-1.2.1/tests/input_files/primer_first_base_index_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_gc_end_input` & `primer3-py-1.2.1/tests/input_files/primer_gc_end_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_high_gc_load_set_input` & `primer3-py-1.2.1/tests/input_files/primer_high_gc_load_set_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_high_tm_load_set_input` & `primer3-py-1.2.1/tests/input_files/primer_high_tm_load_set_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_human_input` & `primer3-py-1.2.1/tests/input_files/primer_human_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_input` & `primer3-py-1.2.1/tests/input_files/primer_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_internal1_input` & `primer3-py-1.2.1/tests/input_files/primer_internal1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_internal_input` & `primer3-py-1.2.1/tests/input_files/primer_internal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_internal_position_input` & `primer3-py-1.2.1/tests/input_files/primer_internal_position_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_lib_amb_codes_input` & `primer3-py-1.2.1/tests/input_files/primer_lib_amb_codes_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_masker_input` & `primer3-py-1.2.1/tests/input_files/primer_masker_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_mispriming_boundary1_input` & `primer3-py-1.2.1/tests/input_files/primer_mispriming_boundary1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_mispriming_boundary2_input` & `primer3-py-1.2.1/tests/input_files/primer_mispriming_boundary2_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_mispriming_input` & `primer3-py-1.2.1/tests/input_files/primer_mispriming_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_mispriming_long_lib_input` & `primer3-py-1.2.1/tests/input_files/primer_mispriming_long_lib_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_mispriming_th_input` & `primer3-py-1.2.1/tests/input_files/primer_mispriming_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_must_match_input` & `primer3-py-1.2.1/tests/input_files/primer_must_match_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_must_overlap_point_input` & `primer3-py-1.2.1/tests/input_files/primer_must_overlap_point_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_must_use_input` & `primer3-py-1.2.1/tests/input_files/primer_must_use_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_must_use_op_input` & `primer3-py-1.2.1/tests/input_files/primer_must_use_op_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_must_use_th_input` & `primer3-py-1.2.1/tests/input_files/primer_must_use_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_new_tasks_input` & `primer3-py-1.2.1/tests/input_files/primer_new_tasks_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_new_tasks_th_input` & `primer3-py-1.2.1/tests/input_files/primer_new_tasks_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_num_best_input` & `primer3-py-1.2.1/tests/input_files/primer_num_best_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_obj_fn_input` & `primer3-py-1.2.1/tests/input_files/primer_obj_fn_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_ok_regions2_input` & `primer3-py-1.2.1/tests/input_files/primer_ok_regions2_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_ok_regions_input` & `primer3-py-1.2.1/tests/input_files/primer_ok_regions_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_overhang_input` & `primer3-py-1.2.1/tests/input_files/primer_overhang_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_overhang_th_input` & `primer3-py-1.2.1/tests/input_files/primer_overhang_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_overlap_junction_input` & `primer3-py-1.2.1/tests/input_files/primer_overlap_junction_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_poly_x_input` & `primer3-py-1.2.1/tests/input_files/primer_poly_x_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_position_penalty_input` & `primer3-py-1.2.1/tests/input_files/primer_position_penalty_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_quality_boundary_input` & `primer3-py-1.2.1/tests/input_files/primer_quality_boundary_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_rat_input` & `primer3-py-1.2.1/tests/input_files/primer_rat_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_renewed_tasks_input` & `primer3-py-1.2.1/tests/input_files/primer_renewed_tasks_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_sec_struct_dpal_input` & `primer3-py-1.2.1/tests/input_files/primer_sec_struct_dpal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_sec_struct_thal_input` & `primer3-py-1.2.1/tests/input_files/primer_sec_struct_thal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_start_codon_input` & `primer3-py-1.2.1/tests/input_files/primer_start_codon_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_syntax_input` & `primer3-py-1.2.1/tests/input_files/primer_syntax_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_task_input` & `primer3-py-1.2.1/tests/input_files/primer_task_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_task_th_input` & `primer3-py-1.2.1/tests/input_files/primer_task_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_thal_args_input` & `primer3-py-1.2.1/tests/input_files/primer_thal_args_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_thal_max_seq_error_input` & `primer3-py-1.2.1/tests/input_files/primer_thal_max_seq_error_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_thermod_align_input` & `primer3-py-1.2.1/tests/input_files/primer_thermod_align_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_three_prime_distance_input` & `primer3-py-1.2.1/tests/input_files/primer_three_prime_distance_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_tm_lc_masking_input` & `primer3-py-1.2.1/tests/input_files/primer_tm_lc_masking_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/primer_windows_newlines_input` & `primer3-py-1.2.1/tests/input_files/primer_windows_newlines_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/test_left_to_right_of_right_input` & `primer3-py-1.2.1/tests/input_files/test_left_to_right_of_right_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/th-w-other-tasks_input` & `primer3-py-1.2.1/tests/input_files/th-w-other-tasks_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/thal_input` & `primer3-py-1.2.1/tests/input_files/thal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/input_files/thal_output` & `primer3-py-1.2.1/tests/input_files/thal_output`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/test_argdefaults.py` & `primer3-py-1.2.1/tests/test_argdefaults.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/test_ntthal_io.py` & `primer3-py-1.2.1/tests/test_ntthal_io.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/test_p3helpers.py` & `primer3-py-1.2.1/tests/test_p3helpers.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/test_primerdesign.py` & `primer3-py-1.2.1/tests/test_primerdesign.py`

 * *Files 10% similar despite different names*

```diff
@@ -448,14 +448,93 @@
         if em - sm > delta_bytes_limit:
             raise AssertionError(
                 f'Memory usage increase after {run_count} runs of \n\t'
                 f'design_primers > {delta_bytes_limit} bytes -- potential \n\t'
                 f'memory leak (mem increase: {em - sm})',
             )
 
+    def test_misprime_lib_mishyb_lib(self):
+        '''Test that the misprime library and mishyb library arguments
+        successfully run through the bindings.
+
+        '''
+        seq_args = {
+            'SEQUENCE_ID': 'MH1000',
+            'SEQUENCE_TEMPLATE': (
+                'GCTTGCATGCCTGCAGGTCGACTCTAGAGGATCCCCCTACATTTT'
+                'AGCATCAGTGAGTACAGCATGCTTACTGGAAGAGAGGGTCATGCA'
+                'ACAGATTAGGAGGTAAGTTTGCAAAGGCAGGCTAAGGAGGAGACG'
+                'CACTGAATGCCATGGTAAGAACTCTGGACATAAAAATATTGGAAG'
+                'TTGTTGAGCAAGTNAAAAAAATGTTTGGAAGTGTTACTTTAGCAA'
+                'TGGCAAGAATGATAGTATGGAATAGATTGGCAGAATGAAGGCAAA'
+                'ATGATTAGACATATTGCATTAAGGTAAAAAATGATAACTGAAGAA'
+                'TTATGTGCCACACTTATTAATAAGAAAGAATATGTGAACCTTGCA'
+                'GATGTTTCCCTCTAGTAG'
+            ),
+            'SEQUENCE_INCLUDED_REGION': [36, 342],
+        }
+        global_args = {
+            'PRIMER_OPT_SIZE': 20,
+            'PRIMER_PICK_INTERNAL_OLIGO': 1,
+            'PRIMER_INTERNAL_MAX_SELF_END': 8,
+            'PRIMER_MIN_SIZE': 18,
+            'PRIMER_MAX_SIZE': 25,
+            'PRIMER_OPT_TM': 60.0,
+            'PRIMER_MIN_TM': 57.0,
+            'PRIMER_MAX_TM': 63.0,
+            'PRIMER_MIN_GC': 20.0,
+            'PRIMER_MAX_GC': 80.0,
+            'PRIMER_MAX_POLY_X': 100,
+            'PRIMER_INTERNAL_MAX_POLY_X': 100,
+            'PRIMER_SALT_MONOVALENT': 50.0,
+            'PRIMER_DNA_CONC': 50.0,
+            'PRIMER_MAX_NS_ACCEPTED': 0,
+            'PRIMER_MAX_SELF_ANY': 12,
+            'PRIMER_MAX_SELF_END': 8,
+            'PRIMER_PAIR_MAX_COMPL_ANY': 12,
+            'PRIMER_PAIR_MAX_COMPL_END': 8,
+            'PRIMER_PRODUCT_SIZE_RANGE': [
+                [75, 100], [100, 125], [125, 150],
+                [150, 175], [175, 200], [200, 225],
+            ],
+        }
+
+        result = bindings.design_primers(
+            seq_args=seq_args,
+            global_args=global_args,
+            misprime_lib={
+                'SEQ1': 'CACCATGGAGCTCCTGATATTAAAGGCGAATGCCATT',
+            },
+        )
+        self.assertEqual(result['PRIMER_PAIR_NUM_RETURNED'], 5)
+        self.assertEqual(result['PRIMER_LEFT_0'], [46, 21])
+
+        result = bindings.design_primers(
+            seq_args=seq_args,
+            global_args=global_args,
+            mishyb_lib={
+                'SEQ1': 'TTATGTGCCACACTTATTAATAAGAAAGAATATGTGAACCTTGCA',
+            },
+        )
+        self.assertEqual(result['PRIMER_PAIR_NUM_RETURNED'], 5)
+        self.assertEqual(result['PRIMER_LEFT_0'], [46, 21])
+
+        bindings.design_primers(
+            seq_args=seq_args,
+            global_args=global_args,
+            misprime_lib={
+                'SEQ1': 'CACCATGGAGCTCCTGATATTAAAGGCGAATGCCATT',
+            },
+            mishyb_lib={
+                'SEQ1': 'TTATGTGCCACACTTATTAATAAGAAAGAATATGTGAACCTTGCA',
+            },
+        )
+        self.assertEqual(result['PRIMER_PAIR_NUM_RETURNED'], 5)
+        self.assertEqual(result['PRIMER_LEFT_0'], [46, 21])
+
 
 def suite():
     suite = unittest.TestSuite()
     suite.addTest(TestDesignBindings())
     return suite
```

### Comparing `primer3-py-1.2.0/tests/test_thermoanalysis.py` & `primer3-py-1.2.1/tests/test_thermoanalysis.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/test_threadsafe.py` & `primer3-py-1.2.1/tests/test_threadsafe.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.0/tests/wrappers.py` & `primer3-py-1.2.1/tests/wrappers.py`

 * *Files identical despite different names*

