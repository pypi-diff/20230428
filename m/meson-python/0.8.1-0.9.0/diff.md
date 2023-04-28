# Comparing `tmp/meson_python-0.8.1.tar.gz` & `tmp/meson_python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meson_python-0.8.1.tar", last modified: Thu Jul 28 17:51:49 2022, max compression
+gzip compressed data, was "meson_python-0.9.0.tar", last modified: Thu Sep 29 22:38:44 2022, max compression
```

## Comparing `meson_python-0.8.1.tar` & `meson_python-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,103 @@
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 meson_python-0.8.1/.github/workflows/checks.yml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 meson_python-0.8.1/.github/workflows/tests-cygwin.yml
--rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 meson_python-0.8.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       43 1970-01-01 00:00:00.000000 meson_python-0.8.1/.gitignore
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 meson_python-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 meson_python-0.8.1/.readthedocs.yml
--rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 meson_python-0.8.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 meson_python-0.8.1/LICENSE
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 meson_python-0.8.1/README.md
--rw-r--r--   0        0        0       15 1970-01-01 00:00:00.000000 meson_python-0.8.1/codecov.yml
--rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 meson_python-0.8.1/docs/changelog.rst
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 meson_python-0.8.1/docs/conf.py
--rw-r--r--   0        0        0     6246 1970-01-01 00:00:00.000000 meson_python-0.8.1/docs/index.rst
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 meson_python-0.8.1/docs/usage/build-options.rst
--rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 meson_python-0.8.1/docs/usage/start.rst
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 meson_python-0.8.1/meson.build
--rw-r--r--   0        0        0    38474 1970-01-01 00:00:00.000000 meson_python-0.8.1/mesonpy/__init__.py
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 meson_python-0.8.1/mesonpy/_compat.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 meson_python-0.8.1/mesonpy/_elf.py
--rw-r--r--   0        0        0     5187 1970-01-01 00:00:00.000000 meson_python-0.8.1/mesonpy/_tags.py
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 meson_python-0.8.1/mesonpy/_util.py
--rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 meson_python-0.8.1/noxfile.py
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 meson_python-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 meson_python-0.8.1/setup.cfg
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/configure-data/configure_data.py.in
--rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/configure-data/meson.build
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/configure-data/pyproject.toml
--rw-r--r--   0        0        0       56 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/dynamic-version/meson.build
--rw-r--r--   0        0        0      134 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/dynamic-version/pyproject.toml
--rw-r--r--   0        0        0       13 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/full-metadata/LICENSE
--rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/full-metadata/README.md
--rw-r--r--   0        0        0       54 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/full-metadata/meson.build
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/full-metadata/pyproject.toml
--rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library/example.c
--rw-r--r--   0        0        0       41 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library/examplelib.c
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library/examplelib.h
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library/meson.build
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library/pyproject.toml
--rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library-pep621/example.c
--rw-r--r--   0        0        0       41 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library-pep621/examplelib.c
--rw-r--r--   0        0        0      204 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library-pep621/meson.build
--rw-r--r--   0        0        0      122 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/library-pep621/pyproject.toml
--rw-r--r--   0        0        0       53 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/license-file/meson.build
--rw-r--r--   0        0        0      168 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/license-file/pyproject.toml
--rw-r--r--   0        0        0        7 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/license-file/something/LICENSE.custom
--rw-r--r--   0        0        0       41 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/link-against-local-lib/examplelib.c
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/link-against-local-lib/examplelib.h
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/link-against-local-lib/examplemod.c
--rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/link-against-local-lib/meson.build
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/link-against-local-lib/pyproject.toml
--rw-r--r--   0        0        0      135 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/pure/meson.build
--rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/pure/pure.py
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/pure/pyproject.toml
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/purelib-and-platlib/meson.build
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/purelib-and-platlib/plat.c
--rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/purelib-and-platlib/pure.py
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/purelib-and-platlib/pyproject.toml
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/subdirs/meson.build
--rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/subdirs/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/subdirs/subdirs/__init__.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/subdirs/subdirs/a/__init__.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/subdirs/subdirs/a/b/c.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/subdirs/subdirs/b/c.py
--rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/unsupported-dynamic/pyproject.toml
--rw-r--r--   0        0        0       67 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/unsupported-python-version/meson.build
--rw-r--r--   0        0        0      162 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/packages/unsupported-python-version/pyproject.toml
--rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_metadata.py
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_output.py
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_pep517.py
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_project.py
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_sdist.py
--rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_tags.py
--rw-r--r--   0        0        0     4732 1970-01-01 00:00:00.000000 meson_python-0.8.1/tests/test_wheel.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 meson_python-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 meson_python-0.9.0/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 meson_python-0.9.0/.github/workflows/ci-sage.yml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 meson_python-0.9.0/.github/workflows/tests-cygwin.yml
+-rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 meson_python-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 meson_python-0.9.0/.gitignore
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 meson_python-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 meson_python-0.9.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 meson_python-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 meson_python-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 meson_python-0.9.0/README.md
+-rw-r--r--   0        0        0       15 1970-01-01 00:00:00.000000 meson_python-0.9.0/codecov.yml
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/examples/spam/meson.build
+-rw-r--r--   0        0        0      194 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/examples/spam/pyproject.toml
+-rw-r--r--   0        0        0       55 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/examples/spam/src/__init__.py
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/examples/spam/src/spammodule.c
+-rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/usage/build-options.rst
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/usage/specific-behaviors.rst
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 meson_python-0.9.0/docs/usage/start.rst
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 meson_python-0.9.0/meson.build
+-rw-r--r--   0        0        0    38808 1970-01-01 00:00:00.000000 meson_python-0.9.0/mesonpy/__init__.py
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 meson_python-0.9.0/mesonpy/_compat.py
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 meson_python-0.9.0/mesonpy/_elf.py
+-rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 meson_python-0.9.0/mesonpy/_tags.py
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 meson_python-0.9.0/mesonpy/_util.py
+-rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 meson_python-0.9.0/noxfile.py
+-rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 meson_python-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 meson_python-0.9.0/setup.cfg
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/docs/__init__.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/docs/examples/__init__.py
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/docs/examples/conftest.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/docs/examples/test_spam.py
+-rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/configure-data/configure_data.py.in
+-rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/configure-data/meson.build
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/configure-data/pyproject.toml
+-rw-r--r--   0        0        0       56 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/dynamic-version/meson.build
+-rw-r--r--   0        0        0      134 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/dynamic-version/pyproject.toml
+-rw-r--r--   0        0        0       54 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable/example.c
+-rw-r--r--   0        0        0      118 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable/meson.build
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable/pyproject.toml
+-rwxr-xr-x   0        0        0       26 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable-bit/example-script.py
+-rw-r--r--   0        0        0       54 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable-bit/example.c
+-rwxr-xr-x   0        0        0       82 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable-bit/executable_module.py
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable-bit/meson.build
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/executable-bit/pyproject.toml
+-rw-r--r--   0        0        0       13 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/full-metadata/LICENSE
+-rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/full-metadata/README.md
+-rw-r--r--   0        0        0       54 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/full-metadata/meson.build
+-rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/full-metadata/pyproject.toml
+-rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library/example.c
+-rw-r--r--   0        0        0       41 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library/examplelib.c
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library/examplelib.h
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library/meson.build
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library/pyproject.toml
+-rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library-pep621/example.c
+-rw-r--r--   0        0        0       41 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library-pep621/examplelib.c
+-rw-r--r--   0        0        0      204 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library-pep621/meson.build
+-rw-r--r--   0        0        0      122 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/library-pep621/pyproject.toml
+-rw-r--r--   0        0        0       53 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/license-file/meson.build
+-rw-r--r--   0        0        0      168 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/license-file/pyproject.toml
+-rw-r--r--   0        0        0        7 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/license-file/something/LICENSE.custom
+-rw-r--r--   0        0        0       41 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/link-against-local-lib/examplelib.c
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/link-against-local-lib/examplelib.h
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/link-against-local-lib/examplemod.c
+-rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/link-against-local-lib/meson.build
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/link-against-local-lib/pyproject.toml
+-rw-r--r--   0        0        0      135 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/pure/meson.build
+-rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/pure/pure.py
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/pure/pyproject.toml
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/purelib-and-platlib/meson.build
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/purelib-and-platlib/plat.c
+-rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/purelib-and-platlib/pure.py
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/purelib-and-platlib/pyproject.toml
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/meson.build
+-rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/mypkg/__init__.py
+-rw-r--r--   0        0        0       76 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/mypkg/cy_extmod.pyx
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/mypkg/extmod.c
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/mypkg/meson.build
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/mypkg/submod/__init__.py
+-rw-r--r--   0        0        0       94 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/mypkg/submod/unknown_filetype.npq
+-rw-r--r--   0        0        0      143 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/pyproject.toml
+-rw-r--r--   0        0        0      126 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/scipy-like/tools/generate_config.py
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/subdirs/meson.build
+-rw-r--r--   0        0        0       69 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/subdirs/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/subdirs/subdirs/__init__.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/subdirs/subdirs/a/__init__.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/subdirs/subdirs/a/b/c.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/subdirs/subdirs/b/c.py
+-rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/unsupported-dynamic/pyproject.toml
+-rw-r--r--   0        0        0       67 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/unsupported-python-version/meson.build
+-rw-r--r--   0        0        0      162 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/packages/unsupported-python-version/pyproject.toml
+-rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_output.py
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_pep517.py
+-rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_project.py
+-rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_sdist.py
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_tags.py
+-rw-r--r--   0        0        0    10454 1970-01-01 00:00:00.000000 meson_python-0.9.0/tests/test_wheel.py
+-rw-r--r--   0        0        0     4477 1970-01-01 00:00:00.000000 meson_python-0.9.0/PKG-INFO
```

### Comparing `meson_python-0.8.1/.github/workflows/tests-cygwin.yml` & `meson_python-0.9.0/.github/workflows/tests-cygwin.yml`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,23 @@
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
+  cancel-in-progress: true
+
 jobs:
   pytest:
     runs-on: windows-latest
+    env:
+      FORCE_COLOR: true
     strategy:
       fail-fast: false
       matrix:
         python:
           - '3.10'
 
     steps:
@@ -35,13 +41,14 @@
             nox --version
 
       - name: Run tests
         run: nox -s test-${{ matrix.python }}
 
       - name: Send coverage report
         uses: codecov/codecov-action@v1
+        if: ${{ always() }}
         env:
           PYTHON: cygwin-${{ matrix.python }}
         with:
           flags: tests
           env_vars: PYTHON
           name: cygwin-${{ matrix.python }}
```

