# Comparing `tmp/salt-analytics-framework-0.0.1.tar.gz` & `tmp/salt-analytics-framework-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Apr 28 20:46:54 2023, max compression
+gzip compressed data, last modified: Fri Apr 28 21:37:58 2023, max compression
```

## Comparing `salt-analytics-framework-0.0.1.tar` & `salt-analytics-framework-0.1.0.tar`

### file list

```diff
@@ -1,156 +1,157 @@
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.bandit
--rw-r--r--   0 root         (0) root         (0)      684 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/
--rw-r--r--   0 root         (0) root         (0)      229 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/actionlint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/actions/setup-actionlint/
--rw-r--r--   0 root         (0) root         (0)      892 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/actions/setup-actionlint/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     7134 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.github/workflows/test.yml
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     7030 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)    19414 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     3282 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2487 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4244 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3059 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/changelog/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/changelog/_template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6553 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.collect.rst
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.forward.rst
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.process.rst
--rw-r--r--   0 root         (0) root         (0)      861 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.rst
--rw-r--r--   0 root         (0) root         (0)      346 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.saltext.engines.rst
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.saltext.rst
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/ref/saf.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    23743 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     3170 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/collect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/collect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/collect/beacons.py
--rw-r--r--   0 root         (0) root         (0)     5145 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/collect/logs.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/collect/noop.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/collect/salt_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/forward/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/forward/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/forward/disk.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/forward/noop.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/forward/test.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/manager.py
--rw-r--r--   0 root         (0) root         (0)     9649 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/models.py
--rw-r--r--   0 root         (0) root         (0)     5687 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/process/noop.py
--rw-r--r--   0 root         (0) root         (0)     3095 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/process/regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/process/shannon_mask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/saltext/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/saltext/engines/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/utils/dt.py
--rw-r--r--   0 root         (0) root         (0)     5726 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/utils/eventbus.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/saf/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4244 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3543 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      584 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/forwarders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/forwarders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/forwarders/test_concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/manager/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/manager/test_disabled_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/functional/manager/test_enabled_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/test_memusage.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/test_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/test_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/logs/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/logs/test_logs.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/logs/test_logs_with_parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/test_arg.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/test_collatz.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/test_config_get.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/integration/engines/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/process/test_regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     5436 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/process/test_shannon_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/salt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/salt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/salt/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tests/unit/salt/engines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tools/
--rw-r--r--   0 root         (0) root         (0)      290 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tools/pre_commit.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-28 20:46:54.000000 salt-analytics-framework-0.0.1/tools/pre_commit.py~
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.bandit
+-rw-r--r--   0 root         (0) root         (0)      684 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actionlint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      995 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     7134 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     7030 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)    19414 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/changelog/_template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.collect.rst
+-rw-r--r--   0 root         (0) root         (0)      557 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.forward.rst
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.process.rst
+-rw-r--r--   0 root         (0) root         (0)      861 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.rst
+-rw-r--r--   0 root         (0) root         (0)      346 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.saltext.engines.rst
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/ref/saf.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    23817 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/beacons.py
+-rw-r--r--   0 root         (0) root         (0)     5145 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/logs.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/collect/salt_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/disk.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/forward/test.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9649 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/models.py
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/noop.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/process/shannon_mask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/saltext/engines/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/dt.py
+-rw-r--r--   0 root         (0) root         (0)     5726 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/utils/eventbus.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/saf/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/forwarders/test_concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/test_disabled_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/functional/manager/test_enabled_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_memusage.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs_with_parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_collatz.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_config_get.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/integration/engines/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/test_regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/process/test_shannon_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tests/unit/salt/engines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/pre_commit.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-04-28 21:37:58.000000 salt-analytics-framework-0.1.0/tools/pre_commit.py~
```

### Comparing `salt-analytics-framework-0.0.1/.coveragerc` & `salt-analytics-framework-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.github/actions/setup-actionlint/action.yml` & `salt-analytics-framework-0.1.0/.github/actions/setup-actionlint/action.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.github/workflows/test.yml` & `salt-analytics-framework-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.gitignore` & `salt-analytics-framework-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pre-commit-config.yaml` & `salt-analytics-framework-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pre-commit-hooks/check-changelog-entries.py` & `salt-analytics-framework-0.1.0/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pre-commit-hooks/check-cli-examples.py` & `salt-analytics-framework-0.1.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pre-commit-hooks/copyright-headers.py` & `salt-analytics-framework-0.1.0/.pre-commit-hooks/copyright-headers.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pre-commit-hooks/make-autodocs.py` & `salt-analytics-framework-0.1.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pre-commit-hooks/sort-pylint-spelling-words.py` & `salt-analytics-framework-0.1.0/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pylint-spelling-words` & `salt-analytics-framework-0.1.0/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/.pylintrc` & `salt-analytics-framework-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/CODE_OF_CONDUCT.md` & `salt-analytics-framework-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/CONTRIBUTING.md` & `salt-analytics-framework-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/LICENSE` & `salt-analytics-framework-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/NOTICE` & `salt-analytics-framework-0.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/PKG-INFO` & `salt-analytics-framework-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.0.1
+Version: 0.1.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
@@ -27,48 +27,14 @@
 Provides-Extra: docs
 Provides-Extra: docsauto
 Provides-Extra: changelog
 Provides-Extra: build
 License-File: LICENSE
 License-File: NOTICE
 
