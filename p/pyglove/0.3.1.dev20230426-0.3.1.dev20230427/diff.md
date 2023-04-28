# Comparing `tmp/pyglove-0.3.1.dev20230426.tar.gz` & `tmp/pyglove-0.3.1.dev20230427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230426.tar", last modified: Wed Apr 26 08:07:03 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230427.tar", last modified: Thu Apr 27 08:06:28 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230426.tar` & `pyglove-0.3.1.dev20230427.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.621081 pyglove-0.3.1.dev20230426/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-26 08:07:03.617081 pyglove-0.3.1.dev20230426/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-26 08:07:01.000000 pyglove-0.3.1.dev20230426/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.593081 pyglove-0.3.1.dev20230426/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.593081 pyglove-0.3.1.dev20230426/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.597081 pyglove-0.3.1.dev20230426/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.597081 pyglove-0.3.1.dev20230426/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.601081 pyglove-0.3.1.dev20230426/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.605081 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.605081 pyglove-0.3.1.dev20230426/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.609081 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21550 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27851 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.609081 pyglove-0.3.1.dev20230426/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.613081 pyglove-0.3.1.dev20230426/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45015 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    77141 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93868 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.613081 pyglove-0.3.1.dev20230426/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.613081 pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.617081 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.617081 pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.617081 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/ext/scalars/step_wise_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/pyglove/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:07:03.593081 pyglove-0.3.1.dev20230426/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-26 08:07:03.000000 pyglove-0.3.1.dev20230426/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-26 08:07:03.000000 pyglove-0.3.1.dev20230426/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:07:03.000000 pyglove-0.3.1.dev20230426/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 08:07:03.000000 pyglove-0.3.1.dev20230426/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:07:03.000000 pyglove-0.3.1.dev20230426/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:07:03.621081 pyglove-0.3.1.dev20230426/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-26 08:06:44.000000 pyglove-0.3.1.dev20230426/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:28.001044 pyglove-0.3.1.dev20230427/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-27 08:06:28.001044 pyglove-0.3.1.dev20230427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-27 08:06:26.000000 pyglove-0.3.1.dev20230427/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.985044 pyglove-0.3.1.dev20230427/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.985044 pyglove-0.3.1.dev20230427/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.985044 pyglove-0.3.1.dev20230427/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.989044 pyglove-0.3.1.dev20230427/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.989044 pyglove-0.3.1.dev20230427/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.993044 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.993044 pyglove-0.3.1.dev20230427/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.993044 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21550 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27851 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.997044 pyglove-0.3.1.dev20230427/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.997044 pyglove-0.3.1.dev20230427/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47479 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81524 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106307 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.997044 pyglove-0.3.1.dev20230427/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.997044 pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:28.001044 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:28.001044 pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:28.001044 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/ext/scalars/step_wise_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/pyglove/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:06:27.985044 pyglove-0.3.1.dev20230427/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-27 08:06:27.000000 pyglove-0.3.1.dev20230427/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-27 08:06:27.000000 pyglove-0.3.1.dev20230427/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:06:27.000000 pyglove-0.3.1.dev20230427/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 08:06:27.000000 pyglove-0.3.1.dev20230427/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:06:27.000000 pyglove-0.3.1.dev20230427/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:06:28.001044 pyglove-0.3.1.dev20230427/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-27 08:06:13.000000 pyglove-0.3.1.dev20230427/setup.py
```

### Comparing `pyglove-0.3.1.dev20230426/LICENSE` & `pyglove-0.3.1.dev20230427/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/PKG-INFO` & `pyglove-0.3.1.dev20230427/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230426
+Version: 0.3.1.dev20230427
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230426/README.md` & `pyglove-0.3.1.dev20230427/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230427/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,38 @@
   @property
   def is_space(self) -> bool:
     return False
 
 
 # pylint: disable=line-too-long
 @functools.total_ordering
+@symbolic.members([
+    (
+        'value',
+        pg_typing.Union(
+            [pg_typing.Int(), pg_typing.Float(), pg_typing.Str()]
+        ).noneable(),
+        'Value of DNA node.',
+    ),
+    (
+        'children',
+        pg_typing.List(pg_typing.Object('DNA'), default=[]),
+        (
+            'DNA list as child nodes for template members or '
+            'chosen candidates of choices.'
+        ),
+    ),
+    (
+        'metadata',
+        pg_typing.Dict(
+            [(pg_typing.StrKey(), pg_typing.Any(), 'Key-value pairs.')]
+        ),
+        'Metadata assigned to the DNA.',
+    ),
+])
 class DNA(symbolic.Object):
   """The genome of a symbolic object relative to its search space.
 
   DNA is a hierarchical structure - each DNA node has a value, and a list of
   child DNA nodes. The root node represents the genome that encodes an entire
   object relative to its space. The value of a DNA node could be None, an
   integer, a float number or a string, dependening on its specification
@@ -1684,30 +1708,14 @@
     return cls.from_dict(parameters, dna_spec)
 
   def __str__(self) -> str:
     """Use compact form as string representation."""
     return self.format(compact=True)
 
 
-# NOTE(daiyip): members is declared separately as a function call since
-# decorator requires DNA to be defined before used as a part of value spec
-# of 'children' field.
-symbolic.members([
-    ('value', pg_typing.Union([
-        pg_typing.Int(), pg_typing.Float(), pg_typing.Str()]).noneable(),
-     'Value of DNA node.'),
-    ('children', pg_typing.List(pg_typing.Object(DNA), default=[]),
-     ('DNA list as child nodes for template members or '
-      'chosen candidates of choices.')),
-    ('metadata', pg_typing.Dict([
-        (pg_typing.StrKey(), pg_typing.Any(), 'Key-value pairs.')
-    ]), 'Metadata assigned to the DNA.')
-])(DNA)
-
-
 class ConditionalKey:
   """Key used in :class:`pyglove.KeyPath` to represent conditional element.
 
   For example, `a[=1].b` means `a.b` when `a == 1`.
   `a[0][=0][0]` means `a[0][0]` when `a[0] == 0`.
   """
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230427/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,15 @@
 
 # Class schema.
 from pyglove.core.typing.class_schema import KeySpec
 from pyglove.core.typing.class_schema import ValueSpec
 from pyglove.core.typing.class_schema import Field
 from pyglove.core.typing.class_schema import Schema
 from pyglove.core.typing.class_schema import create_schema
+from pyglove.core.typing.class_schema import ForwardRef
 
 # Class schema helpers.
 from pyglove.core.typing.class_schema_utils import get_init_signature
 from pyglove.core.typing.class_schema_utils import get_arg_fields
 from pyglove.core.typing.class_schema_utils import ensure_value_spec
 
 # Concrete key specifications.
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Schema definition for symbolic classes and lists/dicts."""
 
 import abc
 import copy
+import functools
+import inspect
 import sys
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
+import types
+from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple, Type, Union
 
 from pyglove.core import object_utils
 
 
 class KeySpec(object_utils.Formattable):
   """Interface for key specifications.
 
@@ -87,14 +90,84 @@
 
   @classmethod
   def from_str(cls, key: str) -> 'KeySpec':
     """Get a concrete ValueSpec from annotation."""
     assert False, 'Overridden in `key_specs.py`.'
 
 
+class ForwardRef(object_utils.Formattable):
+  """Forward type reference."""
+
+  def __init__(self, module: types.ModuleType, name: str):
+    self._module = module
+    self._name = name
+
+  @property
+  def module(self) -> types.ModuleType:
+    """Returns the module where the name is being referenced."""
+    return self._module
+
+  @property
+  def name(self) -> str:
+    """Returns the name of the type reference."""
+    return self._name
+
+  @property
+  def qualname(self) -> str:
+    """Returns the qualified name of the reference."""
+    return f'{self.module.__name__}.{self.name}'
+
+  def as_annotation(self) -> Union[Type[Any], str]:
+    """Returns the forward reference as an annotation."""
+    return self.cls if self.resolved else self.name
+
+  @property
+  def resolved(self) -> bool:
+    """Returns True if the symbol for the name is resolved.."""
+    return hasattr(self.module, self.name)
+
+  @functools.cached_property
+  def cls(self) -> Type[Any]:
+    """Returns the resolved reference class.."""
+    reference = getattr(self.module, self.name, None)
+    if reference is None:
+      raise TypeError(
+          f'{self.name!r} does not exist in module {self.module.__name__!r}'
+      )
+    elif not inspect.isclass(reference):
+      raise TypeError(
+          f'{self.name!r} from module {self.module.__name__!r} is not a class.'
+      )
+    return reference
+
+  def format(self, *args, **kwargs) -> str:
+    """Format this object."""
+    details = object_utils.kvlist_str([
+        ('module', self.module.__name__, None),
+        ('name', self.name, None),
+    ])
+    return f'{self.__class__.__name__}({details})'
+
+  def __eq__(self, other: Any) -> bool:
+    """Operator==."""
+    if self is other:
+      return True
+    elif isinstance(other, ForwardRef):
+      return self.module is other.module and self.name == other.name
+    elif inspect.isclass(other):
+      return self.resolved and self.cls is other
+
+  def __ne__(self, other: Any) -> bool:
+    """Operator!=."""
+    return not self.__eq__(other)
+
+  def __hash__(self) -> int:
+    return hash((self.module, self.name))
+
+
 class ValueSpec(object_utils.Formattable):
   """Interface for value specifications.
 
   A value specification defines what values are acceptable for a symbolic
   field (see :class:`pyglove.Field`). When assignments take place on the
   attributes for the field, the associated ValueSpec object will kick in to
   intercept the process and take care of the following aspects:
@@ -238,15 +311,20 @@
   """
 
   @property
   @abc.abstractmethod
   def value_type(self) -> Union[
       Type[Any],
       Tuple[Type[Any], ...]]:  # pyformat: disable
-    """Returns acceptable value type(s)."""
+    """Returns acceptable (resolved) value type(s)."""
+
+  @property
+  @abc.abstractmethod
+  def forward_refs(self) -> Set[ForwardRef]:
+    """Returns forward referenes used by the value spec."""
 
   @abc.abstractmethod
   def noneable(self) -> 'ValueSpec':
     """Marks none-able and returns `self`."""
 
   @property
   @abc.abstractmethod
@@ -412,14 +490,19 @@
       KeyError: If additional key is found in value, or required key is missing
         and allow_partial is set to False.
       TypeError: If type of value is not the same as spec required.
       ValueError: If value is not acceptable, or value is MISSING_VALUE while
         allow_partial is set to False.
     """
 
+  @property
+  def type_resolved(self) -> bool:
+    """Returns True if all forward references are resolved."""
+    return not any(not ref.resolved for ref in self.forward_refs)
+
   def __ne__(self, other: Any) -> bool:
     """Operator !=."""
     return not self.__eq__(other)
 
   def __repr__(self) -> str:
     """Operator repr."""
     return self.format(compact=True)
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,26 +11,82 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.core.typing.class_schema."""
 
 import copy
 import inspect
+import sys
 from typing import Optional, Union, List
 import unittest
 
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import custom_typing
 from pyglove.core.typing import key_specs as ks
 from pyglove.core.typing import typed_missing
 from pyglove.core.typing import value_specs as vs
 from pyglove.core.typing.class_schema import Field
 from pyglove.core.typing.class_schema import Schema
 
 
+class ForwardRefTest(unittest.TestCase):
+  """Test for `ForwardRef` class."""
+
+  def setUp(self):
+    super().setUp()
+    self._module = sys.modules[__name__]
+
+  def test_basics(self):
+    r = class_schema.ForwardRef(self._module, 'FieldTest')
+    self.assertIs(r.module, self._module)
+    self.assertEqual(r.name, 'FieldTest')
+    self.assertEqual(r.qualname, f'{self._module.__name__}.FieldTest')
+
+  def test_resolved(self):
+    self.assertTrue(class_schema.ForwardRef(self._module, 'FieldTest').resolved)
+    self.assertFalse(class_schema.ForwardRef(self._module, 'Foo').resolved)
+
+  def test_as_annotation(self):
+    self.assertEqual(
+        class_schema.ForwardRef(self._module, 'FieldTest').as_annotation(),
+        FieldTest,
+    )
+    self.assertEqual(
+        class_schema.ForwardRef(self._module, 'Foo').as_annotation(), 'Foo'
+    )
+
+  def test_cls(self):
+    self.assertIs(
+        class_schema.ForwardRef(self._module, 'FieldTest').cls, FieldTest
+    )
+
+    with self.assertRaisesRegex(TypeError, '.* does not exist in module'):
+      _ = class_schema.ForwardRef(self._module, 'Foo').cls
+
+    with self.assertRaisesRegex(TypeError, '.* is not a class'):
+      _ = class_schema.ForwardRef(self._module, 'unittest').cls
+
+  def test_format(self):
+    self.assertEqual(
+        str(class_schema.ForwardRef(self._module, 'FieldTest')),
+        f'ForwardRef(module={self._module.__name__}, name=FieldTest)',
+    )
+
+  def test_eq_ne(self):
+    ref = class_schema.ForwardRef(self._module, 'FieldTest')
+    self.assertEqual(ref, ref)
+    self.assertEqual(ref, class_schema.ForwardRef(self._module, 'FieldTest'))
+    self.assertEqual(ref, FieldTest)
+    self.assertEqual(FieldTest, ref)
+
+    self.assertNotEqual(int, ref)
+    self.assertNotEqual(ref, class_schema.ForwardRef(unittest, 'FieldTest'))
+    self.assertNotEqual(ref, class_schema.ForwardRef(self._module, 'Foo'))
+
+
 class FieldTest(unittest.TestCase):
   """Test for `Field` class."""
 
   def test_basics(self):
     f = Field('a', vs.Int(max_value=10), 'a field')
     self.assertIsInstance(f.key, ks.ConstStrKey)
     self.assertEqual(f.key, 'a')
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/value_specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Concrete value specifications for field definition."""
-
 import copy
+import functools
 import inspect
 import numbers
 import re
 import sys
 import typing
+import __main__
+
 from pyglove.core import object_utils
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import key_specs
 from pyglove.core.typing import type_conversion
 from pyglove.core.typing import typed_missing
 from pyglove.core.typing.class_schema import Field
@@ -98,14 +100,19 @@
       None,
       typing.Type[typing.Any],
       typing.Tuple[typing.Type[typing.Any], ...]]:  # pyformat: disable
     """Returns acceptable value type(s) for current value spec."""
     return self._value_type
 
   @property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns no forward references by default, subclasses can override."""
+    return set()
+
+  @property
   def default(self) -> typing.Any:
     """Returns the default value."""
     return self._default
 
   def set_default(self,
                   default: typing.Any,
                   use_default_apply: bool = True) -> ValueSpec:
@@ -212,21 +219,23 @@
           root_path,
           self,
           allow_partial=allow_partial,
           child_transform=child_transform)
       if not should_continue:
         return value
 
-    if self._value_type is not None and not isinstance(value, self._value_type):
+    if (self.type_resolved
+        and self.value_type is not None
+        and not isinstance(value, self.value_type)):
       converter = type_conversion.get_first_applicable_converter(
-          type(value), self._value_type)
+          type(value), self.value_type)
       if converter is None:
         raise TypeError(
             object_utils.message_on_path(
-                f'Expect {self._value_type} '
+                f'Expect {self.value_type} '
                 f'but encountered {type(value)!r}: {value}.', root_path))
       value = converter(value)
 
     # NOTE(daiyip): child nodes validation and transformation is done before
     # parent nodes, which makes sure when child_transform is called on current
     # node (which is in Field.apply), input are in good shape.
     # It also lets users to create complex object types from transform function
@@ -279,34 +288,30 @@
     annotation = self._annotate()
     if annotation != MISSING_VALUE and self.is_noneable:
       return typing.Optional[annotation]
     return annotation
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
-    return self._value_type
+    return self.value_type
 
   def __eq__(self, other: typing.Any) -> bool:
     """Operator==."""
     if self is other:
       return True
-    if not isinstance(other, self.__class__):
+    if (not isinstance(other, self.__class__)
+        or self.default != other.default
+        or self.is_noneable != other.is_noneable
+        or self.frozen != other.frozen):
       return False
-    if isinstance(self._value_type, tuple):
-      self_value_types = list(self._value_type)
-    else:
-      self_value_types = [self._value_type]
-    if isinstance(other.value_type, tuple):
-      other_value_types = list(other.value_type)
-    else:
-      other_value_types = [self._value_type]
-    return (set(self_value_types) == set(other_value_types)
-            and self.default == other.default
-            and self.is_noneable == other.is_noneable
-            and self.frozen == other.frozen)
+    return self._eq(other)
+
+  def _eq(self, other: 'ValueSpec') -> bool:
+    """Subclasses can override."""
+    return True
 
   def format(self, **kwargs) -> str:
     """Format this object."""
     details = object_utils.kvlist_str([
         ('default', object_utils.quote_if_str(self._default), MISSING_VALUE),
         ('noneable', self._is_noneable, False),
         ('frozen', self._frozen, False)
@@ -441,19 +446,16 @@
         ('default', object_utils.quote_if_str(self._default), MISSING_VALUE),
         ('regex', object_utils.quote_if_str(regex_pattern), None),
         ('noneable', self._is_noneable, False),
         ('frozen', self._frozen, False)
     ])
     return f'{self.__class__.__name__}({details})'
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return super().__eq__(other) and self.regex == other.regex
+  def _eq(self, other: 'Str') -> bool:
+    return self.regex == other.regex
 
 
 class Number(PrimitiveType):
   """Base class for value spec of numeric types."""
 
   def __init__(
       self,
@@ -529,21 +531,17 @@
       if other.min_value is None or other.min_value < self._min_value:
         return False
     if self._max_value is not None:
       if other.max_value is None or other.max_value > self._max_value:
         return False
     return True
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return (super().__eq__(other) and
-            self.min_value == other.min_value and
-            self.max_value == other.max_value)
+  def _eq(self, other: 'Number') -> bool:
+    return (self.min_value == other.min_value
+            and self.max_value == other.max_value)
 
   def format(self, **kwargs) -> str:
     """Format this object."""
     details = object_utils.kvlist_str([
         ('default', self._default, MISSING_VALUE),
         ('min', self._min_value, None),
         ('max', self._max_value, None),
@@ -716,27 +714,22 @@
     for v in other.values:
       if v not in self.values:
         return False
     return True
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
-    if self._value_type == str:
+    if self.value_type == str:
       return str
-    if self._value_type is None:
+    if self.value_type is None:
       return typing.Any
-    return self._value_type
+    return self.value_type
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return (super().__eq__(other)
-            and self._default == other._default  # pylint: disable=protected-access
-            and self.values == other.values)
+  def _eq(self, other: 'Enum') -> bool:
+    return self.values == other.values
 
   def format(self, **kwargs) -> str:
     """Format this object."""
     details = object_utils.kvlist_str([
         ('default', object_utils.quote_if_str(self._default), MISSING_VALUE),
         ('values', self._values, None),
         ('frozen', self._frozen, False),
@@ -816,14 +809,19 @@
 
   @property
   def element(self) -> Field:
     """Returns Field specification of list element."""
     return self._element
 
   @property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    return self._element.value.forward_refs
+
+  @property
   def min_size(self) -> int:
     """Returns max size of the list."""
     return self._element.key.min_value  # pytype: disable=attribute-error  # bind-properties
 
   @property
   def max_size(self) -> typing.Optional[int]:
     """Returns max size of the list."""
@@ -880,19 +878,16 @@
         return False
     return self._element.value.is_compatible(other.element.value)
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
     return typing.List[_any_if_no_annotation(self._element.value.annotation)]
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return super().__eq__(other) and self.element == other.element
+  def _eq(self, other: 'List') -> bool:
+    return self.element == other.element
 
   def format(self,
              compact: bool = False,
              verbose: bool = True,
              root_indent: int = 0,
              hide_default_values: bool = True,
              hide_missing_values: bool = True,
@@ -1037,14 +1032,22 @@
     return self._max_size
 
   @property
   def elements(self) -> typing.List[Field]:
     """Returns Field specification for tuple elements."""
     return self._elements
 
+  @functools.cached_property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    forward_refs = set()
+    for elem in self.elements:
+      forward_refs.update(elem.value.forward_refs)
+    return forward_refs
+
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
     if self.fixed_length:
       return typing.Tuple[tuple([
           _any_if_no_annotation(elem.value.annotation)
           for elem in self._elements])]       # pytype: disable=invalid-annotation
     else:
@@ -1149,20 +1152,16 @@
       if self.min_size > other.min_size:
         return False
       if self.max_size is not None and (
           other.max_size is None or self.max_size < other.max_size):
         return False
       return self.elements[0].value.is_compatible(other.elements[0].value)
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return (super().__eq__(other)
-            and self.elements == other.elements
+  def _eq(self, other: typing.Any) -> bool:
+    return (self.elements == other.elements
             and self.min_size == other.min_size
             and self.max_size == other.max_size)
 
   def format(self,
              compact: bool = False,
              verbose: bool = True,
              root_indent: int = 0,
@@ -1290,14 +1289,24 @@
 
   def noneable(self) -> 'Dict':
     """Override noneable in Dict to always set default value None."""
     self._is_noneable = True
     self._default = None
     return self
 
+  @functools.cached_property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    if self.schema is None:
+      return set()
+    forward_refs = set()
+    for field in self.schema.fields.values():
+      forward_refs.update(field.value.forward_refs)
+    return forward_refs
+
   def _apply(self,
              value: typing.Dict[typing.Any, typing.Any],
              allow_partial: bool,
              child_transform: typing.Callable[
                  [object_utils.KeyPath, Field, typing.Any], typing.Any],
              root_path: object_utils.KeyPath) -> typing.Any:
     """Dict specific apply."""
@@ -1323,19 +1332,16 @@
       return self._schema.is_compatible(other.schema)
     return True
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
     return typing.Dict[str, typing.Any]
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return super().__eq__(other) and self.schema == other.schema
+  def _eq(self, other: 'Dict') -> bool:
+    return self.schema == other.schema
 
   def format(self,
              compact: bool = False,
              verbose: bool = True,
              root_indent: int = 0,
              **kwargs) -> str:
     """Format this object."""
@@ -1361,24 +1367,27 @@
   """Value spec for object type.
 
   Examples::
 
     # A required instance of class A and its subclasses.
     pg.typing.Object(A)
 