### Comparing `meson_python-0.8.1/.github/workflows/tests.yml` & `meson_python-0.9.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,33 @@
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
+  cancel-in-progress: true
+
 jobs:
   pytest:
     runs-on: ${{ matrix.os }}-latest
+    env:
+      FORCE_COLOR: true
     strategy:
       fail-fast: false
       matrix:
         os:
           - ubuntu
           - macos
           - windows
         python:
+          - 'pypy-3.8'
+          - 'pypy-3.9'
           - '3.7'
           - '3.8'
           - '3.9'
           - '3.10'
           - '3.11-dev'
 
     steps:
@@ -32,36 +40,42 @@
       - name: Set up target Python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
 
       - name: Pick environment to run
         run: |
-          import platform; import os; import sys; import codecs
-          base = '.'.join(map(str, sys.version_info[:2]))
-          env = 'BASE={}\n'.format(base)
-          print('Picked:\n{}for{}'.format(env, sys.version))
-          with codecs.open(os.environ['GITHUB_ENV'], 'a', 'utf-8') as file_handler:
-               file_handler.write(env)
+          import platform
+          import os
+          import sys
+          if platform.python_implementation() == 'PyPy':
+              base = f'pypy{sys.version_info.major}.{sys.version_info.minor}'
+          else:
+              base = f'{sys.version_info.major}.{sys.version_info.minor}'
+          env = f'BASE={base}\n'
+          print(f'Picked:\n{env}for {sys.version}')
+          with open(os.environ['GITHUB_ENV'], 'a', encoding='utf-8') as file:
+              file.write(env)
         shell: python
 
       - name: Set up Python for nox
         uses: actions/setup-python@v2
         with:
           python-version: 3.9
 
       - name: Install nox
         run: |
             python -m pip install nox
             nox --version
 
       - name: Run tests
-        run: nox -s test-${{ env.BASE }}
+        run: nox -v -s test-${{ env.BASE }}
 
       - name: Send coverage report
         uses: codecov/codecov-action@v1
+        if: ${{ always() }}
         env:
           PYTHON: ${{ matrix.python }}
         with:
           flags: tests
           env_vars: PYTHON
           name: ${{ matrix.python }}
```

### Comparing `meson_python-0.8.1/.pre-commit-config.yaml` & `meson_python-0.9.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ci:
   autofix_prs: false
   autoupdate_commit_msg: 'pre-commit: bump repositories'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.2.0
+  rev: v4.3.0
   hooks:
   - id: check-ast
   - id: check-builtin-literals
   - id: check-docstring-first
   - id: check-merge-conflict
   - id: check-yaml
   - id: check-toml
@@ -17,11 +17,11 @@
   - id: end-of-file-fixer
   - id: trailing-whitespace
 - repo: https://github.com/PyCQA/isort
   rev: 5.10.1
   hooks:
   - id: isort
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 5.0.4
   hooks:
   - id: flake8
     language_version: python3.8
```

### Comparing `meson_python-0.8.1/CHANGELOG.rst` & `meson_python-0.9.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 +++++++++
 Changelog
 +++++++++
 
 
+0.9.0 (29-09-2022)
+==================
+
+- More fixes on ABI tag detection
+- Fix incorrect tag on 32-bit Python running on a x86_64 host
+- Fix sdist permissions
+- Fix incorrect PyPy tags
+- Fix ``install_subdirs`` not being included in wheels
+- Take ``MACOSX_DEPLOYMENT_TARGET`` into account for the platform tag
+- Don't set the rpath on binaries if unneeded
+
+
 0.8.1 (28-07-2022)
 ==================
 
 - Fix ``UnboundLocalError`` in tag detection code
 
 
 0.8.0 (26-07-2022)
```

### Comparing `meson_python-0.8.1/LICENSE` & `meson_python-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/README.md` & `meson_python-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/docs/changelog.rst` & `meson_python-0.9.0/docs/changelog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 +++++++++
 Changelog
 +++++++++
 
 
+0.9.0 (29-09-2022)
+==================
+
+- More fixes on ABI tag detection
+- Fix incorrect tag on 32-bit Python running on a x86_64 host
+- Fix sdist permissions
+- Fix incorrect PyPy tags
+- Fix ``install_subdirs`` not being included in wheels
+- Take ``MACOSX_DEPLOYMENT_TARGET`` into account for the platform tag
+- Don't set the rpath on binaries if unneeded
+
+
 0.8.1 (28-07-2022)
 ==================
 
 - Fix ``UnboundLocalError`` in tag detection code
 
 
 0.8.0 (26-07-2022)
```

### Comparing `meson_python-0.8.1/docs/conf.py` & `meson_python-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/docs/index.rst` & `meson_python-0.9.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 
 .. toctree::
    :caption: Usage
    :hidden:
 
    usage/start
    usage/build-options
+   usage/specific-behaviors
 
 
 .. toctree::
    :caption: Release
    :hidden:
 
    changelog
```

### Comparing `meson_python-0.8.1/docs/usage/build-options.rst` & `meson_python-0.9.0/docs/usage/build-options.rst`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/docs/usage/start.rst` & `meson_python-0.9.0/docs/usage/start.rst`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/mesonpy/__init__.py` & `meson_python-0.9.0/mesonpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,21 @@
 
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import pyproject_metadata  # noqa: F401
     import wheel.wheelfile  # noqa: F401
 
 
-__version__ = '0.8.1'
+if sys.version_info >= (3, 8):
+    from functools import cached_property
+else:
+    cached_property = lambda x: property(functools.lru_cache(maxsize=None)(x))  # noqa: E731
+
+
+__version__ = '0.9.0'
 
 
 class _depstr:
     """Namespace that holds the requirement strings for dependencies we *might*
     need at runtime. Having them in one place makes it easier to update.
     """
     patchelf = 'patchelf >= 0.11.0'