-.. image:: https://img.shields.io/github/workflow/status/saltstack/salt-analytics-framework/CI?style=plastic
-   :target: https://github.com/saltstack/salt-analytics-framework/actions/workflows/testing.yml
-   :alt: CI
-
-
-.. image:: https://readthedocs.org/projects/salt-analytics-framework/badge/?style=plastic
-   :target: https://salt-analytics-framework.readthedocs.io
-   :alt: Docs
-
-
-.. image:: https://img.shields.io/codecov/c/github/saltstack/salt-analytics-framework?style=plastic&token=CqV7t0yKTb
-   :target: https://codecov.io/gh/saltstack/salt-analytics-framework
-   :alt: Codecov
-
-
-.. image:: https://img.shields.io/pypi/pyversions/salt-analytics-framework?style=plastic
-   :target: https://pypi.org/project/salt-analytics-framework
-   :alt: Python Versions
-
-
-.. image:: https://img.shields.io/pypi/wheel/salt-analytics-framework?style=plastic
-   :target: https://pypi.org/project/salt-analytics-framework
-   :alt: Python Wheel
-
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=plastic
-   :target: https://github.com/psf/black
-   :alt: Code Style: black
-
-
-.. image:: https://img.shields.io/pypi/l/salt-analytics-framework?style=plastic
-   :alt: PyPI - License
-
-
 ..
    include-starts-here
 
 ================================
 What is Salt Analytics Framework
 ================================
```

### Comparing `salt-analytics-framework-0.0.1/changelog/_template.rst` & `salt-analytics-framework-0.1.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/Makefile` & `salt-analytics-framework-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/conf.py` & `salt-analytics-framework-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/index.rst` & `salt-analytics-framework-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/make.bat` & `salt-analytics-framework-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/ref/saf.collect.rst` & `salt-analytics-framework-0.1.0/docs/ref/saf.collect.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/ref/saf.forward.rst` & `salt-analytics-framework-0.1.0/docs/ref/saf.forward.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/ref/saf.process.rst` & `salt-analytics-framework-0.1.0/docs/ref/saf.process.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/docs/ref/saf.rst` & `salt-analytics-framework-0.1.0/docs/ref/saf.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/noxfile.py` & `salt-analytics-framework-0.1.0/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,22 +565,26 @@
         install_coverage_requirements=False,
         install_test_requirements=False,
         install_source=False,
         install_salt=False,
         install_extras=["changelog"],
     )
 
-    version = session.run(
-        "python",
-        "setup.py",
-        "--version",
-        silent=True,
-        log=False,
-        stderr=None,
-    ).strip()
+    version = (
+        session.run(
+            "python",
+            "setup.py",
+            "--version",
+            silent=True,
+            log=False,
+            stderr=None,
+        )
+        .strip()
+        .split()[-1]
+    )
 
     town_cmd = ["towncrier", "build", f"--version={version}"]
     if draft:
         town_cmd.append("--draft")
     session.run(*town_cmd)
```

### Comparing `salt-analytics-framework-0.0.1/pyproject.toml` & `salt-analytics-framework-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/setup.cfg` & `salt-analytics-framework-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/__init__.py` & `salt-analytics-framework-0.1.0/src/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/collect/beacons.py` & `salt-analytics-framework-0.1.0/src/saf/collect/beacons.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/collect/logs.py` & `salt-analytics-framework-0.1.0/src/saf/collect/logs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/collect/noop.py` & `salt-analytics-framework-0.1.0/src/saf/collect/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/collect/salt_exec.py` & `salt-analytics-framework-0.1.0/src/saf/collect/salt_exec.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/forward/disk.py` & `salt-analytics-framework-0.1.0/src/saf/forward/disk.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/forward/noop.py` & `salt-analytics-framework-0.1.0/src/saf/forward/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/forward/test.py` & `salt-analytics-framework-0.1.0/src/saf/forward/test.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/manager.py` & `salt-analytics-framework-0.1.0/src/saf/manager.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/models.py` & `salt-analytics-framework-0.1.0/src/saf/models.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/pipeline.py` & `salt-analytics-framework-0.1.0/src/saf/pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/plugins.py` & `salt-analytics-framework-0.1.0/src/saf/plugins.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/process/noop.py` & `salt-analytics-framework-0.1.0/src/saf/process/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/process/regex_mask.py` & `salt-analytics-framework-0.1.0/src/saf/process/regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/process/shannon_mask.py` & `salt-analytics-framework-0.1.0/src/saf/process/shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/saltext/engines/analytics.py` & `salt-analytics-framework-0.1.0/src/saf/saltext/engines/analytics.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/saf/utils/eventbus.py` & `salt-analytics-framework-0.1.0/src/saf/utils/eventbus.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/PKG-INFO` & `salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.0.1
+Version: 0.1.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
@@ -27,48 +27,14 @@
 Provides-Extra: docs
 Provides-Extra: docsauto
 Provides-Extra: changelog
 Provides-Extra: build
 License-File: LICENSE
 License-File: NOTICE
 