+    # A required instance of class A and its subclasses (forward declaration).
+    pg.typing.Object('A')
+
     # An optional instance of class A with None as its default value.
     pg.typing.Object(A).noneable()
 
     # An instance of class A with default value.
     pg.typing.Object(A, default=A())
   """
 
   def __init__(
       self,
-      cls: typing.Type[typing.Any],
+      cls: typing.Union[typing.Type[typing.Any], str],
       default: typing.Any = MISSING_VALUE,
       user_validator: typing.Optional[
           typing.Callable[[typing.Any], None]] = None):
     """Constructor.
 
     Args:
       cls: Class of the object. Objects of subclass of this class is acceptable.
@@ -1386,24 +1395,44 @@
       user_validator: (Optional) user function or callable object for additional
         validation on the applied object, which can reject a value by raising
         Exceptions. Please note that this validation is an addition to
         validating object type constraint.
     """
     if cls is None:
       raise TypeError('"cls" for Object spec cannot be None.')
-    if not isinstance(cls, type):
-      raise TypeError('"cls" for Object spec should be a type.')
-    if cls is object:
-      raise TypeError('<class \'object\'> is too general for Object spec.')
+
+    forward_ref = None
+    if isinstance(cls, str):
+      forward_ref = class_schema.ForwardRef(_get_spec_callsite_module(), cls)
+    elif isinstance(cls, type):
+      if cls is object:
+        raise TypeError('<class \'object\'> is too general for Object spec.')
+    else:
+      raise TypeError('"cls" for Object spec should be a type or str.')
+
+    self._forward_ref = forward_ref
     super().__init__(cls, default, user_validator)
 
   @property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    if self._forward_ref is None:
+      return set()
+    return set([self._forward_ref])
+
+  @property
   def cls(self) -> typing.Type[typing.Any]:
     """Returns the class of this object spec."""
-    return self.value_type
+    if self._forward_ref is None:
+      return typing.cast(typing.Type[typing.Any], self._value_type)
+    return self._forward_ref.cls
+
+  @property
+  def value_type(self) -> typing.Type[typing.Any]:
+    return self.cls
 
   def _apply(self,
              value: typing.Any,
              allow_partial: bool,
              child_transform: typing.Callable[
                  [object_utils.KeyPath, Field, typing.Any], typing.Any],
              root_path: object_utils.KeyPath) -> typing.Any:
@@ -1420,47 +1449,57 @@
     """Extend current value spec on top of a base spec."""
     if isinstance(base, Callable) and base.is_compatible(self):
       return self
     return super().extend(base)
 
   def _extend(self, base: 'Object') -> None:
     """Object specific extension."""
-    if not issubclass(self.value_type, base.value_type):
+    if not base.is_compatible(self):
       raise TypeError(f'{self!r} cannot extend {base!r}: incompatible class.')
 
   def _is_compatible(self, other: 'Object') -> bool:
     """Object specific compatiblity check."""
+    # NOTE(daiyip): When either the current spec or the other spec contains
+    # unresolved forward declarations, we consider them compatible.
+    if not self.type_resolved or not other.type_resolved:
+      return True
     return issubclass(other.cls, self.cls)
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
-    return self.cls
+    if self._forward_ref is not None:
+      return self._forward_ref.as_annotation()
+    return self._value_type
 
   @property
   def schema(self) -> typing.Optional[Schema]:
     """Returns the schema of object class if available."""
     return getattr(self.value_type, 'schema', None)
 
-  def __eq__(self, other: typing.Any) -> bool:
+  def _eq(self, other: 'Object') -> bool:
     """Operator==."""
-    if self is other:
-      return True
-    return (super().__eq__(other) and
-            self.value_type == other.value_type)
+    if self.type_resolved:
+      return self.value_type == other.value_type
+    return self.forward_refs == other.forward_refs
 
   def format(self,
              compact: bool = False,
              verbose: bool = True,
              root_indent: int = 0,
              hide_default_values: bool = True,
              hide_missing_values: bool = True,
              **kwargs) -> str:
     """Format this object."""
+    if self._forward_ref is not None:
+      name = self._forward_ref.name
+    else:
+      name = self._value_type.__name__
+
     details = object_utils.kvlist_str([
-        ('', self._value_type.__name__, None),
+        ('', name, None),
         ('default', object_utils.format(
             self._default,
             compact,
             verbose,
             root_indent,
             hide_default_values=hide_default_values,
             hide_missing_values=hide_missing_values,
@@ -1535,14 +1574,26 @@
       raise TypeError(
           f'\'returns\' should be a ValueSpec object. Encountered: {returns!r}')
     self._args = args
     self._kw = kw
     self._return_value = returns
     super().__init__(callable_type, default, user_validator)
 
+  @functools.cached_property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    forward_refs = set()
+    for arg in self.args:
+      forward_refs.update(arg.forward_refs)
+    for _, arg in self.kw:
+      forward_refs.update(arg.forward_refs)
+    if self.return_value:
+      forward_refs.update(self.return_value.forward_refs)
+    return forward_refs
+
   @property
   def args(self) -> typing.List[ValueSpec]:
     """Value specs for positional arguments."""
     return self._args
 
   @property
   def kw(self) -> typing.List[typing.Tuple[str, ValueSpec]]:
@@ -1691,18 +1742,16 @@
 
     if self._return_value:
       return_value = _any_if_no_annotation(self._return_value.annotation)
     else:
       return_value = None
     return typing.Callable[args, return_value]  # pytype: disable=invalid-annotation
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    return (super().__eq__(other)
-            and self._args == other.args
+  def _eq(self, other: 'Callable') -> bool:
+    return (self._args == other.args
             and self._kw == other.kw
             and self._return_value == other.return_value)
 
   def format(self, **kwargs) -> str:
     """Format this spec."""
     details = object_utils.kvlist_str([
         ('args', object_utils.format(self._args, **kwargs), '[]'),
@@ -1768,65 +1817,89 @@
   """Value spec for type.
 
   Examples::
 
     # A required type or subclass of A.
     pg.typing.Type(A)
 