@@ -130,66 +136,98 @@
 class _WheelBuilder():
     """Helper class to build wheels from projects."""
 
     # Maps wheel scheme names to Meson placeholder directories
     _SCHEME_MAP: ClassVar[Dict[str, Tuple[str, ...]]] = {
         'scripts': ('{bindir}',),
         'purelib': ('{py_purelib}',),
-        # {moduledir_shared} should be listed in platlib here too, but currently
-        # there is a Meson bug preventing us from using, so we will have to let
-        # that fallback on heuristics.
-        # see https://github.com/mesonbuild/meson/pull/9474
-        'platlib': ('{py_platlib}',),
+        'platlib': ('{py_platlib}', '{moduledir_shared}'),
         'headers': ('{includedir}',),
         'data': ('{datadir}',),
         # our custom location
         'mesonpy-libs': ('{libdir}', '{libdir_shared}')
     }
 
-    def __init__(self, project: Project) -> None:
+    def __init__(
+        self,
+        project: Project,
+        source_dir: pathlib.Path,
+        install_dir: pathlib.Path,
+        build_dir: pathlib.Path,
+        sources: Dict[str, Dict[str, Any]],
+        copy_files: Dict[str, str],
+    ) -> None:
         self._project = project
-        self._libs_build_dir = project._build_dir / 'mesonpy-wheel-libs'
+        self._source_dir = source_dir
+        self._install_dir = install_dir
+        self._build_dir = build_dir
+        self._sources = sources
+        self._copy_files = copy_files
+
+        self._libs_build_dir = self._build_dir / 'mesonpy-wheel-libs'
+
+    @cached_property
+    def _wheel_files(self) -> DefaultDict[str, List[Tuple[pathlib.Path, str]]]:
+        return self._map_to_wheel(self._sources, self._copy_files)
+
+    @property
+    def _has_internal_libs(self) -> bool:
+        return bool(self._wheel_files['mesonpy-libs'])
 
     @property
     def basename(self) -> str:
         """Normalized wheel name and version (eg. meson_python-1.0.0)."""
         return '{distribution}-{version}'.format(
             distribution=self._project.name.replace('-', '_'),
             version=self._project.version,
         )
 
     @property
     def name(self) -> str:
         """Wheel name, this includes the basename and tags."""
         return '{basename}-{python_tag}-{abi_tag}-{platform_tag}'.format(
             basename=self.basename,
-            python_tag=self._project.python_tag,
-            abi_tag=self._project.abi_tag,
-            platform_tag=self._project.platform_tag,
+            python_tag=self.python_tag,
+            abi_tag=self.abi_tag,
+            platform_tag=self.platform_tag,
         )
 
     @property
     def distinfo_dir(self) -> str:
         return f'{self.basename}.dist-info'
 
     @property
     def data_dir(self) -> str:
         return f'{self.basename}.data'
 
+    @cached_property
+    def is_pure(self) -> bool:
+        """Is the wheel "pure" (architecture independent)?"""
+        # XXX: I imagine some users might want to force the package to be
+        # non-pure, but I think it's better that we evaluate use-cases as they
+        # arise and make sure allowing the user to override this is indeed the
+        # best option for the use-case.
+        if self._wheel_files['platlib']:
+            return False
+        for _, file in self._wheel_files['scripts']:
+            if self._is_native(file):
+                return False
+        return True
+
     @property
     def wheel(self) -> bytes:  # noqa: F811
         """Return WHEEL file for dist-info."""
         return textwrap.dedent('''
             Wheel-Version: 1.0
             Generator: meson
             Root-Is-Purelib: {is_purelib}
             Tag: {tags}
         ''').strip().format(
-            is_purelib='true' if self._project.is_pure else 'false',
-            tags=f'{self._project.python_tag}-{self._project.abi_tag}-{self._project.platform_tag}',
+            is_purelib='true' if self.is_pure else 'false',
+            tags=f'{self.python_tag}-{self.abi_tag}-{self.platform_tag}',
         ).encode()
 
     @property
     def _debian_python(self) -> bool:
         """Check if we are running on Debian-patched Python."""
         try:
             import distutils
@@ -197,32 +235,206 @@
                 import distutils.command.install
             except ModuleNotFoundError:
                 raise ModuleNotFoundError('Unable to import distutils, please install python3-distutils')
             return 'deb_system' in distutils.command.install.INSTALL_SCHEMES
         except ModuleNotFoundError:
             return False
 
-    def _is_elf(self, file: Union[str, pathlib.Path]) -> bool:
-        """Check if file is an ELF file."""
+    @property
+    def python_tag(self) -> str:
+        selected_tag = self._select_abi_tag()
+        if selected_tag and selected_tag.python:
+            return selected_tag.python
+        return 'py3'
+
+    @property
+    def abi_tag(self) -> str:
+        selected_tag = self._select_abi_tag()
+        if selected_tag:
+            return selected_tag.abi
+        return 'none'
+
+    @cached_property
+    def platform_tag(self) -> str:
+        if self.is_pure:
+            return 'any'
+        # XXX: Choose the sysconfig platform here and let something like auditwheel
+        #      fix it later if there are system dependencies (eg. replace it with a manylinux tag)
+        platform_ = sysconfig.get_platform()
+        parts = platform_.split('-')
+        if parts[0] == 'macosx':
+            target = os.environ.get('MACOSX_DEPLOYMENT_TARGET')
+            if target:
+                print(
+                    '{yellow}MACOSX_DEPLOYMENT_TARGET is set so we are setting the '
+                    'platform tag to {target}{reset}'.format(target=target, **_STYLES)
+                )
+                parts[1] = target
+            else:
+                # If no target macOS version is specified fallback to
+                # platform.mac_ver() instead of sysconfig.get_platform() as the
+                # latter specifies the target macOS version Python was built
+                # against.
+                parts[1] = platform.mac_ver()[0]
+
+            if parts[1] in ('11', '12'):
+                # Workaround for bug where pypa/packaging does not consider macOS
+                # tags without minor versions valid. Some Python flavors (Homebrew
+                # for example) on macOS started to do this in version 11, and
+                # pypa/packaging should handle things correctly from version 13 and
+                # forward, so we will add a 0 minor version to MacOS 11 and 12.
+                # https://github.com/FFY00/meson-python/issues/91
+                # https://github.com/pypa/packaging/issues/578
+                parts[1] += '.0'
+
+            platform_ = '-'.join(parts)
+        elif parts[0] == 'linux' and parts[1] == 'x86_64' and sys.maxsize == 0x7fffffff:
+            # 32-bit Python running on an x86_64 host
+            # https://github.com/FFY00/meson-python/issues/123
+            parts[1] = 'i686'
+            platform_ = '-'.join(parts)
+        return platform_.replace('-', '_').replace('.', '_')
+
+    def _calculate_file_abi_tag_heuristic_windows(self, filename: str) -> Optional[mesonpy._tags.Tag]:
+        """Try to calculate the Windows tag from the Python extension file name."""
+        match = _WINDOWS_NATIVE_MODULE_REGEX.match(filename)
+        if not match:
+            return None
+        tag = match.group('tag')
+
+        try:
+            return mesonpy._tags.StableABITag(tag)
+        except ValueError:
+            return mesonpy._tags.InterpreterTag(tag)
+
+    def _calculate_file_abi_tag_heuristic_posix(self, filename: str) -> Optional[mesonpy._tags.Tag]:
+        """Try to calculate the Posix tag from the Python extension file name."""
+        # sysconfig is not guaranted to export SHLIB_SUFFIX but let's be
+        # preventive and check its value to make sure it matches our expectations
+        try:
+            extension = sysconfig.get_config_vars().get('SHLIB_SUFFIX', '.so')
+            if extension != '.so':
+                raise NotImplementedError(
+                    f"We don't currently support the {extension} extension. "
+                    'Please report this to https://github.com/FFY00/mesonpy/issues '
+                    'and include information about your operating system.'
+                )
+        except KeyError:
+            warnings.warn(
+                'sysconfig does not export SHLIB_SUFFIX, so we are unable to '
+                'perform the sanity check regarding the extension suffix. '
+                'Please report this to https://github.com/FFY00/mesonpy/issues '
+                'and include the output of `python -m sysconfig`.'
+            )
+        match = _LINUX_NATIVE_MODULE_REGEX.match(filename)
+        if not match:  # this file does not appear to be a native module
+            return None
+        tag = match.group('tag')
+
+        try:
+            return mesonpy._tags.StableABITag(tag)
+        except ValueError:
+            return mesonpy._tags.InterpreterTag(tag)
+
+    def _calculate_file_abi_tag_heuristic(self, filename: str) -> Optional[mesonpy._tags.Tag]:
+        """Try to calculate the ABI tag from the Python extension file name."""
+        if os.name == 'nt':
+            return self._calculate_file_abi_tag_heuristic_windows(filename)
+        # everything else *should* follow the POSIX way, at least to my knowledge
+        return self._calculate_file_abi_tag_heuristic_posix(filename)
+
+    def _file_list_repr(self, files: Collection[str], prefix: str = '\t\t', max_count: int = 3) -> str:
+        if len(files) > max_count:
+            files = list(itertools.islice(files, max_count)) + [f'(... +{len(files)}))']
+        return ''.join(f'{prefix}- {file}\n' for file in files)
+
+    def _files_by_tag(self) -> Mapping[mesonpy._tags.Tag, Collection[str]]:
+        """Map files into ABI tags."""
+        files_by_tag: Dict[mesonpy._tags.Tag, List[str]] = collections.defaultdict(list)
+
+        for _, file in self._wheel_files['platlib']:
+            # if in platlib, calculate the ABI tag
+            tag = self._calculate_file_abi_tag_heuristic(file)
+            if tag:
+                files_by_tag[tag].append(file)
+
+        return files_by_tag
+
+    def _select_abi_tag(self) -> Optional[mesonpy._tags.Tag]:  # noqa: C901
+        """Given a list of ABI tags, selects the most specific one.
+
+        Raises an error if there are incompatible tags.
+        """
+        # Possibilities:
+        #   - interpreter specific (cpython/pypy/etc, version)
+        #   - stable abi (abiX)
+        tags = self._files_by_tag()
+        selected_tag = None
+        for tag, files in tags.items():
+            # no selected tag yet, let's assign this one
+            if not selected_tag:
+                selected_tag = tag
+            # interpreter tag
+            elif isinstance(tag, mesonpy._tags.InterpreterTag):
+                if tag != selected_tag:
+                    if isinstance(selected_tag, mesonpy._tags.InterpreterTag):
+                        raise ValueError(
+                            'Found files with incompatible ABI tags:\n'
+                            + self._file_list_repr(tags[selected_tag])
+                            + '\tand\n'
+                            + self._file_list_repr(files)
+                        )
+                    selected_tag = tag
+            # stable ABI
+            elif isinstance(tag, mesonpy._tags.StableABITag):
+                if isinstance(selected_tag, mesonpy._tags.StableABITag) and tag != selected_tag:
+                    raise ValueError(
+                        'Found files with incompatible ABI tags:\n'
+                        + self._file_list_repr(tags[selected_tag])
+                        + '\tand\n'
+                        + self._file_list_repr(files)
+                    )
+        return selected_tag
+
+    def _is_native(self, file: Union[str, pathlib.Path]) -> bool:
+        """Check if file is a native file."""
+        self._project.build()  # the project needs to be built for this :/
+
         with open(file, 'rb') as f:
-            return f.read(4) == b'\x7fELF'
+            if platform.system() == 'Linux':
+                return f.read(4) == b'\x7fELF'  # ELF
+            elif platform.system() == 'Darwin':
+                return f.read(4) in (
+                    b'\xfe\xed\xfa\xce',  # 32-bit
+                    b'\xfe\xed\xfa\xcf',  # 64-bit
+                    b'\xcf\xfa\xed\xfe',  # arm64
+                    b'\xca\xfe\xba\xbe',  # universal / fat (same as java class so beware!)
+                )
+            elif platform.system() == 'Windows':
+                return f.read(2) == b'MZ'
+
+        # For unknown platforms, check for file extensions.
+        _, ext = os.path.splitext(file)
+        if ext in ('.so', '.a', '.out', '.exe', '.dll', '.dylib', '.pyd'):
+            return True
+        return False
 
     def _warn_unsure_platlib(self, origin: pathlib.Path, destination: pathlib.Path) -> None:
         """Warn if we are unsure if the file should be mapped to purelib or platlib.
 
         This happens when we use heuristics to try to map a file purelib or
         platlib but can't differentiate between the two. In which case, we place
         the file in platlib to be safe and warn the user.
 
         If we can detect the file is architecture dependent and indeed does not
         belong in purelib, we will skip the warning.
         """
         # {moduledir_shared} is currently handled in heuristics due to a Meson bug,
         # but we know that files that go there are supposed to go to platlib.