-.. image:: https://img.shields.io/github/workflow/status/saltstack/salt-analytics-framework/CI?style=plastic
-   :target: https://github.com/saltstack/salt-analytics-framework/actions/workflows/testing.yml
-   :alt: CI
-
-
-.. image:: https://readthedocs.org/projects/salt-analytics-framework/badge/?style=plastic
-   :target: https://salt-analytics-framework.readthedocs.io
-   :alt: Docs
-
-
-.. image:: https://img.shields.io/codecov/c/github/saltstack/salt-analytics-framework?style=plastic&token=CqV7t0yKTb
-   :target: https://codecov.io/gh/saltstack/salt-analytics-framework
-   :alt: Codecov
-
-
-.. image:: https://img.shields.io/pypi/pyversions/salt-analytics-framework?style=plastic
-   :target: https://pypi.org/project/salt-analytics-framework
-   :alt: Python Versions
-
-
-.. image:: https://img.shields.io/pypi/wheel/salt-analytics-framework?style=plastic
-   :target: https://pypi.org/project/salt-analytics-framework
-   :alt: Python Wheel
-
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=plastic
-   :target: https://github.com/psf/black
-   :alt: Code Style: black
-
-
-.. image:: https://img.shields.io/pypi/l/salt-analytics-framework?style=plastic
-   :alt: PyPI - License
-
-
 ..
    include-starts-here
 
 ================================
 What is Salt Analytics Framework
 ================================
```

### Comparing `salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/SOURCES.txt` & `salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 noxfile.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 .github/actionlint.yaml
 .github/actions/setup-actionlint/action.yml
+.github/workflows/release.yml
 .github/workflows/test.yml
 .pre-commit-hooks/check-changelog-entries.py
 .pre-commit-hooks/check-cli-examples.py
 .pre-commit-hooks/copyright-headers.py
 .pre-commit-hooks/make-autodocs.py
 .pre-commit-hooks/sort-pylint-spelling-words.py
 changelog/_template.rst
```

### Comparing `salt-analytics-framework-0.0.1/src/salt_analytics_framework.egg-info/requires.txt` & `salt-analytics-framework-0.1.0/src/salt_analytics_framework.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/conftest.py` & `salt-analytics-framework-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/functional/conftest.py` & `salt-analytics-framework-0.1.0/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/functional/forwarders/test_concurrency.py` & `salt-analytics-framework-0.1.0/tests/functional/forwarders/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/functional/manager/conftest.py` & `salt-analytics-framework-0.1.0/tests/functional/manager/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/functional/manager/test_disabled_pipeline.py` & `salt-analytics-framework-0.1.0/tests/functional/manager/test_disabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/functional/manager/test_enabled_pipeline.py` & `salt-analytics-framework-0.1.0/tests/functional/manager/test_enabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/test_memusage.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_memusage.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/test_multiple.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_multiple.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/beacons/test_status.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/beacons/test_status.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/logs/conftest.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/logs/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/logs/test_logs.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/logs/test_logs_with_parse.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/logs/test_logs_with_parse.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/conftest.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/test_arg.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_arg.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/test_collatz.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_collatz.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/collectors/salt_exec/test_config_get.py` & `salt-analytics-framework-0.1.0/tests/integration/collectors/salt_exec/test_config_get.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/conftest.py` & `salt-analytics-framework-0.1.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/integration/engines/test_engine.py` & `salt-analytics-framework-0.1.0/tests/integration/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/unit/process/test_regex_mask.py` & `salt-analytics-framework-0.1.0/tests/unit/process/test_regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tests/unit/process/test_shannon_mask.py` & `salt-analytics-framework-0.1.0/tests/unit/process/test_shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tools/pre_commit.py` & `salt-analytics-framework-0.1.0/tools/pre_commit.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.0.1/tools/pre_commit.py~` & `salt-analytics-framework-0.1.0/tools/pre_commit.py~`

 * *Files identical despite different names*