+    # An required type or subclass of A (forward declaration).
+    pg.typing.Type('A')
+
     # An optional type or subclass of A.
     pg.typing.Type(A).noneable()
 
     # A required type or subclass of A with default value B
     # (B is a subclass of A).
     pg.typing.Type(A, default=B)
-
   """
 
   def __init__(
       self,
-      t: typing.Type,  # pylint: disable=g-bare-generic
+      t: typing.Union[typing.Type[typing.Any], str],
       default: typing.Type = MISSING_VALUE):  # pylint: disable=g-bare-generic  # pytype: disable=annotation-type-mismatch
-    if not isinstance(t, type):
+    forward_ref = None
+    if isinstance(t, str):
+      forward_ref = class_schema.ForwardRef(_get_spec_callsite_module(), t)
+    elif not isinstance(t, type):
       raise TypeError(f'{t!r} is not a type.')
     self._expected_type = t
+    self._forward_ref = forward_ref
     super().__init__(type, default)
 
   @property
-  def type(self):
+  def type(self) -> typing.Type[typing.Any]:
     """Returns desired type."""
+    if self._forward_ref is not None:
+      return self._forward_ref.cls
     return self._expected_type
 
+  @functools.cached_property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    if self._forward_ref is None:
+      return set()
+    return set([self._forward_ref])
+
   def _validate(self, path: object_utils.KeyPath, value: typing.Type) -> None:  # pylint: disable=g-bare-generic
     """Validate applied value."""
-    if not issubclass(value, self.type):
+    if self.type_resolved and not issubclass(value, self.type):
       raise ValueError(
           object_utils.message_on_path(
               f'{value!r} is not a subclass of {self.type!r}', path))
 
   def _is_compatible(self, other: 'Type') -> bool:
     """Type specific compatiblity check."""
+    # NOTE(daiyip): When either the current spec or the other spec contains
+    # unresolved forward declarations, we consider them compatible.
+    if not self.type_resolved or not other.type_resolved:
+      return True
     return issubclass(other.type, self.type)
 
   def _extend(self, base: 'Type') -> None:
     """Type specific extension."""
-    if not issubclass(self.type, base.type):
+    if not base.is_compatible(self):
       raise TypeError(f'{self!r} cannot extend {base!r}: incompatible type.')
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
-    return typing.Type[self._expected_type]
+    expected_type = self._expected_type
+    if self._forward_ref is not None:
+      expected_type = self._forward_ref.as_annotation()
+    return typing.Type[expected_type]  # pytype: disable=invalid-annotation
 
-  def __eq__(self, other: 'Type') -> bool:
+  def _eq(self, other: 'Type') -> bool:
     """Equals."""
-    return super().__eq__(other) and self.type == other.type
+    if self.type_resolved:
+      return self.type == other.type
+    return self.forward_refs == other.forward_refs
 
   def format(self, **kwargs):
     """Format this object."""
     details = object_utils.kvlist_str([
-        ('', self.type, None),
+        ('', self._expected_type, None),
         ('default', self._default, MISSING_VALUE),
         ('noneable', self._is_noneable, False),
         ('frozen', self._frozen, False),
     ])
     return f'{self.__class__.__name__}({details})'
 
 
@@ -1871,37 +1944,73 @@
       if not isinstance(c, ValueSpec):
         raise ValueError(
             f'Items in \'candidates\' must be ValueSpec objects.'
             f'Encountered {c} at {i}.')
       if c.is_noneable:
         has_noneable_candidate = True
 
-      # pytype: disable=attribute-error
-      spec_type = (c.__class__, c._value_type)  # pylint: disable=protected-access
-      # pytype: enable=attribute-error
+      # NOTE(daiyip): When forward declaration is present (e.g.
+      # `pg.typing.Object('A')`), calling `value_type` will trigger the
+      # resolution of the referred type. Therefore, we refer to `_value_type`
+      # instead of `value_type` to access the class name string in such cases.
+      spec_type = (c.__class__, getattr(c, '_value_type'))
       if spec_type not in candidates_by_type:
         candidates_by_type[spec_type] = []
       candidates_by_type[spec_type].append(c)
 
     for spec_type, cs in candidates_by_type.items():
       if len(cs) > 1:
         # NOTE(daiyip): Now we simply reject union of multiple value spec of
         # the same type. We may consider support Union of different List, Tuple,
         # Dict and Object later.
         raise ValueError(
             f'Found {len(cs)} value specs of the same type {spec_type}.')
 
+    candidate_types = set()
+    no_value_type_check = False
+    for c in candidates:
+      child_value_type = getattr(c, '_value_type')
+      if child_value_type is None:
+        no_value_type_check = True
+      elif isinstance(child_value_type, tuple):
+        candidate_types.update(child_value_type)
+      else:
+        candidate_types.add(child_value_type)
+
     self._candidates = candidates
-    candidate_types = {c.value_type for c in candidates}
-    union_value_type = (None
-                        if None in candidate_types else tuple(candidate_types))
+    union_value_type = None if no_value_type_check else tuple(candidate_types)
     super().__init__(union_value_type, default)
+
     if has_noneable_candidate:
       super().noneable()
 
+  @functools.cached_property
+  def forward_refs(self) -> typing.Set[class_schema.ForwardRef]:
+    """Returns forward references used in this spec."""
+    forward_refs = set()
+    for c in self._candidates:
+      forward_refs.update(c.forward_refs)
+    return forward_refs
+
+  @functools.cached_property
+  def value_type(
+      self) -> typing.Optional[typing.Tuple[typing.Type[typing.Any]]]:
+    # NOTE(daiyip): Override `value_type` property to delay the type resolution
+    # when forward declaration is invovled.
+    if self._value_type is None or not self.forward_refs:
+      return self._value_type
+
+    value_types = set()
+    for c in self._candidates:
+      child_value_type = c.value_type
+      if not isinstance(child_value_type, tuple):
+        child_value_type = (child_value_type,)
+      value_types.update(child_value_type)
+    return tuple(value_types)
+
   def noneable(self) -> 'Union':
     """Customized noneable for Union."""
     super().noneable()
     for c in self._candidates:
       c.noneable()
     return self
 
@@ -1944,32 +2053,38 @@
              child_transform: typing.Callable[
                  [object_utils.KeyPath, Field, typing.Any],
                  typing.Any
              ],
              root_path: object_utils.KeyPath) -> typing.Any:
     """Union specific apply."""
     for c in self._candidates:
-      if c.value_type is None or isinstance(value, c.value_type):
+      if (c.type_resolved
+          and (c.value_type is None or isinstance(value, c.value_type))):
         return c.apply(value, allow_partial, child_transform, root_path)
 
     # NOTE(daiyip): This code is to support consider A as B scenario when there
     # is a converter from A to B (converter may return value that is not B). A
     # use case is that tf.Variable is not a tf.Tensor, but value spec of
     # tf.Tensor should be able to accept tf.Variable.
     matched_candidate = None
     for c in self._candidates:
-      if type_conversion.get_first_applicable_converter(
+      if c.type_resolved and type_conversion.get_first_applicable_converter(
           type(value), c.value_type) is not None:
         matched_candidate = c
         break
 
-    # `_apply` is entered only when there is a type match or conversion path.
-    assert matched_candidate is not None
-    return matched_candidate.apply(
-        value, allow_partial, child_transform, root_path)
+    if self.type_resolved:
+      # `_apply` is entered only when there is a type match or conversion path.
+      assert matched_candidate is not None
+      return matched_candidate.apply(
+          value, allow_partial, child_transform, root_path)
+
+    # Return value directly if the forward declaration of the current union
+    # is unsolved.
+    return value
 
   def _extend(self, base: 'Union') -> None:
     """Union specific extension."""
     def _base_candidate(c, v):
       """Find a non-Union base spec from `v` for a input spec `c`."""
       if isinstance(v, Union):
         for vc in v.candidates:
@@ -2027,18 +2142,15 @@
             **kwargs), None),
         ('default', object_utils.quote_if_str(self._default), MISSING_VALUE),
         ('noneable', self._is_noneable, False),
         ('frozen', self._frozen, False),
     ])
     return f'{self.__class__.__name__}({details})'
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if not super().__eq__(other):
-      return False
+  def _eq(self, other: 'Union') -> bool:
     if len(self.candidates) != len(other.candidates):
       return False
     for sc in self.candidates:
       oc = other.get_candidate(sc)
       if sc != oc:
         return False
     return True
@@ -2103,20 +2215,16 @@
     return self
 
   @property
   def annotation(self) -> typing.Any:
     """Returns type annotation."""
     return self._annotation
 
-  def __eq__(self, other: typing.Any) -> bool:
-    """Operator==."""
-    if self is other:
-      return True
-    return (super().__eq__(other)
-            and self.annotation == other.annotation)
+  def _eq(self, other: 'Any') -> bool:
+    return self.annotation == other.annotation
 
 
 def _any_if_no_annotation(annotation: typing.Any):
   """Returns typing.Any if annotation is MISSING_VALUE."""
   return typing.Any if annotation == MISSING_VALUE else annotation
 
 
@@ -2198,8 +2306,20 @@
     )
 
 
 def _get_optional_arg(values: typing.Sequence[Any]) -> Any:
   return [x for x in values if x is not type(None)][0]
 
 
+def _get_spec_callsite_module():
+  """Returns the module of the callsite where ValueSpec objects are created."""
+  calling_module = None
+  callstack = inspect.stack()
+  current_source_file = sys.modules[__name__].__file__
+  for frame, file, *_ in callstack[1:]:
+    if file != current_source_file:
+      calling_module = inspect.getmodule(frame)
+      break
+  return calling_module or __main__
+
+
 ValueSpec.from_annotation = _from_annotation
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230427/pyglove/core/typing/value_specs_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,39 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.core.typing.value_specs."""
 