-        if self._is_elf(origin) or destination.root == '{moduledir_shared}':
+        if self._is_native(origin):
             # The file is architecture dependent and does not belong in puredir,
             # so the warning is skipped.
             return
         warnings.warn(
             'Could not tell if file was meant for purelib or platlib, '
             f'so it was mapped to platlib: {origin} ({destination})',
             stacklevel=2,
@@ -240,22 +452,21 @@
         if self._debian_python:
             search_path = origin
             while search_path != search_path.parent:
                 search_path = search_path.parent
                 if search_path.name == 'dist-packages' and search_path.parent.parent.name == 'lib':
                     calculated_path = origin.relative_to(search_path)
                     warnings.warn(f'File matched Debian heuristic ({calculated_path}): {origin} ({destination})')
-                    if not destination.root == '{moduledir_shared}':
-                        self._warn_unsure_platlib(origin, destination)
+                    self._warn_unsure_platlib(origin, destination)
                     return 'platlib', calculated_path
         # Try to map to the interpreter purelib or platlib
         for scheme in ('purelib', 'platlib'):
             # try to match the install path on the system to one of the known schemes
             scheme_path = pathlib.Path(sys_paths[scheme]).absolute()
-            destdir_scheme_path = self._project._install_dir / scheme_path.relative_to(scheme_path.anchor)
+            destdir_scheme_path = self._install_dir / scheme_path.relative_to(scheme_path.anchor)
             try:
                 wheel_path = pathlib.Path(origin).relative_to(destdir_scheme_path)
             except ValueError:
                 continue
             if sys_paths['purelib'] == sys_paths['platlib']:
                 self._warn_unsure_platlib(origin, destination)
             return 'platlib', wheel_path
@@ -306,96 +517,99 @@
                 warnings.warn(
                     'File could not be mapped to an equivalent wheel directory: '
                     '{} ({})'.format(copy_files[file], meson_destination)
                 )
 
         return wheel_files
 
-    def _install_file(
+    def _install_path(
         self,
         wheel_file: wheel.wheelfile.WheelFile,  # type: ignore[name-defined]
         counter: mesonpy._util.CLICounter,
         origin: Path,
         destination: pathlib.Path,
     ) -> None:
-        """"Install" file into the wheel and do the necessary processing before
-        doing so.
+        """"Install" file or directory into the wheel
+        and do the necessary processing before doing so.
 
         Some files might need to be fixed up to set the RPATH to the internal
         library directory on Linux wheels for eg.
         """
         location = os.fspath(destination).replace(os.path.sep, '/')
         counter.update(location)
 
         # fix file
-        if platform.system() == 'Linux':
-            # add .mesonpy.libs to the RPATH of ELF files
-            if self._is_elf(os.fspath(origin)):
-                # copy ELF to our working directory to avoid Meson having to regenerate the file
-                new_origin = self._libs_build_dir / pathlib.Path(origin).relative_to(self._project._build_dir)
-                os.makedirs(new_origin.parent, exist_ok=True)
-                shutil.copy2(origin, new_origin)
-                origin = new_origin
-                # add our in-wheel libs folder to the RPATH
-                elf = mesonpy._elf.ELF(origin)
-                libdir_path = f'$ORIGIN/{os.path.relpath(f".{self._project.name}.mesonpy.libs", destination.parent)}'
-                if libdir_path not in elf.rpath:
-                    elf.rpath = [*elf.rpath, libdir_path]
+        if os.path.isdir(origin):
+            for root, dirnames, filenames in os.walk(str(origin)):
+                # Sort the directory names so that `os.walk` will walk them in a
+                # defined order on the next iteration.
+                dirnames.sort()
+                for name in sorted(filenames):
+                    path = os.path.normpath(os.path.join(root, name))
+                    if os.path.isfile(path):
+                        arcname = os.path.join(destination, os.path.relpath(path, origin).replace(os.path.sep, '/'))
+                        wheel_file.write(path, arcname)
+        else:
+            if self._has_internal_libs and platform.system() == 'Linux':
+                # add .mesonpy.libs to the RPATH of ELF files
+                if self._is_native(os.fspath(origin)):
+                    # copy ELF to our working directory to avoid Meson having to regenerate the file
+                    new_origin = self._libs_build_dir / pathlib.Path(origin).relative_to(self._build_dir)
+                    os.makedirs(new_origin.parent, exist_ok=True)
+                    shutil.copy2(origin, new_origin)
+                    origin = new_origin
+                    # add our in-wheel libs folder to the RPATH
+                    elf = mesonpy._elf.ELF(origin)
+                    libdir_path = f'$ORIGIN/{os.path.relpath(f".{self._project.name}.mesonpy.libs", destination.parent)}'
+                    if libdir_path not in elf.rpath:
+                        elf.rpath = [*elf.rpath, libdir_path]
 
-        wheel_file.write(origin, location)
+            wheel_file.write(origin, location)
 
-    def build(
-        self,
-        sources: Dict[str, Dict[str, Any]],
-        copy_files: Dict[str, str],
-        directory: Path,
-    ) -> pathlib.Path:
+    def build(self, directory: Path) -> pathlib.Path:
         import wheel.wheelfile
 
         self._project.build()  # ensure project is built
 
         wheel_file = pathlib.Path(directory, f'{self.name}.whl')
-        wheel_files = self._map_to_wheel(sources, copy_files)
 
         with wheel.wheelfile.WheelFile(wheel_file, 'w') as whl:
             # add metadata
             whl.writestr(f'{self.distinfo_dir}/METADATA', self._project.metadata)
             whl.writestr(f'{self.distinfo_dir}/WHEEL', self.wheel)
 
             # add license (see https://github.com/FFY00/meson-python/issues/88)
-            if self._project._metadata:
-                license_ = self._project._metadata.license
-                if license_ and license_.file:
-                    whl.write(
-                        self._project._source_dir / license_.file,
-                        f'{self.distinfo_dir}/{os.path.basename(license_.file)}',
-                    )
+            if self._project.license_file:
+                whl.write(
+                    self._source_dir / self._project.license_file,
+                    f'{self.distinfo_dir}/{os.path.basename(self._project.license_file)}',
+                )
 
             print('{light_blue}{bold}Copying files to wheel...{reset}'.format(**_STYLES))
             with mesonpy._util.cli_counter(
-                len(list(itertools.chain.from_iterable(wheel_files.values()))),
+                len(list(itertools.chain.from_iterable(self._wheel_files.values()))),
             ) as counter:
                 # install root scheme files
-                root_scheme = 'purelib' if self._project.is_pure else 'platlib'
-                for destination, origin in wheel_files[root_scheme]:
-                    self._install_file(whl, counter, origin, destination)
+                root_scheme = 'purelib' if self.is_pure else 'platlib'
+                for destination, origin in self._wheel_files[root_scheme]:
+                    self._install_path(whl, counter, origin, destination)
 
                 # install bundled libraries
-                for destination, origin in wheel_files['mesonpy-libs']:
+                for destination, origin in self._wheel_files['mesonpy-libs']:
                     assert platform.system() == 'Linux', 'Bundling libraries in wheel is currently only supported in POSIX!'
                     destination = pathlib.Path(f'.{self._project.name}.mesonpy.libs', destination)
-                    self._install_file(whl, counter, origin, destination)
+                    self._install_path(whl, counter, origin, destination)
 
                 # install the other schemes
                 for scheme in self._SCHEME_MAP:
                     if scheme in (root_scheme, 'mesonpy-libs'):
                         continue
-                    for destination, origin in wheel_files[scheme]:
+                    for destination, origin in self._wheel_files[scheme]:
                         destination = pathlib.Path(self.data_dir, scheme, destination)
-                        self._install_file(whl, counter, origin, destination)
+                        self._install_path(whl, counter, origin, destination)
 
         return wheel_file
 
 
 class Project():
     """Meson project wrapper to generate Python artifacts."""
 
@@ -439,15 +653,15 @@
         # make sure the build dir exists
         self._build_dir.mkdir(exist_ok=True)
         self._install_dir.mkdir(exist_ok=True)
 
         # write the native file
         native_file_data = textwrap.dedent(f'''
             [binaries]
-            python3 = '{sys.executable}'
+            python = '{sys.executable}'
         ''')
         native_file_mismatch = (
             not self._meson_native_file.exists()
             or self._meson_native_file.read_text() != native_file_data
         )
         if native_file_mismatch:
             try:
@@ -525,14 +739,25 @@
             self._metadata.requires_python.prereleases = True
             if platform.python_version().rstrip('+') not in self._metadata.requires_python:
                 raise MesonBuilderError(
                     f'Unsupported Python version `{platform.python_version()}`, '
                     f'expected `{self._metadata.requires_python}`'
                 )
 
+    @cached_property
+    def _wheel_builder(self) -> _WheelBuilder:
+        return _WheelBuilder(
+            self,
+            self._source_dir,
+            self._install_dir,
+            self._build_dir,
+            self._install_plan,
+            self._copy_files,
+        )
+
     @functools.lru_cache(maxsize=None)
     def build(self) -> None:
         """Trigger the Meson build."""
         self._meson('compile')
         self._meson('install', '--destdir', os.fspath(self._install_dir))
 
     @classmethod
@@ -608,15 +833,15 @@
         if self._metadata and 'version' not in self._metadata.dynamic:
             version = str(self._metadata.version)
         else:
             version = self._meson_version
         assert isinstance(version, str)
         return version
 
-    @property  # type: ignore[misc]
+    @property
     @functools.lru_cache(maxsize=1)
     def metadata(self) -> bytes:  # noqa: C901
         """Project metadata."""
         # the rest of the keys are only available when using PEP 621 metadata
         if not self.pep621:
             return textwrap.dedent(f'''
                 Metadata-Version: 2.1
@@ -628,217 +853,31 @@
         assert self._metadata
         # use self.version as the version may be dynamic -- fetched from Meson
         core_metadata = self._metadata.as_rfc822()
         core_metadata.headers['Version'] = [self.version]
         return bytes(core_metadata)
 
     @property
+    def license_file(self) -> Optional[pathlib.Path]:
+        if self._metadata:
+            license_ = self._metadata.license
+            if license_ and license_.file:
+                return pathlib.Path(license_.file)
+        return None
+
+    @property
     def is_pure(self) -> bool:
         """Is the wheel "pure" (architecture independent)?"""
-        # XXX: I imagine some users might want to force the package to be
-        # non-pure, but I think it's better that we evaluate use-cases as they
-        # arise and make sure allowing the user to override this is indeed the
-        # best option for the use-case.
-        not_pure = ('{bindir}', '{libdir_shared}', '{libdir_static}', '{py_platlib}', '{moduledir_shared}')
-        for data_type, files in self._install_plan.items():
-            for entry in files.values():
-                if entry['destination'] is None:  # pragma: no cover
-                    continue
-                if any(key in entry['destination'] for key in not_pure):
-                    return False
-        return True
+        return bool(self._wheel_builder.is_pure)
 
     @property
     def pep621(self) -> bool:
         """Does the project use PEP 621 metadata?"""
         return self._pep621
 
-    @property
-    def python_tag(self) -> str:
-        selected_tag = self._select_abi_tag()
-        if selected_tag and selected_tag.python:
-            return selected_tag.python
-        return 'py3'
-
-    @property
-    def abi_tag(self) -> str:
-        selected_tag = self._select_abi_tag()
-        if selected_tag:
-            return selected_tag.abi
-        return 'none'
-
-    @property
-    def platform_tag(self) -> str:
-        if self.is_pure:
-            return 'any'
-        # XXX: Choose the sysconfig platform here and let something like auditwheel
-        #      fix it later if there are system dependencies (eg. replace it with a manylinux tag)
-        platform_ = sysconfig.get_platform()
-        parts = platform_.split('-')
-        if parts[0] == 'macosx' and parts[1] in ('11', '12'):
-            # Workaround for bug where pypa/packaging does not consider macOS
-            # tags without minor versions valid. Some Python flavors (Homebrew
-            # for example) on macOS started to do this in version 11, and
-            # pypa/packaging should handle things correctly from version 13 and
-            # forward, so we will add a 0 minor version to MacOS 11 and 12.
-            # https://github.com/FFY00/meson-python/issues/91
-            # https://github.com/pypa/packaging/issues/578
-            parts[1] += '.0'
-            platform_ = '-'.join(parts)
-        return platform_.replace('-', '_').replace('.', '_')
-
-    def _calculate_file_abi_tag_heuristic_windows(self, filename: str) -> Optional[mesonpy._tags.Tag]:
-        """Try to calculate the Windows tag from the Python extension file name."""
-        match = _WINDOWS_NATIVE_MODULE_REGEX.match(filename)
-        if not match:
-            return None
-        tag = match.group('tag')
-
-        try:
-            return mesonpy._tags.StableABITag(tag)
-        except ValueError:
-            return mesonpy._tags.WindowsInterpreterTag(tag)
-
-    def _calculate_file_abi_tag_heuristic_posix(self, filename: str) -> Optional[mesonpy._tags.Tag]:
-        """Try to calculate the Posix tag from the Python extension file name."""
-        # sysconfig is not guaranted to export SHLIB_SUFFIX but let's be
-        # preventive and check its value to make sure it matches our expectations
-        try:
-            extension = sysconfig.get_config_vars().get('SHLIB_SUFFIX', '.so')
-            if extension != '.so':
-                raise NotImplementedError(
-                    f"We don't currently support the {extension} extension. "
-                    'Please report this to https://github.com/FFY00/mesonpy/issues '
-                    'and include information about your operating system.'
-                )
-        except KeyError:
-            warnings.warn(
-                'sysconfig does not export SHLIB_SUFFIX, so we are unable to '
-                'perform the sanity check regarding the extension suffix. '
-                'Please report this to https://github.com/FFY00/mesonpy/issues '
-                'and include the output of `python -m sysconfig`.'
-            )
-        match = _LINUX_NATIVE_MODULE_REGEX.match(filename)
-        if not match:  # this file does not appear to be a native module
-            return None
-        tag = match.group('tag')
-
-        try:
-            return mesonpy._tags.StableABITag(tag)
-        except ValueError:
-            return mesonpy._tags.LinuxInterpreterTag(tag)
-
-    def _calculate_file_abi_tag_heuristic(self, filename: str) -> Optional[mesonpy._tags.Tag]:
-        """Try to calculate the ABI tag from the Python extension file name."""
-        if os.name == 'nt':
-            return self._calculate_file_abi_tag_heuristic_windows(filename)
-        # everything else *should* follow the POSIX way, at least to my knowledge
-        return self._calculate_file_abi_tag_heuristic_posix(filename)
-
-    def _file_list_repr(self, files: Collection[str], prefix: str = '\t\t', max_count: int = 3) -> str:
-        if len(files) > max_count:
-            files = list(itertools.islice(files, max_count)) + [f'(... +{len(files)}))']
-        return ''.join(f'{prefix}- {file}\n' for file in files)
-
-    def _files_by_tag(self) -> Mapping[mesonpy._tags.Tag, Collection[str]]:
-        """Map files into ABI tags."""
-        files_by_tag: Dict[mesonpy._tags.Tag, List[str]] = collections.defaultdict(list)
-        for file, details in self._install_plan.get('targets', {}).items():
-            destination = pathlib.Path(details['destination'])
-            from_heuristic = False
-
-            # if in platlib, calculate the ABI tag
-            if not (
-                mesonpy._compat.is_relative_to(destination, '{py_platlib}')
-                or mesonpy._compat.is_relative_to(destination, '{moduledir_shared}')
-            ):
-                # XXX: Ideally we would just check the anchor placeholder in the
-                #      path (eg. check if it is {py_platlib}) but Meson seems to
-                #      have a bug where it sometimes returns a full path without
-                #      placeholder, so we will check if the file path is
-                #      relative to platlib.
-                #      This can be problematic because the platlib path might be
-                #      same one used for other schemes. In these situations we
-                #      will be picking up files are not supposed to be in
-                #      platlib, and that could just be supporting files.
-                #      See https://github.com/FFY00/meson-python/issues/95
-                #      Meson bug: https://github.com/mesonbuild/meson/issues/10601
-                sys_vars = sysconfig.get_config_vars().copy()
-                sys_vars['base'] = sys_vars['platbase'] = sys.base_prefix
-                platlib = sysconfig.get_path('platlib', vars=sys_vars)
-                if platlib and mesonpy._compat.is_relative_to(destination, platlib):
-                    from_heuristic = True
-                else:
-                    continue
-
-            tag = self._calculate_file_abi_tag_heuristic(file)
-            if tag:
-                if from_heuristic:
-                    warnings.warn(
-                        'Could not tell with certainty if this file was meant '
-                        'to be mapped to platlib, but it was used to calculate '
-                        f'the ABI tag: {destination}'
-                    )
-                files_by_tag[tag].append(file)
-
-        return files_by_tag
-
-    def _select_abi_tag(self) -> Optional[mesonpy._tags.Tag]:  # noqa: C901
-        """Given a list of ABI tags, selects the most specific one.
-
-        Raises an error if there are incompatible tags.
-        """
-        # Possibilities:
-        #   - interpreter specific (cpython/pypy/etc, version)
-        #   - stable abi (abiX)
-        tags = self._files_by_tag()
-        selected_tag = None
-        for tag, files in tags.items():
-            if __debug__:  # sanity check
-                if os.name == 'nt':
-                    assert not isinstance(tag, mesonpy._tags.LinuxInterpreterTag)
-                else:
-                    assert not isinstance(tag, mesonpy._tags.WindowsInterpreterTag)
-            # no selected tag yet, let's assign this one
-            if not selected_tag:
-                selected_tag = tag
-            # interpreter tags
-            elif isinstance(tag, mesonpy._tags.LinuxInterpreterTag):
-                if tag != selected_tag:
-                    if isinstance(selected_tag, mesonpy._tags.LinuxInterpreterTag):
-                        raise ValueError(
-                            'Found files with incompatible ABI tags:\n'
-                            + self._file_list_repr(tags[selected_tag])
-                            + '\tand\n'
-                            + self._file_list_repr(files)
-                        )
-                    selected_tag = tag
-            elif isinstance(tag, mesonpy._tags.WindowsInterpreterTag):
-                if tag != selected_tag:
-                    if isinstance(selected_tag, mesonpy._tags.WindowsInterpreterTag):
-                        warnings.warn(
-                            'Found files with different ABI tags but couldn\'t tell '
-                            'if they are incompatible:\n'
-                            + self._file_list_repr(tags[selected_tag])
-                            + '\tand\n'
-                            + self._file_list_repr(files)
-                            + 'Please report this to https://github.com/FFY00/mesonpy/issues.'
-                        )
-                    selected_tag = tag
-            # stable ABI
-            elif isinstance(tag, mesonpy._tags.StableABITag):
-                if isinstance(selected_tag, mesonpy._tags.StableABITag) and tag != selected_tag:
-                    raise ValueError(
-                        'Found files with incompatible ABI tags:\n'
-                        + self._file_list_repr(tags[selected_tag])
-                        + '\tand\n'
-                        + self._file_list_repr(files)
-                    )
-        return selected_tag
-
     def sdist(self, directory: Path) -> pathlib.Path:
         """Generates a sdist (source distribution) in the specified directory."""
         # generate meson dist file
         self._meson('dist', '--allow-dirty', '--no-tests', '--formats', 'gztar')
 
         # move meson dist file to output path
         dist_name = f'{self.name}-{self.version}'
@@ -859,15 +898,17 @@
                     continue
                 path = self._source_dir.joinpath(*member_parts[1:])
 
                 if not path.is_file():
                     continue
 
                 info = tarfile.TarInfo(member.name)
-                info.size = os.path.getsize(path)
+                file_stat = os.stat(path)
+                info.size = file_stat.st_size
+                info.mode = int(oct(file_stat.st_mode)[-3:], 8)
 
                 # rewrite the path if necessary, to match the sdist distribution name
                 if dist_name != meson_dist_name:
                     info.name = pathlib.Path(
                         dist_name,
                         path.relative_to(self._source_dir)
                     ).as_posix()
@@ -882,15 +923,15 @@
             pkginfo_info.size = len(self.metadata)  # type: ignore[arg-type]
             tar.addfile(pkginfo_info, fileobj=io.BytesIO(self.metadata))  # type: ignore[arg-type]
 
         return sdist
 
     def wheel(self, directory: Path) -> pathlib.Path:  # noqa: F811
         """Generates a wheel (binary distribution) in the specified directory."""
-        wheel = _WheelBuilder(self).build(self._install_plan, self._copy_files, self._build_dir)
+        wheel = self._wheel_builder.build(self._build_dir)
 
         final_wheel = pathlib.Path(directory, wheel.name)
         shutil.move(os.fspath(wheel), final_wheel)
         return final_wheel
 
 
 @contextlib.contextmanager
```

### Comparing `meson_python-0.8.1/mesonpy/_compat.py` & `meson_python-0.9.0/mesonpy/_compat.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/mesonpy/_elf.py` & `meson_python-0.9.0/mesonpy/_elf.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 class ELF:
     def __init__(self, path: Path) -> None:
         self._path = os.fspath(path)
         self._rpath: Optional[Collection[str]] = None
         self._needed: Optional[Collection[str]] = None
 
     def _patchelf(self, *args: str) -> str:
-        return subprocess.check_output(['patchelf', *args, self._path]).decode()
+        return subprocess.check_output(['patchelf', *args, self._path], stderr=subprocess.STDOUT).decode()
 
     @property
     def rpath(self) -> Collection[str]:
-        if not self._rpath:
-            self._rpath = self._patchelf('--print-rpath').strip().split(';')
-        return self._rpath
+        if self._rpath is None:
+            rpath = self._patchelf('--print-rpath').strip()
+            self._rpath = rpath.split(':') if rpath else []
+        return frozenset(self._rpath)
 
     @rpath.setter
     def rpath(self, value: Collection[str]) -> None:
         self._patchelf('--set-rpath', ':'.join(value))
         self._rpath = value
 
     @property
```

### Comparing `meson_python-0.8.1/mesonpy/_tags.py` & `meson_python-0.9.0/mesonpy/_tags.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Quansight, LLC
 # SPDX-FileCopyrightText: 2021 Filipe Laíns <lains@riseup.net>
 
 import abc
 import re
-import sys
-import warnings
 
 from typing import Any, Optional
 
 from mesonpy._compat import Literal, Sequence
 
 
 class Tag(abc.ABC):
@@ -57,28 +55,34 @@
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, self.__class__) and other.abi_number == self.abi_number
 
     def __hash__(self) -> int:
         return hash(str(self))
 
 
-class LinuxInterpreterTag(Tag):
+class InterpreterTag(Tag):
     def __init__(self, value: str) -> None:
         parts = value.split('-')
         if len(parts) < 2:
             raise ValueError(
                 'Invalid PEP 3149 interpreter tag, expected at '
                 f'least 2 parts but got {len(parts)}'
             )
 
+        # On Windows, file extensions look like `.cp311-win_amd64.pyd`, so the
+        # implementation part (`cpython-`) is different from Linux. Handle that here:
+        if parts[0].startswith('cp3'):
+            parts.insert(0, 'cpython')
+            parts[1] = parts[1][2:]  # strip 'cp'
+
         self._implementation = parts[0]
         self._interpreter_version = parts[1]
         self._additional_information = parts[2:]
 
-        if self.implementation not in ('cpython', 'pypy', 'pypy3'):
+        if self.implementation != 'cpython' and not self.implementation.startswith('pypy'):
             raise NotImplementedError(
                 f'Unknown Python implementation: {self.implementation}. '
                 'Please report this to https://github.com/FFY00/mesonpy/issues '
                 'and include information about the Python distribution you are using.'
             )
 
     @property
@@ -101,67 +105,30 @@
         ))
 
     @property
     def python(self) -> str:
         if self.implementation == 'cpython':
             # The Python tag for CPython does not seem to include the flags suffixes.
             return f'cp{self.interpreter_version}'.rstrip('dmu')
-        elif self.implementation in ('pypy', 'pypy3'):
-            interpreter_version = f'{sys.version_info[0]}{sys.version_info[1]}'
-            return f'pp{interpreter_version}'
+        elif self.implementation.startswith('pypy'):
+            return f'pp{self.implementation[4:]}'
+            # XXX: FYI older PyPy version use the following model
+            #      pp{self.implementation[4]}{self.interpreter_version[2:]}
         raise ValueError(f'Unknown implementation: {self.implementation}')
 
     @property
     def abi(self) -> str:
-        # XXX: This is a bit flimsy and needs custom logic to support each case,
-        #      but currently there's no better way to do it.
         if self.implementation == 'cpython':
             return f'cp{self.interpreter_version}'
-        elif self.implementation == 'pypy':
-            return f'pypy_{self.interpreter_version}'
-        elif self.implementation == 'pypy3':
-            return f'pypy3_{self.interpreter_version}'
+        elif self.implementation.startswith('pypy'):
+            return f'{self.implementation}_{self.interpreter_version}'
         raise ValueError(f'Unknown implementation: {self.implementation}')
 
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, self.__class__)
             and other.implementation == self.implementation
             and other.interpreter_version == self.interpreter_version
         )
 
     def __hash__(self) -> int:
         return hash(str(self))
-
-
-class WindowsInterpreterTag(Tag):
-    def __init__(self, value: str) -> None:
-        # XXX: This is not actually standardized, so our implementation relies
-        #      on observing how the current software behaves!
-        self._parts = value.split('-')
-        if len(self.parts) != 2:
-            warnings.warn(
-                'Unexpected native module tag name, the ABI dectection might be broken. '
-                'Please report this to https://github.com/FFY00/mesonpy/issues '
-                'and include information about the Python distribution you are using.'
-            )
-
-    @property
-    def parts(self) -> Sequence[str]:
-        return tuple(self._parts)
-
-    def __str__(self) -> str:
-        return '-'.join(self.parts)
-
-    @property
-    def python(self) -> str:
-        return self.abi
-
-    @property
-    def abi(self) -> str:
-        return self._parts[0]
-
-    def __eq__(self, other: Any) -> bool:
-        return isinstance(other, self.__class__) and other.parts == self.parts
-
-    def __hash__(self) -> int:
-        return hash(str(self))
```

### Comparing `meson_python-0.8.1/mesonpy/_util.py` & `meson_python-0.9.0/mesonpy/_util.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/noxfile.py` & `meson_python-0.9.0/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,20 @@
             session.run('python', '-m', 'http.server', '8000', '-d', '_build/html')
         else:
             print('Unsupported argument to docs')
 
 
 @nox.session(python='3.7')
 def mypy(session):
-    session.install('mypy')
+    session.install('mypy==0.981')
 
     session.run('mypy', '-p', 'mesonpy')
 
 
-@nox.session(python=['3.7', '3.8', '3.9', '3.10', '3.11'])
+@nox.session(python=['3.7', '3.8', '3.9', '3.10', '3.11', 'pypy3.8', 'pypy3.9'])
 def test(session):
     htmlcov_output = os.path.join(session.virtualenv.location, 'htmlcov')
     xmlcov_output = os.path.join(session.virtualenv.location, f'coverage-{session.python}.xml')
 
     session.install('.[test]')
 
     # optional github actions integration
```

### Comparing `meson_python-0.8.1/pyproject.toml` & `meson_python-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = 'mesonpy'
 backend-path = ['.']
 requires = [
-  'meson>=0.62.0',
+  'meson>=0.63.0',
   'ninja',
   'pyproject-metadata>=0.5.0',
   'tomli>=1.0.0',
   'typing-extensions>=3.7.4; python_version<"3.8"',
 ]
 
 [project]
@@ -40,19 +40,21 @@
 [project.optional-dependencies]
 test = [
   'pytest',
   'pytest-cov',
   'pytest-mock',
   'GitPython',
   'auditwheel',
+  'Cython',
+  'pyproject-metadata>=0.6.1',
 ]
 docs = [
   'furo>=2021.08.31',
   'sphinx~=4.0',
   'sphinx-autodoc-typehints>=1.10',
 ]
 
 [project.urls]
 homepage = 'https://github.com/FFY00/mesonpy'
 repository = 'https://github.com/FFY00/mesonpy'
-documentation = 'https://mesonpy.readthedocs.io'
-changelog = 'https://mesonpy.readthedocs.io/en/latest/changelog.html'
+documentation = 'https://meson-python.readthedocs.io/'
+changelog = 'https://meson-python.readthedocs.io/en/latest/changelog.html'
```

### Comparing `meson_python-0.8.1/tests/conftest.py` & `meson_python-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/packages/full-metadata/pyproject.toml` & `meson_python-0.9.0/tests/packages/full-metadata/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/packages/link-against-local-lib/examplemod.c` & `meson_python-0.9.0/tests/packages/link-against-local-lib/examplemod.c`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/test_metadata.py` & `meson_python-0.9.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/test_output.py` & `meson_python-0.9.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/test_pep517.py` & `meson_python-0.9.0/tests/test_pep517.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/test_project.py` & `meson_python-0.9.0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `meson_python-0.8.1/tests/test_sdist.py` & `meson_python-0.9.0/tests/test_sdist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-License-Identifier: MIT
 
 import os
 import tarfile
 import textwrap
 
+import pytest
+
 import mesonpy
 
 from .conftest import in_git_repo_context
 
 
 def test_contents(sdist_library):
     sdist = tarfile.open(sdist_library, 'r:gz')
@@ -62,7 +64,24 @@
         'pure-1.0.0/PKG-INFO',
         'pure-1.0.0/meson.build',
         'pure-1.0.0/pure.py',
         'pure-1.0.0/pyproject.toml',
     }
     read_data = sdist.extractfile('pure-1.0.0/pure.py').read().replace(b'\r\n', b'\n')
     assert read_data == new_data.encode()
+
+
+@pytest.mark.skipif(os.name == 'nt', reason='Executable bit does not exist on Windows')
+def test_executable_bit(sdist_executable_bit):
+    sdist = tarfile.open(sdist_executable_bit, 'r:gz')
+
+    assert set((tar.name, tar.mode) for tar in sdist.getmembers()) == {
+        ('executable_bit-1.0.0/PKG-INFO', 420),
+        # We match the executable bit on everything
+        # but PKG-INFO(we create this ourselves)
+        # Note: File perms are in octal, but Python returns it in int
+        ('executable_bit-1.0.0/example-script.py', int('755', 8)),
+        ('executable_bit-1.0.0/example.c', int('644', 8)),
+        ('executable_bit-1.0.0/executable_module.py', int('755', 8)),
+        ('executable_bit-1.0.0/meson.build', int('644', 8)),
+        ('executable_bit-1.0.0/pyproject.toml', int('644', 8)),
+    }
```

### Comparing `meson_python-0.8.1/tests/test_tags.py` & `meson_python-0.9.0/tests/test_tags.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,60 +36,40 @@
 
 @pytest.mark.parametrize(
     ('value', 'implementation', 'version', 'additional', 'abi', 'python'),
     [
         ('cpython-37-x86_64-linux-gnu', 'cpython', '37', ('x86_64', 'linux', 'gnu'), 'cp37', 'cp37'),
         ('cpython-310-x86_64-linux-gnu', 'cpython', '310', ('x86_64', 'linux', 'gnu'), 'cp310', 'cp310'),
         ('cpython-310', 'cpython', '310', (), 'cp310', 'cp310'),
+        ('cp311-win_amd64', 'cpython', '311', ('win_amd64', ), 'cp311', 'cp311'),
+        ('cpython-311-win_amd64', 'cpython', '311', ('win_amd64', ), 'cp311', 'cp311'),
         ('cpython-310-special', 'cpython', '310', ('special',), 'cp310', 'cp310'),
-        ('pypy-41', 'pypy', '41', (), 'pypy_41', f'pp{INTERPRETER_VERSION}'),
-        ('pypy3-72-x86_64-linux-gnu', 'pypy3', '72', ('x86_64', 'linux', 'gnu'), 'pypy3_72', f'pp{INTERPRETER_VERSION}'),
         ('cpython-310-x86_64-linux-gnu', 'cpython', '310', ('x86_64', 'linux', 'gnu'), 'cp310', 'cp310'),
+        ('pypy39-pp73-x86_64-linux-gnu', 'pypy39', 'pp73', ('x86_64', 'linux', 'gnu'), 'pypy39_pp73', 'pp39'),
+        ('pypy39-pp73-win_amd64', 'pypy39', 'pp73', ('win_amd64', ), 'pypy39_pp73', 'pp39'),
+        ('pypy38-pp73-darwin', 'pypy38', 'pp73', ('darwin', ), 'pypy38_pp73', 'pp38'),
     ]
 )
-def test_linux_interpreter_tag(value, implementation, version, additional, abi, python):
-    tag = mesonpy._tags.LinuxInterpreterTag(value)
-    assert str(tag) == value
+def test_interpreter_tag(value, implementation, version, additional, abi, python):
+    tag = mesonpy._tags.InterpreterTag(value)
+    if not value.startswith('cp311'):
+        # Avoid testing the workaround for the invalid Windows tag
+        assert str(tag) == value
+
     assert tag.implementation == implementation
     assert tag.interpreter_version == version
     assert tag.additional_information == additional
     assert tag.abi == abi
     assert tag.python == python
-    assert tag == mesonpy._tags.LinuxInterpreterTag(value)
+    assert tag == mesonpy._tags.InterpreterTag(value)
 
 
 @pytest.mark.parametrize(
     ('value', 'msg'),
     [
         ('', 'Invalid PEP 3149 interpreter tag, expected at least 2 parts but got 1'),
         ('invalid', 'Invalid PEP 3149 interpreter tag, expected at least 2 parts but got 1'),
     ]
 )
-def test_linux_interpreter_tag_invalid(value, msg):
+def test_interpreter_tag_invalid(value, msg):
     with pytest.raises(ValueError, match=msg):
-        mesonpy._tags.LinuxInterpreterTag(value)
-
-
-@pytest.mark.parametrize(
-    ('value', 'parts', 'abi', 'python'),
-    [
-        ('cp310-win_amd64', ('cp310', 'win_amd64'), 'cp310', 'cp310'),
-        ('cp38-win32', ('cp38', 'win32'), 'cp38', 'cp38')
-    ]
-)
-def test_windows_interpreter_tag(value, parts, abi, python):
-    tag = mesonpy._tags.WindowsInterpreterTag(value)
-    assert str(tag) == value
-    assert tag.parts == parts
-    assert tag.abi == abi
-    assert tag.python == python
-    assert tag == mesonpy._tags.WindowsInterpreterTag(value)
-
-
-@pytest.mark.parametrize('value', ['', 'unknown', 'too-much-information'])
-def test_windows_interpreter_tag_warn(value):
-    with pytest.warns(Warning, match=(
-        'Unexpected native module tag name, the ABI dectection might be broken. '
-        'Please report this to https://github.com/FFY00/mesonpy/issues '
-        'and include information about the Python distribution you are using.'
-    )):
-        mesonpy._tags.WindowsInterpreterTag(value)
+        mesonpy._tags.InterpreterTag(value)
```

### Comparing `meson_python-0.8.1/PKG-INFO` & `meson_python-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meson-python
-Version: 0.8.1
+Version: 0.9.0
 Summary: Meson Python build backend (PEP 517)
 Keywords: meson build backend pep517 package
 Home-page: https://github.com/FFY00/mesonpy
 Author-Email: Filipe Laíns <lains@riseup.net>
 License: Copyright © 2021 Quansight Labs <flains@quansight.com>
         Copyright © 2021 Filipe Laíns <filipe.lains@gmail.com>
         
@@ -26,28 +26,30 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
         FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
         DEALINGS IN THE SOFTWARE.
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Project-URL: Homepage, https://github.com/FFY00/mesonpy
 Project-URL: Repository, https://github.com/FFY00/mesonpy
-Project-URL: Documentation, https://mesonpy.readthedocs.io
-Project-URL: Changelog, https://mesonpy.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://meson-python.readthedocs.io/
+Project-URL: Changelog, https://meson-python.readthedocs.io/en/latest/changelog.html
 Requires-Python: >=3.7
 Requires-Dist: colorama; os_name == "nt"
 Requires-Dist: meson>=0.62.0
 Requires-Dist: ninja
 Requires-Dist: pyproject-metadata>=0.5.0
 Requires-Dist: tomli>=1.0.0
 Requires-Dist: typing-extensions>=3.7.4; python_version < "3.8"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: GitPython; extra == "test"
 Requires-Dist: auditwheel; extra == "test"
+Requires-Dist: Cython; extra == "test"
+Requires-Dist: pyproject-metadata>=0.6.1; extra == "test"
 Requires-Dist: furo>=2021.08.31; extra == "docs"
 Requires-Dist: sphinx~=4.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints>=1.10; extra == "docs"
 Provides-Extra: test
 Provides-Extra: docs
 Description-Content-Type: text/markdown
```