-import copy
-import inspect
+import contextlib
+import sys
 import typing
 import unittest
 
 from pyglove.core import object_utils
-from pyglove.core.typing import class_schema
 from pyglove.core.typing import callable_signature
+from pyglove.core.typing import class_schema
 from pyglove.core.typing import typed_missing
 from pyglove.core.typing import value_specs as vs
 from pyglove.core.typing.class_schema import ValueSpec
 
 
 class BoolTest(unittest.TestCase):
   """Tests for `Bool`."""
 
   def test_value_type(self):
     self.assertEqual(vs.Bool().value_type, bool)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Bool().forward_refs, set())
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Bool().type_resolved)
+
   def test_default(self):
     self.assertEqual(vs.Bool().default, typed_missing.MISSING_VALUE)
     self.assertEqual(vs.Bool(True).default, True)
 
   def test_noneable(self):
     self.assertFalse(vs.Bool().is_noneable)
     self.assertTrue(vs.Bool().noneable().is_noneable)
@@ -73,15 +79,15 @@
         '<(type|class) \'int\'>.'):
       vs.Bool().apply(1)
 
     with self.assertRaisesRegex(ValueError, 'Value cannot be None'):
       vs.Bool().apply(None)
 
   def test_is_compatible(self):
-    v= vs.Bool()
+    v = vs.Bool()
     self.assertTrue(v.is_compatible(v))
     self.assertTrue(vs.Bool().is_compatible(vs.Bool()))
     self.assertTrue(vs.Bool().noneable().is_compatible(vs.Bool()))
     self.assertFalse(vs.Bool().is_compatible(vs.Bool().noneable()))
     self.assertFalse(vs.Bool().is_compatible(vs.Int()))
 
   def test_extend(self):
@@ -131,14 +137,20 @@
 
 class StrTest(unittest.TestCase):
   """Tests for `Str`."""
 
   def test_value_type(self):
     self.assertEqual(vs.Str().value_type, str)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Str().forward_refs, set())
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Str().type_resolved)
+
   def test_default(self):
     self.assertEqual(vs.Str().default, typed_missing.MISSING_VALUE)
     self.assertEqual(vs.Str('abc').default, 'abc')
 
   def test_noneable(self):
     self.assertFalse(vs.Str().is_noneable)
     self.assertTrue(vs.Str().noneable().is_noneable)
@@ -250,14 +262,20 @@
 
 class IntTest(unittest.TestCase):
   """Tests for `Int`."""
 
   def test_value_type(self):
     self.assertEqual(vs.Int().value_type, int)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Int().forward_refs, set())
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Int().type_resolved)
+
   def test_default(self):
     self.assertEqual(vs.Int().default, typed_missing.MISSING_VALUE)
     self.assertEqual(vs.Int(1).default, 1)
 
   def test_noneable(self):
     self.assertFalse(vs.Int().is_noneable)
     self.assertTrue(vs.Int().noneable().is_noneable)
@@ -340,26 +358,28 @@
   def test_extend(self):
     # Child without constraints will inheirt constraints.
     self.assertEqual(vs.Int().extend(vs.Int(min_value=0, max_value=1)),
                      vs.Int(min_value=0, max_value=1))
 
     # Child extends base with constraints will intersect valid range.
     self.assertEqual(
-        vs.Int(min_value=2,
-                   max_value=5).extend(vs.Int(min_value=2, max_value=6)),
-        vs.Int(min_value=2, max_value=5))
+        vs.Int(min_value=2, max_value=5).extend(
+            vs.Int(min_value=2, max_value=6)
+        ),
+        vs.Int(min_value=2, max_value=5),
+    )
 
     # Child may extend a noneable base into non-noneable.
     self.assertFalse(vs.Int().extend(vs.Int().noneable()).is_noneable)
 
     # Child may extend a union that has the same type.
     self.assertEqual(
-        vs.Int().extend(
-            vs.Union([vs.Int(min_value=1),
-                          vs.Bool()])), vs.Int(min_value=1))
+        vs.Int().extend(vs.Union([vs.Int(min_value=1), vs.Bool()])),
+        vs.Int(min_value=1),
+    )
 
     with self.assertRaisesRegex(TypeError,
                                 '.* cannot extend .*: incompatible type.'):
       vs.Int().extend(vs.Bool())
 
     # Child cannot extend a non-noneable base to noneable.
     with self.assertRaisesRegex(
@@ -416,14 +436,20 @@
 
 class FloatTest(unittest.TestCase):
   """Tests for `Float`."""
 
   def test_value_type(self):
     self.assertEqual(vs.Float().value_type, float)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Float().forward_refs, set())
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Float().type_resolved)
+
   def test_default(self):
     self.assertEqual(vs.Float().default, typed_missing.MISSING_VALUE)
     self.assertEqual(vs.Float(1.0).default, 1.0)
 
   def test_noneable(self):
     self.assertFalse(vs.Float().is_noneable)
     self.assertTrue(vs.Float().noneable().is_noneable)
@@ -593,14 +619,20 @@
     b1 = B()
     b2 = B()
     c = C()
     self.assertEqual(vs.Enum(a, [a, b1, None]).value_type, A)
     self.assertEqual(vs.Enum(b1, [b1, b2]).value_type, B)
     self.assertIsNone(vs.Enum(a, [a, b1, c]).value_type)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Enum('a', ['a', None]).forward_refs, set())
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Enum('a', ['a', None]).type_resolved)
+
   def test_default(self):
     self.assertEqual(vs.Enum('a', ['a', 'b']).default, 'a')
     self.assertEqual(vs.Enum('a', ['a']).noneable().default, 'a')
     self.assertIsNone(vs.Enum(None, [None, 'a']).default)
 
   def test_noneable(self):
     self.assertFalse(vs.Enum('a', ['a', 'b']).is_noneable)
@@ -695,14 +727,30 @@
 
 class ListTest(unittest.TestCase):
   """Tests for `List`."""
 
   def test_value_type(self):
     self.assertEqual(vs.List(vs.Int()).value_type, list)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.List(vs.Int()).forward_refs, set())
+    self.assertEqual(
+        vs.List(vs.Object('A')).forward_refs, set([forward_ref('A')])
+    )
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.List(vs.Int()).type_resolved)
+    self.assertFalse(vs.List(vs.Object('A')).type_resolved)
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertTrue(vs.List(vs.Object('A')).type_resolved)
+
   def test_default(self):
     self.assertEqual(
         vs.List(vs.Int()).default, typed_missing.MISSING_VALUE)
     self.assertIsNone(vs.List(vs.Int()).noneable().default)
     self.assertEqual(vs.List(vs.Int(), []).default, [])
 
   def test_min_max_size(self):
@@ -733,14 +781,19 @@
         vs.List(vs.Any()).annotation, typing.List[typing.Any])
     self.assertEqual(
         vs.List(vs.Int()).noneable().annotation,
         typing.Optional[typing.List[int]])
     self.assertEqual(
         vs.List(vs.Int().noneable()).annotation,
         typing.List[typing.Optional[int]])
+    self.assertEqual(
+        vs.List(vs.Object(BoolTest)).annotation, typing.List[BoolTest]
+    )
+    # Unresolved forward declaration will use string as annotation.
+    self.assertEqual(vs.List(vs.Object('A')).annotation, typing.List['A'])
 
   def test_eq(self):
     self.assertEqual(vs.List(vs.Int()), vs.List(vs.Int()))
     self.assertEqual(
         vs.List(vs.Int(), []), vs.List(vs.Int(), []))
     self.assertEqual(
         vs.List(vs.Int(), [], max_size=10),
@@ -786,18 +839,35 @@
     self.assertIsInstance(l[0], object_utils.KeyPath)
     self.assertEqual(l, [object_utils.KeyPath.parse('a.b.c')])
     self.assertEqual(
         vs.List(vs.Int()).apply(
             typed_missing.MISSING_VALUE, allow_partial=True),
         typed_missing.MISSING_VALUE)
     self.assertEqual(
-        vs.List(vs.Dict([('a', vs.Str())
-                                ])).apply([{}], allow_partial=True), [{
-                                    'a': typed_missing.MissingValue(vs.Str())
-                                }])
+        vs.List(vs.Dict([('a', vs.Str())])).apply([{}], allow_partial=True),
+        [{'a': typed_missing.MissingValue(vs.Str())}],
+    )
+
+    l = vs.List(vs.Object('A'))
+
+    # Element spec `vs.Object('A')` is not resolved, thus we do not perform type
+    # checking on list element.
+    self.assertEqual(l.apply([1]), [1])
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      # Now 'A' is resolved, thus type check will occur.
+      with self.assertRaisesRegex(TypeError, 'Expect .* but encountered'):
+        l.apply([1])
+
+      # But objects of `A` are acceptable.
+      a = A()
+      self.assertEqual(l.apply([a]), [a])
 
     with self.assertRaisesRegex(ValueError, 'Value cannot be None'):
       vs.List(vs.Int()).apply(None)
 
     with self.assertRaisesRegex(
         TypeError, 'Expect <(type|class) \'list\'> but encountered '
         '<(type|class) \'int\'>.'):
@@ -817,23 +887,23 @@
 
   def test_apply_with_user_validator(self):
     def _sum_greater_than_zero(value):
       if sum(value) <= 0:
         raise ValueError('Sum expected to be larger than zero')
 
     self.assertEqual(
-        vs.List(vs.Int(),
-                    user_validator=_sum_greater_than_zero).apply([0, 1]),
-        [0, 1])
+        vs.List(vs.Int(), user_validator=_sum_greater_than_zero).apply([0, 1]),
+        [0, 1],
+    )
 
     with self.assertRaisesRegex(
         ValueError, 'Sum expected to be larger than zero \\(path=\\[0\\]\\)'):
-      vs.List(
-          vs.List(vs.Int(),
-                      user_validator=_sum_greater_than_zero)).apply([[-1]])
+      vs.List(vs.List(vs.Int(), user_validator=_sum_greater_than_zero)).apply(
+          [[-1]]
+      )
 
   def test_is_compatible(self):
     self.assertTrue(
         vs.List(vs.Int()).is_compatible(vs.List(vs.Int())))
 
     self.assertTrue(
         vs.List(vs.Int()).noneable().is_compatible(vs.List(vs.Int())))
@@ -934,14 +1004,36 @@
 class TupleTest(unittest.TestCase):
   """Tests for `Tuple`."""
 
   def test_value_type(self):
     self.assertEqual(vs.Tuple([vs.Int()]).value_type, tuple)
     self.assertEqual(vs.Tuple(vs.Int()).value_type, tuple)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Tuple(vs.Int()).forward_refs, set())
+    self.assertEqual(
+        vs.Tuple(vs.Object('A')).forward_refs, set([forward_ref('A')])
+    )
+    self.assertEqual(
+        vs.Tuple([vs.Object('A'), vs.Int(), vs.Object('B')]).forward_refs,
+        set([forward_ref('A'), forward_ref('B')]),
+    )
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Tuple(vs.Int()).type_resolved)
+    self.assertFalse(vs.Tuple(vs.Object('A')).type_resolved)
+    self.assertFalse(vs.Tuple([vs.Int(), vs.Object('A')]).type_resolved)
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertTrue(vs.Tuple(vs.Object('A')).type_resolved)
+      self.assertTrue(vs.Tuple([vs.Int(), vs.Object('A')]).type_resolved)
+
   def test_default(self):
     self.assertEqual(
         vs.Tuple(vs.Int()).default, typed_missing.MISSING_VALUE)
     self.assertIsNone(vs.Tuple([vs.Int()]).noneable().default)
     self.assertEqual(vs.Tuple([vs.Int()], (1,)).default, (1,))
 
   def test_noneable(self):
@@ -993,14 +1085,27 @@
     self.assertEqual(
         vs.Tuple(vs.Int()).annotation, typing.Tuple[int, ...])
     self.assertEqual(
         vs.Tuple([vs.Int(), vs.Str()]).annotation, typing.Tuple[int, str])
     self.assertEqual(
         vs.Tuple([vs.Int(), vs.Any()]).annotation,
         typing.Tuple[int, typing.Any])
+    self.assertEqual(
+        vs.Tuple(vs.Object('BoolTest')).annotation, typing.Tuple[BoolTest, ...]
+    )
+    self.assertEqual(
+        vs.Tuple(vs.Object('A')).annotation, typing.Tuple['A', ...]
+    )
+    self.assertEqual(
+        vs.Tuple([vs.Int(), vs.Object('BoolTest')]).annotation,
+        typing.Tuple[int, BoolTest],
+    )
+    self.assertEqual(
+        vs.Tuple([vs.Int(), vs.Object('A')]).annotation, typing.Tuple[int, 'A']
+    )
 
   def test_eq(self):
     v = vs.Tuple([vs.Int(), vs.Int()])
     self.assertEqual(v, v)
 
     self.assertEqual(vs.Tuple(vs.Int()), vs.Tuple(vs.Int()))
     self.assertEqual(vs.Tuple([vs.Int()]), vs.Tuple([vs.Int()]))
@@ -1120,16 +1225,17 @@
     self.assertEqual(
         vs.Tuple([vs.Int(), vs.Int()],
                  user_validator=_sum_greater_than_zero).apply((0, 1)),
         (0, 1))
 
     with self.assertRaisesRegex(
         ValueError, 'Sum expected to be larger than zero \\(path=\\[0\\]\\)'):
-      vs.Tuple([vs.Tuple([vs.Int()],
-               user_validator=_sum_greater_than_zero)]).apply(((-1,),))
+      vs.Tuple(
+          [vs.Tuple([vs.Int()], user_validator=_sum_greater_than_zero)]
+      ).apply(((-1,),))
 
   def test_is_compatible(self):
     self.assertTrue(vs.Tuple(vs.Int()).is_compatible(vs.Tuple(vs.Int())))
     self.assertTrue(vs.Tuple(vs.Int()).is_compatible(vs.Tuple([vs.Int()])))
     self.assertTrue(
         vs.Tuple(vs.Int()).is_compatible(
             vs.Tuple(vs.Int(), min_size=2, max_size=4)))
@@ -1258,16 +1364,15 @@
     with self.assertRaisesRegex(
         TypeError, '.* cannot extend .*: unmatched number of elements.'):
       vs.Tuple([vs.Int()]).extend(vs.Tuple([vs.Int(), vs.Int()]))
 
     # Child cannot extend a non-noneable base to noneable.
     with self.assertRaisesRegex(
         TypeError, '.* cannot extend .*: None is not allowed in base spec.'):
-      vs.Tuple([vs.Int()
-                   ]).noneable().extend(vs.Tuple([vs.Int()]))
+      vs.Tuple([vs.Int()]).noneable().extend(vs.Tuple([vs.Int()]))
 
     # Child with larger max_size cannot extend base with smaller max_size.
     with self.assertRaisesRegex(
         TypeError, '.* cannot extend .*: max_value is larger.'):
       vs.Tuple([vs.Int(max_value=100)]).extend(vs.Tuple([vs.Int(max_value=0)]))
 
   def test_freeze(self):
@@ -1296,14 +1401,47 @@
 
 class DictTest(unittest.TestCase):
   """Tests for `Dict`."""
 
   def test_value_type(self):
     self.assertIs(vs.Dict().value_type, dict)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Dict().forward_refs, set())
+    self.assertEqual(
+        vs.Dict([
+            ('x', vs.Object('A')),
+            ('y', vs.Dict([
+                ('z', vs.Object('B'))
+            ]))
+        ]).forward_refs,
+        set((forward_ref('A'), forward_ref('B'))))
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Dict().type_resolved)
+    v = vs.Dict([
+        ('x', vs.Object('A')),
+        ('y', vs.Dict([
+            ('z', vs.Object('B'))
+        ]))
+    ])
+    self.assertFalse(v.type_resolved)
+
+    class A:
+      pass
+
+    class B:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertFalse(v.type_resolved)
+
+    with simulate_forward_declaration(A, B):
+      self.assertTrue(v.type_resolved)
+
   def test_default(self):
     self.assertEqual(
         vs.Dict([('a', vs.Int(), 'field 1')]).default,
         {'a': typed_missing.MISSING_VALUE})
 
     self.assertEqual(
         vs.Dict([
@@ -1314,15 +1452,15 @@
         ]).default,
         dict(a=1, b={'c': 'foo'}))
 
     self.assertEqual(
         vs.Dict([
             ('a', vs.Int(1), 'field 1'),
             ('b', vs.Dict([
-                ('c', vs.Str(), 'field 2.1')
+                ('c', vs.Object('A'), 'field 2.1')
             ]), 'field 2')]).default,
         dict(a=1, b={'c': typed_missing.MISSING_VALUE}))
 
     self.assertIsNone(vs.Dict([('a', vs.Int(), 'field 1')]).noneable().default)
 
   def test_noneable(self):
     self.assertFalse(vs.Dict().is_noneable)
@@ -1407,14 +1545,35 @@
             ('b', vs.Bool().noneable(), 'field 2'),
         ]).apply({'a': 1}),
         {
             'a': 1,
             'b': None
         })
 
+    # Tests with forward declaration.
+    v = vs.Dict([
+        ('a', vs.Int(), 'field 1'),
+        ('b', vs.Object('B'), 'field 2')
+    ])
+
+    # Before forward reference 'B' can be resolved, `b` can accept anything.
+    self.assertEqual(v.apply(dict(a=1, b=2)), dict(a=1, b=2))
+
+    # After forward reference 'B' can be resolved, `b` can accept only objects
+    # of `B`.
+    class B:
+      pass
+
+    b = B()
+    with simulate_forward_declaration(B):
+      self.assertEqual(v.apply(dict(a=1, b=b)), dict(a=1, b=b))
+      with self.assertRaisesRegex(TypeError, 'Expect .* but encountered'):
+        v.apply(dict(a=1, b=2))
+
+    # Tests for partial apply.
     self.assertEqual(
         vs.Dict([
             ('a', vs.Int(), 'field 1'),
             ('b', vs.Bool().noneable(), 'field 2'),
         ]).apply({'b': True}, allow_partial=True),
         {
             'a': typed_missing.MISSING_VALUE,
@@ -1568,50 +1727,80 @@
       pass
 
     class D(C, object_utils.MaybePartial):
 
       def missing_values(self):
         return {'SOME_KEY': 'SOME_VALUE'}
 
+    # pylint: disable=invalid-name
     self.A = A
     self.B = B
     self.C = C
     self.D = D
+    # pylint: enable=invalid-name
 
   def test_value_type(self):
     self.assertEqual(vs.Object(self.A).value_type, self.A)
+    v = vs.Object('A')
+
+    with simulate_forward_declaration(self.A):
+      self.assertIs(v.value_type, self.A)
+
+    with self.assertRaisesRegex(TypeError, "'A' does not exist in module .*"):
+      _ = vs.Object('A').value_type
+
+  def test_forward_refs(self):
+    self.assertEqual(vs.Object(self.A).forward_refs, set())
+    self.assertEqual(vs.Object('Foo').forward_refs, set([forward_ref('Foo')]))
 
   def test_default(self):
     self.assertEqual(vs.Object(self.A).default, typed_missing.MISSING_VALUE)
     a = self.A()
     self.assertEqual(vs.Object(self.A, a).default, a)
 
   def test_noneable(self):
     self.assertFalse(vs.Object(self.A).is_noneable)
     self.assertTrue(vs.Object(self.A).noneable().is_noneable)
+    self.assertTrue(vs.Object('Foo').noneable().is_noneable)
 
   def test_str(self):
     self.assertEqual(str(vs.Object(self.A)), 'Object(A)')
+    self.assertEqual(str(vs.Object('Foo')), 'Object(Foo)')
     self.assertEqual(
         str(vs.Object(self.A).noneable()),
         'Object(A, default=None, noneable=True)')
     self.assertEqual(
         str(vs.Object(self.A).noneable().freeze()),
         'Object(A, default=None, noneable=True, frozen=True)')
 
   def test_annotation(self):
     self.assertEqual(vs.Object(self.A).annotation, self.A)
+    with simulate_forward_declaration(self.A):
+      self.assertEqual(vs.Object('A').annotation, self.A)
+    self.assertEqual(vs.Object('Foo').annotation, 'Foo')
     self.assertEqual(
         vs.Object(self.A).noneable().annotation, typing.Optional[self.A])
 
   def test_eq(self):
     o = vs.Object(self.A)
     self.assertEqual(o, o)
     self.assertIsNone(o.schema)
     self.assertEqual(vs.Object(self.A), vs.Object(self.A))
+
+    class A:
+      pass
+
+    o = vs.Object('A')
+    # The local class 'A' is not a module level class.
+    self.assertNotEqual(o, vs.Object(A))
+    with simulate_forward_declaration(self.A):
+      self.assertEqual(o, vs.Object(self.A))
+
+    self.assertEqual(vs.Object('A'), vs.Object('A'))
+    self.assertNotEqual(vs.Object('A'), vs.Object('B'))
     self.assertEqual(
         vs.Object(self.A).noneable(), vs.Object(self.A).noneable())
     self.assertNotEqual(vs.Object(self.A).noneable(), vs.Object(self.A))
     self.assertNotEqual(vs.Object(self.A), vs.Object(self.B))
 
   def test_bad_init(self):
     with self.assertRaisesRegex(
@@ -1633,14 +1822,24 @@
 
     b = self.B()
     self.assertEqual(vs.Object(self.A).apply(b), b)
 
     d = self.D()
     self.assertEqual(vs.Object(self.C).apply(d, allow_partial=True), d)
 
+    v = vs.Object('A')
+    # 'A' is not resolved, so it could accept any object type.
+    self.assertIs(v.apply(1), 1)
+    with simulate_forward_declaration(self.A, self.B):
+      self.assertIs(v.apply(a), a)
+      self.assertIs(v.apply(b), b)
+      with self.assertRaisesRegex(TypeError, 'Expect .* but encountered'):
+        # 'A' is resolved, so it could not accept 1 any more.
+        _ = v.apply(1)
+
     with self.assertRaisesRegex(ValueError, 'Value cannot be None'):
       vs.Object(self.A).apply(None)
 
     with self.assertRaisesRegex(
         TypeError,
         'Expect <class .*A\'> but encountered <(type|class) \'int\'>.'):
       vs.Object(self.A).apply(1)
@@ -1664,23 +1863,43 @@
     with self.assertRaisesRegex(ValueError, 'Value should be zero \\(path=\\)'):
       vs.Object(self.B, user_validator=_value_is_zero).apply(self.B(1))
 
   def test_is_compatible(self):
     self.assertTrue(vs.Object(self.A).is_compatible(vs.Object(self.A)))
     self.assertTrue(
         vs.Object(self.A).noneable().is_compatible(vs.Object(self.A)))
+
+    # Before a forward declaration can be resolved, `is_compatible` always
+    # returns True.
+    self.assertTrue(vs.Object('A').is_compatible(vs.Object('B')))
+    with simulate_forward_declaration(self.A, self.B):
+      self.assertTrue(vs.Object('A').is_compatible(vs.Object('B')))
+      self.assertFalse(vs.Object('B').is_compatible(vs.Object('A')))
+
     self.assertTrue(vs.Object(self.A).is_compatible(vs.Object(self.B)))
+    self.assertTrue(vs.Object('Foo').is_compatible(vs.Object('Bar')))
 
     self.assertFalse(vs.Object(self.A).is_compatible(vs.Int()))
     self.assertFalse(
         vs.Object(self.A).is_compatible(vs.Object(self.A).noneable()))
     self.assertFalse(vs.Object(self.B).is_compatible(vs.Object(self.A)))
     self.assertFalse(vs.Object(self.B).is_compatible(vs.Object(self.C)))
 
   def test_extend(self):
+    # Before a forward declaration can be resolved, `extend` will succeed
+    self.assertEqual(
+        vs.Object('A').extend(vs.Object('B')), vs.Object('A'))
+
+    # When forward declaration is resolved, `extend` will follow class
+    # relationships.
+    with simulate_forward_declaration(self.A, self.B):
+      with self.assertRaisesRegex(
+          TypeError, '.* cannot extend .*: incompatible class.'):
+        vs.Object('A').extend(vs.Object('B'))
+
     self.assertEqual(
         vs.Object(self.B).extend(vs.Object(self.A)),
         vs.Object(self.B))
     self.assertEqual(
         vs.Object(self.A).extend(vs.Callable([vs.Any()])),
         vs.Object(self.A))
     self.assertEqual(
@@ -1728,14 +1947,43 @@
 class CallableTest(unittest.TestCase):
   """Tests for `Callable`."""
 
   def test_value_type(self):
     self.assertIsNone(vs.Callable().value_type)
     self.assertEqual(vs.Functor().annotation, object_utils.Functor)
 
+  def test_forward_refs(self):
+    self.assertEqual(vs.Callable().forward_refs, set())
+    self.assertEqual(
+        vs.Callable([vs.Int(), vs.Object('A')],
+                    kw=[('x', vs.Object('B'))],
+                    returns=vs.Object('C')).forward_refs,
+        set([forward_ref('A'), forward_ref('B'), forward_ref('C')]))
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Callable().type_resolved)
+    self.assertTrue(vs.Callable([vs.Object('BoolTest')]).type_resolved)
+    self.assertTrue(
+        vs.Callable(kw=[('x', vs.Object('BoolTest'))]).type_resolved)
+    self.assertTrue(vs.Callable(returns=vs.Object('BoolTest')).type_resolved)
+
+    self.assertFalse(vs.Callable([vs.Object('A')]).type_resolved)
+    self.assertFalse(
+        vs.Callable(kw=[('x', vs.Object('A'))]).type_resolved)
+    self.assertFalse(vs.Callable(returns=vs.Object('A')).type_resolved)
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertTrue(vs.Callable([vs.Object('A')]).type_resolved)
+      self.assertTrue(
+          vs.Callable(kw=[('x', vs.Object('A'))]).type_resolved)
+      self.assertTrue(vs.Callable(returns=vs.Object('A')).type_resolved)
+
   def test_default(self):
     self.assertEqual(vs.Callable().default, typed_missing.MISSING_VALUE)
     func = lambda x: x
     self.assertIs(vs.Callable(default=func).default, func)
 
   def test_noneable(self):
     self.assertFalse(vs.Callable().is_noneable)
@@ -2081,18 +2329,38 @@
 
   def test_init(self):
     with self.assertRaisesRegex(TypeError, '.* is not a type'):
       _ = vs.Type(1)
 
   def test_value_type(self):
     self.assertEqual(vs.Type(Exception).value_type, type)
+    self.assertEqual(vs.Type('A').value_type, type)
+
+  def test_forward_refs(self):
+    self.assertEqual(vs.Type(Exception).forward_refs, set())
+    self.assertEqual(vs.Type('A').forward_refs, set([forward_ref('A')]))
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Type(Exception).type_resolved)
+    self.assertTrue(vs.Type('BoolTest').type_resolved)
+    self.assertFalse(vs.Type('A').type_resolved)
 
   def test_type(self):
     self.assertIs(vs.Type(int).type, int)
     self.assertIs(vs.Type(Exception).type, Exception)
+    self.assertIs(vs.Type('BoolTest').type, BoolTest)
+
+    with self.assertRaisesRegex(TypeError, '.* does not exist'):
+      _ = vs.Type('A').type
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertIs(vs.Type('A').type, A)
 
   def test_default(self):
     self.assertEqual(vs.Type(Exception).default, typed_missing.MISSING_VALUE)
     self.assertEqual(vs.Type(Exception, default=ValueError).default, ValueError)
 
   def test_noneable(self):
     self.assertFalse(vs.Type(Exception).is_noneable)
@@ -2105,22 +2373,33 @@
         'Type(<class \'Exception\'>, default=None, noneable=True)')
     self.assertEqual(
         str(vs.Type(Exception).noneable().freeze()),
         'Type(<class \'Exception\'>, default=None, noneable=True, frozen=True)')
 
   def test_annotation(self):
     self.assertEqual(vs.Type(Exception).annotation, typing.Type[Exception])
+    self.assertEqual(vs.Type('BoolTest').annotation, typing.Type[BoolTest])
+    self.assertEqual(vs.Type('A').annotation, typing.Type['A'])
     self.assertEqual(
         vs.Type(Exception).noneable().annotation,
         typing.Optional[typing.Type[Exception]])
 
   def test_eq(self):
     t = vs.Type(Exception)
     self.assertEqual(t, t)
     self.assertEqual(vs.Type(Exception), vs.Type(Exception))
+    self.assertEqual(vs.Type('A'), vs.Type('A'))
+
+    class A:
+      pass
+
+    self.assertNotEqual(vs.Type('A'), vs.Type(A))
+    with simulate_forward_declaration(A):
+      self.assertEqual(vs.Type('A'), vs.Type(A))
+
     self.assertEqual(
         vs.Type(Exception).noneable(),
         vs.Type(Exception).noneable())
     self.assertEqual(
         vs.Type(Exception, default=ValueError),
         vs.Type(Exception, default=ValueError))
     self.assertNotEqual(vs.Type(Exception), vs.Type(int))
@@ -2131,23 +2410,57 @@
         vs.Type(Exception), vs.Type(Exception, default=ValueError))
 
   def test_apply(self):
     self.assertEqual(vs.Type(Exception).apply(Exception), Exception)
     self.assertEqual(vs.Type(Exception).apply(ValueError), ValueError)
     self.assertIsNone(vs.Type(Exception).noneable().apply(None))
 
+    v = vs.Type('A')
+
+    # Before 'A' can be resolved, v could accept any type.
+    self.assertIs(v.apply(int), int)
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertIs(v.apply(A), A)
+
+      # After 'A' can be resolved, v could only accept 'A'.
+      with self.assertRaisesRegex(ValueError, '.* is not a subclass of .*'):
+        _ = v.apply(int)
+
     with self.assertRaisesRegex(ValueError, '.* is not a subclass of .*'):
       vs.Type(Exception).apply(int)
 
     with self.assertRaisesRegex(ValueError, 'Value cannot be None'):
       vs.Type(Exception).apply(None)
 
   def test_is_compatible(self):
     self.assertTrue(vs.Type(Exception).is_compatible(vs.Type(Exception)))
     self.assertTrue(vs.Type(Exception).is_compatible(vs.Type(ValueError)))
+
+    # Before `A` can be accepted, it's always considered compatible.
+    self.assertTrue(vs.Type('A').is_compatible(vs.Type(Exception)))
+    self.assertTrue(vs.Type(Exception).is_compatible(vs.Type('A')))
+
+    # After `A` can be accepted, it can only accept subclasses of `A`.
+    class A:
+      pass
+
+    class B(A):
+      pass
+
+    with simulate_forward_declaration(A, B):
+      self.assertTrue(vs.Type('A').is_compatible(vs.Type('A')))
+      self.assertTrue(vs.Type('A').is_compatible(vs.Type('B')))
+      self.assertFalse(vs.Type('B').is_compatible(vs.Type('A')))
+      self.assertFalse(vs.Type(Exception).is_compatible(vs.Type('A')))
+      self.assertFalse(vs.Type('A').is_compatible(vs.Type(Exception)))
+
     self.assertTrue(
         vs.Type(Exception).noneable().is_compatible(vs.Type(ValueError)))
     self.assertFalse(
         vs.Type(Exception).is_compatible(vs.Type(ValueError).noneable()))
     self.assertFalse(vs.Type(Exception).is_compatible(vs.Type(int)))
 
   def test_extend(self):
@@ -2206,21 +2519,62 @@
 
       def __call__(self):
         pass
 
     class B(A):
       pass
 
+    # pylint: disable=invalid-name
     self.A = A
     self.B = B
+    # pylint: enable=invalid-name
 
   def test_value_type(self):
     self.assertEqual(
         set(vs.Union([vs.Int(), vs.Bool()]).value_type),
         set([int, bool]))
+    v = vs.Union([vs.Object('A'), vs.Object('B')])
+    with simulate_forward_declaration(self.A, self.B):
+      self.assertEqual(set(v.value_type), set([self.A, self.B]))
+
+    v = vs.Union(
+        [vs.Int(), vs.Object('A'), vs.Union([vs.Int(), vs.Float()]).noneable()]
+    )
+    with simulate_forward_declaration(self.A):
+      self.assertEqual(set(v.value_type), set((int, self.A, float)))
+
+  def test_forward_refs(self):
+    self.assertEqual(
+        vs.Union([vs.Int(), vs.Object(self.A)]).forward_refs, set()
+    )
+    self.assertEqual(
+        vs.Union([vs.Int(), vs.Object('Foo')]).forward_refs,
+        set([forward_ref('Foo')]),
+    )
+    self.assertEqual(
+        vs.Union([
+            vs.Int(),
+            vs.Object('Bar'),
+            vs.Union([
+                vs.Float(),
+                vs.Object('Foo'),
+            ]).noneable(),
+        ]).forward_refs,
+        set([forward_ref('Bar'), forward_ref('Foo')]),
+    )
+
+  def test_type_resolved(self):
+    self.assertTrue(vs.Union([vs.Int(), vs.Float()]).type_resolved)
+    self.assertFalse(vs.Union([vs.Object('A'), vs.Float()]).type_resolved)
+
+    class A:
+      pass
+
+    with simulate_forward_declaration(A):
+      self.assertTrue(vs.Union([vs.Object('A'), vs.Float()]).type_resolved)
 
   def test_default(self):
     self.assertEqual(
         vs.Union([vs.Int(), vs.Bool()]).default,
         typed_missing.MISSING_VALUE)
     self.assertIsNone(
         vs.Union([vs.Int(), vs.Bool()]).noneable().default)
@@ -2229,16 +2583,16 @@
   def test_noneable(self):
     self.assertFalse(vs.Union([vs.Int(), vs.Bool()]).is_noneable)
     self.assertTrue(
         vs.Union([vs.Int(), vs.Bool()]).noneable().is_noneable)
     self.assertFalse(
         vs.Union([vs.Int(), vs.Bool()]).candidates[0].is_noneable)
     self.assertTrue(
-        vs.Union([vs.Int(),
-                      vs.Bool()]).noneable().candidates[0].is_noneable)
+        vs.Union([vs.Int(), vs.Bool()]).noneable().candidates[0].is_noneable
+    )
     self.assertTrue(
         vs.Union([vs.Int().noneable(), vs.Bool()]).is_noneable)
 
   def test_str(self):
     self.assertEqual(
         repr(vs.Union([vs.Int(), vs.Bool()])), 'Union([Int(), Bool()])')
     self.assertEqual(
@@ -2344,14 +2698,33 @@
     self.assertIsNone(
         vs.Union([vs.Int(), vs.Str()]).noneable().apply(None))
     self.assertEqual(
         vs.Union([vs.Int(), vs.Str()]).apply(
             typed_missing.MISSING_VALUE, allow_partial=True),
         typed_missing.MISSING_VALUE)
 
+    v = vs.Union([vs.Int(), vs.Object('A')])
+
+    # Before `A` could be resolved, `v` can accept anything.
+    self.assertEqual(v.apply('foo'), 'foo')
+
+    # After `A` is resolved, `v` can only accept subclasses of A.
+    class A:
+      pass
+
+    class B(A):
+      pass
+
+    b = B()
+    with simulate_forward_declaration(A):
+      self.assertIs(v.apply(b), b)
+      with self.assertRaisesRegex(TypeError, 'Expect .* but encountered .*'):
+        _ = v.apply('foo')
+
+    # Bad cases.
     with self.assertRaisesRegex(ValueError, 'Value cannot be None'):
       vs.Union([vs.Int(), vs.Str()]).apply(None)
 
     with self.assertRaisesRegex(
         TypeError, 'Expect \\(.*\\) but encountered <(type|class) \'list\'>.'):
       vs.Union([vs.Int(), vs.Str()]).apply([])
 
@@ -2479,15 +2852,17 @@
   def test_str(self):
     self.assertEqual(str(vs.Any()), 'Any()')
     self.assertEqual(str(vs.Any(1)), 'Any(default=1)')
     self.assertEqual(str(vs.Any(1).freeze()), 'Any(default=1, frozen=True)')
 
   def test_annotation(self):
     self.assertEqual(vs.Any().annotation, typed_missing.MISSING_VALUE)
-    self.assertEqual(vs.Any().noneable().annotation, typed_missing.MISSING_VALUE)
+    self.assertEqual(
+        vs.Any().noneable().annotation, typed_missing.MISSING_VALUE
+    )
     self.assertEqual(vs.Any(annotation=int).noneable().annotation, int)
 
   def test_eq(self):
     self.assertEqual(vs.Any(), vs.Any())
     self.assertEqual(vs.Any(True), vs.Any(True))
     self.assertNotEqual(vs.Any(), vs.Int())
     self.assertNotEqual(vs.Any(True), vs.Any())
@@ -2599,9 +2974,24 @@
         vs.Union([vs.Int(), vs.Str()]),
     )
     self.assertEqual(
         ValueSpec.from_annotation(int, False), vs.Any(annotation=int)
     )
 
 
+@contextlib.contextmanager
+def simulate_forward_declaration(*module_level_symbols):
+  try:
+    for symbol in module_level_symbols:
+      setattr(sys.modules[__name__], symbol.__name__, symbol)
+    yield
+  finally:
+    for symbol in module_level_symbols:
+      delattr(sys.modules[__name__], symbol.__name__)
+
+
+def forward_ref(name):
+  return class_schema.ForwardRef(sys.modules[__name__], name)
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230427/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove/generators.py` & `pyglove-0.3.1.dev20230427/pyglove/generators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230427/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230426
+Version: 0.3.1.dev20230427
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230426/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230427/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230426/setup.py` & `pyglove-0.3.1.dev20230427/setup.py`

 * *Files identical despite different names*

