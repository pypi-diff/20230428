# Comparing `tmp/ansible-compat-3.0.2.tar.gz` & `tmp/ansible-compat-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-3.0.2.tar", last modified: Thu Apr 13 17:14:09 2023, max compression
+gzip compressed data, was "ansible-compat-4.0.0.tar", last modified: Fri Apr 28 13:57:26 2023, max compression
```

## Comparing `ansible-compat-3.0.2.tar` & `ansible-compat-4.0.0.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.272825 ansible-compat-3.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.264825 ansible-compat-3.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.276825 ansible-compat-3.0.2/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.264825 ansible-compat-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.280825 ansible-compat-3.0.2/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27606 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/src/ansible_compat/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.280825 ansible-compat-3.0.2/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 17:14:09.000000 ansible-compat-3.0.2/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.284825 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/collections/acme.goodies/roles/baz/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.268825 ansible-compat-3.0.2/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:14:09.288825 ansible-compat-3.0.2/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-13 17:13:53.000000 ansible-compat-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.183455 ansible-compat-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.187455 ansible-compat-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.187455 ansible-compat-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.191455 ansible-compat-4.0.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.191455 ansible-compat-4.0.0/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.191455 ansible-compat-4.0.0/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.195455 ansible-compat-4.0.0/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28295 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.195455 ansible-compat-4.0.0/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.199455 ansible-compat-4.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.179455 ansible-compat-4.0.0/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/tox.ini
```

### Comparing `ansible-compat-3.0.2/.github/dependabot.yml` & `ansible-compat-4.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/.github/workflows/release.yml` & `ansible-compat-4.0.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     steps:
       - name: Switch to using Python 3.9 by default
         uses: actions/setup-python@v4
         with:
           python-version: 3.9
       - name: Install tox
-        run: python3 -m pip install --user "tox>=4.0.0rc1"
+        run: python3 -m pip install --user "tox>=4.0.0"
       - name: Check out src from Git
         uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
       - name: Build dists
         run: python -m tox -e pkg
       - name: Publish to pypi.org
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@unstable/v1
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `ansible-compat-3.0.2/.github/workflows/tox.yml` & `ansible-compat-4.0.0/.github/workflows/tox.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,22 @@
     outputs:
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
     steps:
       - name: Determine matrix
         id: generate_matrix
         uses: coactions/dynamic-matrix@v1
         with:
+          min_python: "3.9"
           max_python: "3.11"
           other_names: |
             lint
             docs
             pkg
-            py38-ansible212
-            py38-ansible213
+            py39-ansible212
+            py39-ansible213
             py39-ansible214
             py311-devel
           platforms: linux,macos
           macos: minmax
   build:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os || 'ubuntu-22.04' }}
```

### Comparing `ansible-compat-3.0.2/.gitignore` & `ansible-compat-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/.pre-commit-config.yaml` & `ansible-compat-4.0.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -67,25 +67,14 @@
           # https://github.com/pre-commit/mirrors-isort/issues/9#issuecomment-624404082
           - --filter-files
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
-  - repo: https://github.com/pycqa/flake8.git
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        language_version: python3
-        additional_dependencies:
-          - flake8-2020>=1.6.0
-          - flake8-docstrings>=1.5.0
-          - flake8-pytest-style>=1.2.2
-          - flake8-rst-docstrings>=0.2.3
-          - flake8-rst>=0.8.0
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.1.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: ["--strict"]
         additional_dependencies:
@@ -110,21 +99,21 @@
   - repo: local
     hooks:
       - id: pip-compile-upgrade
         # To run it execute: `pre-commit run pip-compile-upgrade --hook-stage manual`
         name: Upgrade constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
-        entry: python -m piptools compile --resolver=backtracking --upgrade -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core
+        entry: python -m piptools compile --resolver=backtracking --upgrade -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib
         pass_filenames: false
         stages:
           - manual
         additional_dependencies:
           - pip-tools>=6.11.0
       - id: pip-compile
         name: Check constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
-        entry: python -m piptools compile --resolver=backtracking -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core
+        entry: python -m piptools compile --resolver=backtracking -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib
         pass_filenames: false
         additional_dependencies:
           - pip-tools>=6.11.0
```

### Comparing `ansible-compat-3.0.2/.readthedocs.yml` & `ansible-compat-4.0.0/.readthedocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 build:
   image: latest
 
 # Optionally set the version of Python and requirements required
 # to build docs
 python:
-  version: "3.8"
+  version: "3.9"
   install:
     # On https://readthedocs.org/dashboard/ansible-lint/environmentvariables/ we
     # do have PIP_CONSTRAINTS=requirements.txt which ensures we install only
     # pinned requirements that that we know to be working.
     - method: pip
       path: .
       extra_requirements:
```

### Comparing `ansible-compat-3.0.2/LICENSE` & `ansible-compat-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/PKG-INFO` & `ansible-compat-4.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 3.0.2
+Version: 4.0.0
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
@@ -14,25 +14,24 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # ansible-compat
```

### Comparing `ansible-compat-3.0.2/README.md` & `ansible-compat-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/docs/images/favicon.ico` & `ansible-compat-4.0.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/docs/images/logo.png` & `ansible-compat-4.0.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/docs/images/logo.svg` & `ansible-compat-4.0.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.0.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/mkdocs.yml` & `ansible-compat-4.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/pyproject.toml` & `ansible-compat-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools >= 61.0", # PEP-621
   "setuptools_scm[toml] >= 7.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dynamic = ["version"]
 name = "ansible-compat"
 description = "Ansible compatibility goodies"
 readme = "README.md"
 authors = [{ "name" = "Sorin Sbarnea", "email" = "ssbarnea@redhat.com" }]
 maintainers = [{ "name" = "Sorin Sbarnea", "email" = "ssbarnea@redhat.com" }]
 license = { text = "MIT" }
@@ -20,15 +20,14 @@
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python",
   "Topic :: System :: Systems Administration",
   "Topic :: Software Development :: Bug Tracking",
   "Topic :: Software Development :: Quality Assurance",
@@ -62,15 +61,15 @@
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
 fail_under = 93
 skip_covered = true
 show_missing = true
 
 [tool.mypy]
-python_version = 3.8
+python_version = 3.9
 color_output = true
 error_summary = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_any_generics = true
 # disallow_any_unimported = True
 #; warn_redundant_casts = True
```

### Comparing `ansible-compat-3.0.2/requirements.txt` & `ansible-compat-4.0.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=docs --extra=test --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core pyproject.toml
+#    pip-compile --extra=docs --extra=test --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core --unsafe-package=resolvelib pyproject.toml
 #
-argparse-manpage==4
+argparse-manpage==4.1
     # via ansible-compat (pyproject.toml)
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 beautifulsoup4==4.12.1
     # via
     #   mkdocs-ansible
     #   mkdocs-htmlproofer-plugin
 black==23.3.0
     # via ansible-compat (pyproject.toml)
@@ -42,17 +42,17 @@
     #   mkdocs-ansible
     #   pip-tools
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-ansible
     #   mkdocs-material
-coverage==7.2.3
+coverage==7.2.4
     # via ansible-compat (pyproject.toml)
-cryptography==40.0.1
+cryptography==40.0.2
     # via ansible-core
 csscompressor==0.9.5
     # via
     #   mkdocs-ansible
     #   mkdocs-minify-plugin
 cssselect2==0.7.0
     # via
@@ -172,21 +172,21 @@
     #   pytest
 pathspec==0.11.1
     # via black
 pillow==9.5.0
     # via
     #   cairosvg
     #   mkdocs-ansible
-pip==23.0.1
+pip==23.1.2
     # via pip-tools
 pip-tools==6.13.0
     # via ansible-compat (pyproject.toml)
 pipdeptree==2.7.0
     # via mkdocs-ansible
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via black
 pluggy==1.0.0
     # via pytest
 pycparser==2.21
     # via
     #   cffi
     #   mkdocs-ansible
@@ -200,15 +200,15 @@
     #   mkdocs-ansible
     #   mkdocs-material
     #   mkdocstrings
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.0
+pytest==7.3.1
     # via
     #   ansible-compat (pyproject.toml)
     #   pytest-mock
     #   pytest-plus
 pytest-mock==3.10.0
     # via ansible-compat (pyproject.toml)
 pytest-plus==0.4.0
@@ -238,17 +238,15 @@
     #   mkdocs-ansible
     #   mkdocs-material
 requests==2.28.2
     # via
     #   mkdocs-ansible
     #   mkdocs-htmlproofer-plugin
     #   mkdocs-material
-resolvelib==0.8.1
-    # via ansible-core
-setuptools==67.6.1
+setuptools==67.7.2
     # via pip-tools
 six==1.16.0
     # via
     #   mkdocs-ansible
     #   python-dateutil
 soupsieve==2.4
     # via
@@ -294,7 +292,8 @@
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   mkdocs-ansible
 
 # The following packages are considered to be unsafe in a requirements file:
 # ansible-core
+# resolvelib
```

### Comparing `ansible-compat-3.0.2/src/ansible_compat/config.py` & `ansible-compat-4.0.0/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/src/ansible_compat/constants.py` & `ansible-compat-4.0.0/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/src/ansible_compat/errors.py` & `ansible-compat-4.0.0/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/src/ansible_compat/loaders.py` & `ansible-compat-4.0.0/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/src/ansible_compat/prerun.py` & `ansible-compat-4.0.0/src/ansible_compat/prerun.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Utilities for configuring ansible runtime environment."""
 import hashlib
 import os
+from pathlib import Path
 
 
-def get_cache_dir(project_dir: str) -> str:
+def get_cache_dir(project_dir: str) -> Path:
     """Compute cache directory to be used based on project path."""
     # we only use the basename instead of the full path in order to ensure that
     # we would use the same key regardless the location of the user home
     # directory or where the project is clones (as long the project folder uses
     # the same name).
     basename = os.path.basename(os.path.abspath(project_dir)).encode(encoding="utf-8")
     # 6 chars of entropy should be enough
     cache_key = hashlib.sha256(basename).hexdigest()[:6]
     cache_dir = (
         os.getenv("XDG_CACHE_HOME", os.path.expanduser("~/.cache"))
         + "/ansible-compat/"
         + cache_key
     )
-    return cache_dir
+    return Path(cache_dir)
```

### Comparing `ansible-compat-3.0.2/src/ansible_compat/runtime.py` & `ansible-compat-4.0.0/src/ansible_compat/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Ansible runtime environment manager."""
+import contextlib
 import importlib
 import json
 import logging
 import os
 import pathlib
 import re
 import shutil
 import subprocess
 import tempfile
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
+import warnings
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import packaging
 import subprocess_tee
 from packaging.version import Version
 
 from ansible_compat.config import (
     AnsibleConfig,
@@ -37,32 +39,36 @@
     CompletedProcess = subprocess.CompletedProcess
 
 _logger = logging.getLogger(__name__)
 # regex to extract the first version from a collection range specifier
 version_re = re.compile(":[>=<]*([^,]*)")
 
 
+class AnsibleWarning(Warning):
+    """Warnings related to Ansible runtime."""
+
+
 class Runtime:
     """Ansible Runtime manager."""
 
     _version: Optional[packaging.version.Version] = None
-    cache_dir: Optional[str] = None
+    cache_dir: Optional[pathlib.Path] = None
     # Used to track if we have already initialized the Ansible runtime as attempts
     # to do it multiple tilmes will cause runtime warnings from within ansible-core
     initialized: bool = False
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         project_dir: Optional[str] = None,
         isolated: bool = False,
         min_required_version: Optional[str] = None,
         require_module: bool = False,
         max_retries: int = 0,
-        environ: Optional[Dict[str, str]] = None,
+        environ: Optional[dict[str, str]] = None,
     ) -> None:
         """Initialize Ansible runtime environment.
 
         :param project_dir: The directory containing the Ansible project. If
                             not mentioned it will be guessed from the current
                             working directory.
         :param isolated: Assure that installation of collections or roles
@@ -96,43 +102,52 @@
 
         if isolated:
             self.cache_dir = get_cache_dir(self.project_dir)
         self.config = AnsibleConfig()
 
         if not self.version_in_range(lower=min_required_version):
             raise RuntimeError(
-                f"Found incompatible version of ansible runtime {self.version}, instead of {min_required_version} or newer."
+                f"Found incompatible version of ansible runtime {self.version}, instead of {min_required_version} or newer.",
             )
         if require_module:
             self._ensure_module_available()
 
+        # pylint: disable=import-outside-toplevel
+        from ansible.utils.display import Display
+
+        # pylint: disable=unused-argument
+        def warning(self: Display, msg: str, formatted: bool = False) -> None:
+            """Override ansible.utils.display.Display.warning to avoid printing warnings."""
+            warnings.warn(msg, category=AnsibleWarning, stacklevel=2)
+
+        # Monkey patch ansible warning in order to use warnings module.
+        Display.warning = warning
+
     def _ensure_module_available(self) -> None:
         """Assure that Ansible Python module is installed and matching CLI version."""
         ansible_release_module = None
-        try:
+        with contextlib.suppress(ModuleNotFoundError, ImportError):
             ansible_release_module = importlib.import_module("ansible.release")
-        except (ModuleNotFoundError, ImportError):
-            pass
 
         if ansible_release_module is None:
             raise RuntimeError("Unable to find Ansible python module.")
 
         ansible_module_version = packaging.version.parse(
-            ansible_release_module.__version__
+            ansible_release_module.__version__,
         )
         if ansible_module_version != self.version:
             raise RuntimeError(
                 f"Ansible CLI ({self.version}) and python module"
                 f" ({ansible_module_version}) versions do not match. This "
-                "indicates a broken execution environment."
+                "indicates a broken execution environment.",
             )
 
         # For ansible 2.15+ we need to initialize the plugin loader
         # https://github.com/ansible/ansible-lint/issues/2945
-        if not Runtime.initialized:  # noqa: F823
+        if not Runtime.initialized:
             col_path = [f"{self.cache_dir}/collections"]
             if self.version >= Version("2.15.0.dev0"):
                 # pylint: disable=import-outside-toplevel,no-name-in-module
                 from ansible.plugins.loader import init_plugin_loader
 
                 init_plugin_loader(col_path)
             else:
@@ -141,32 +156,32 @@
                     _AnsibleCollectionFinder,
                 )
 
                 # noinspection PyProtectedMember
                 # pylint: disable=protected-access
                 col_path += self.config.collections_paths
                 col_path += os.path.dirname(
-                    os.environ.get(ansible_collections_path(), ".")
+                    os.environ.get(ansible_collections_path(), "."),
                 ).split(":")
                 _AnsibleCollectionFinder(
-                    paths=col_path
+                    paths=col_path,
                 )._install()  # pylint: disable=protected-access
             Runtime.initialized = True
 
     def clean(self) -> None:
         """Remove content of cache_dir."""
         if self.cache_dir:
             shutil.rmtree(self.cache_dir, ignore_errors=True)
 
     def exec(
         self,
-        args: Union[str, List[str]],
+        args: Union[str, list[str]],
         retry: bool = False,
         tee: bool = False,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[dict[str, str]] = None,
         cwd: Optional[str] = None,
     ) -> CompletedProcess:
         """Execute a command inside an Ansible environment.
 
         :param retry: Retry network operations on failures.
         :param tee: Also pass captured stdout/stderr to system while running.
         """
@@ -211,15 +226,17 @@
             self._version = parse_ansible_version(proc.stdout)
             return self._version
 
         msg = "Unable to find a working copy of ansible executable."
         raise MissingAnsibleError(msg, proc=proc)
 
     def version_in_range(
-        self, lower: Optional[str] = None, upper: Optional[str] = None
+        self,
+        lower: Optional[str] = None,
+        upper: Optional[str] = None,
     ) -> bool:
         """Check if Ansible version is inside a required range.
 
         The lower limit is inclusive and the upper one exclusive.
         """
         if lower and self.version < packaging.version.Version(lower):
             return False
@@ -249,15 +266,15 @@
         # As ansible-galaxy install is not able to automatically determine
         # if the range requires a pre-release, we need to manuall add the --pre
         # flag when needed.
         matches = version_re.search(collection)
         if matches and Version(matches[1]).is_prerelease:
             cmd.append("--pre")
 
-        cpaths: List[str] = self.config.collections_paths
+        cpaths: list[str] = self.config.collections_paths
         if destination and str(destination) not in cpaths:
             # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
             # we hack ansible_collections_path instead and inject our own path there.
             # pylint: disable=no-member
             cpaths.insert(0, str(destination))
         cmd.append(f"{collection}")
 
@@ -269,15 +286,17 @@
         )
         if run.returncode != 0:
             msg = f"Command returned {run.returncode} code:\n{run.stdout}\n{run.stderr}"
             _logger.error(msg)
             raise InvalidPrerequisiteError(msg)
 
     def install_collection_from_disk(
-        self, path: str, destination: Optional[Union[str, pathlib.Path]] = None
+        self,
+        path: str,
+        destination: Optional[Union[str, pathlib.Path]] = None,
     ) -> None:
         """Build and install collection from a given disk path."""
         if not self.version_in_range(upper="2.11"):
             self.install_collection(path, destination=destination, force=True)
             return
         # older versions of ansible able unable to install without building
         with tempfile.TemporaryDirectory() as tmp_dir:
@@ -299,28 +318,31 @@
                     os.path.join(tmp_dir, archive_file),
                     destination=destination,
                     force=True,
                 )
 
     # pylint: disable=too-many-branches
     def install_requirements(
-        self, requirement: str, retry: bool = False, offline: bool = False
+        self,
+        requirement: str,
+        retry: bool = False,
+        offline: bool = False,
     ) -> None:
         """Install dependencies from a requirements.yml.
 
         :param requirement: path to requirements.yml file
         :param retry: retry network operations on failures
         :param offline: bypass installation, may fail if requirements are not met.
         """
         if not os.path.exists(requirement):
             return
         reqs_yaml = yaml_from_file(requirement)
         if not isinstance(reqs_yaml, (dict, list)):
             raise InvalidPrerequisiteError(
-                f"{requirement} file is not a valid Ansible requirements file."
+                f"{requirement} file is not a valid Ansible requirements file.",
             )
 
         if isinstance(reqs_yaml, list) or "roles" in reqs_yaml:
             cmd = [
                 "ansible-galaxy",
                 "role",
                 "install",
@@ -328,15 +350,15 @@
                 f"{requirement}",
             ]
             if self.cache_dir:
                 cmd.extend(["--roles-path", f"{self.cache_dir}/roles"])
 
             if offline:
                 _logger.warning(
-                    "Skipped installing old role dependencies due to running in offline mode."
+                    "Skipped installing old role dependencies due to running in offline mode.",
                 )
             else:
                 _logger.info("Running %s", " ".join(cmd))
 
                 result = self.exec(cmd, retry=retry)
                 if result.returncode != 0:
                     _logger.error(result.stdout)
@@ -348,15 +370,15 @@
                 "ansible-galaxy",
                 "collection",
                 "install",
                 "-v",
             ]
             if offline:
                 _logger.warning(
-                    "Skipped installing collection dependencies due to running in offline mode."
+                    "Skipped installing collection dependencies due to running in offline mode.",
                 )
             else:
                 cmd.extend(["-r", requirement])
                 cpaths = self.config.collections_paths
                 if self.cache_dir:
                     # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
                     # we hack ansible_collections_path instead and inject our own path there.
@@ -371,17 +393,17 @@
                     env={**os.environ, "ANSIBLE_COLLECTIONS_PATH": ":".join(cpaths)},
                 )
                 if result.returncode != 0:
                     _logger.error(result.stdout)
                     _logger.error(result.stderr)
                     raise AnsibleCommandError(result)
 
-    def prepare_environment(  # noqa: C901
+    def prepare_environment(
         self,
-        required_collections: Optional[Dict[str, str]] = None,
+        required_collections: Optional[dict[str, str]] = None,
         retry: bool = False,
         install_local: bool = False,
         offline: bool = False,
         role_name_check: int = 0,
     ) -> None:
         """Make dependencies available if needed."""
         if required_collections is None:
@@ -413,82 +435,84 @@
         if os.path.exists("galaxy.yml"):
             if destination:
                 # while function can return None, that would not break the logic
                 colpath = f"{destination}/ansible_collections/{colpath_from_path(os.getcwd())}"
                 if os.path.islink(colpath):
                     if os.path.realpath(colpath) == os.getcwd():
                         _logger.warning(
-                            "Found symlinked collection, skipping its installation."
+                            "Found symlinked collection, skipping its installation.",
                         )
                         return
                     _logger.warning(
                         "Collection is symlinked, but not pointing to %s directory, so we will remove it.",
                         os.getcwd(),
                     )
                     os.unlink(colpath)
 
             # molecule scenario within a collection
             self.install_collection_from_disk(".", destination=destination)
         elif pathlib.Path().resolve().parent.name == "roles" and os.path.exists(
-            "../../galaxy.yml"
+            "../../galaxy.yml",
         ):
             # molecule scenario located within roles/<role-name>/molecule inside
             # a collection
             self.install_collection_from_disk("../..", destination=destination)
         else:
             # no collection, try to recognize and install a standalone role
             self._install_galaxy_role(
-                self.project_dir, role_name_check=role_name_check, ignore_errors=True
+                self.project_dir,
+                role_name_check=role_name_check,
+                ignore_errors=True,
             )
 
-    def require_collection(  # noqa: C901
+    def require_collection(
         self,
         name: str,
         version: Optional[str] = None,
         install: bool = True,
     ) -> None:
         """Check if a minimal collection version is present or exits.
 
         In the future this method may attempt to install a missing or outdated
         collection before failing.
         """
         try:
             ns, coll = name.split(".", 1)
         except ValueError as exc:
             raise InvalidPrerequisiteError(
-                f"Invalid collection name supplied: {name}%s"
+                f"Invalid collection name supplied: {name}%s",
             ) from exc
 
-        paths: List[str] = self.config.collections_paths
+        paths: list[str] = self.config.collections_paths
         if not paths or not isinstance(paths, list):
             raise InvalidPrerequisiteError(
-                f"Unable to determine ansible collection paths. ({paths})"
+                f"Unable to determine ansible collection paths. ({paths})",
             )
 
         if self.cache_dir:
             # if we have a cache dir, we want to be use that would be preferred
             # destination when installing a missing collection
             # https://github.com/PyCQA/pylint/issues/4667
             paths.insert(0, f"{self.cache_dir}/collections")  # pylint: disable=E1101
 
         for path in paths:
             collpath = os.path.expanduser(
-                os.path.join(path, "ansible_collections", ns, coll)
+                os.path.join(path, "ansible_collections", ns, coll),
             )
             if os.path.exists(collpath):
                 mpath = os.path.join(collpath, "MANIFEST.json")
                 if not os.path.exists(mpath):
                     msg = f"Found collection at '{collpath}' but missing MANIFEST.json, cannot get info."
                     _logger.fatal(msg)
                     raise InvalidPrerequisiteError(msg)
 
-                with open(mpath, "r", encoding="utf-8") as f:
+                with open(mpath, encoding="utf-8") as f:
                     manifest = json.loads(f.read())
                     found_version = packaging.version.parse(
-                        manifest["collection_info"]["version"]
+                        manifest["collection_info"]["version"],
                     )
                     if version and found_version < packaging.version.parse(version):
                         if install:
                             self.install_collection(f"{name}:>={version}")
                             self.require_collection(name, version, install=False)
                         else:
                             msg = f"Found {name} collection {found_version} but {version} or newer is required."
@@ -503,17 +527,17 @@
                 msg = f"Collection '{name}' not found in '{paths}'"
                 _logger.fatal(msg)
                 raise InvalidPrerequisiteError(msg)
 
     def _prepare_ansible_paths(self) -> None:
         """Configure Ansible environment variables."""
         try:
-            library_paths: List[str] = self.config.default_module_path.copy()
-            roles_path: List[str] = self.config.default_roles_path.copy()
-            collections_path: List[str] = self.config.collections_paths.copy()
+            library_paths: list[str] = self.config.default_module_path.copy()
+            roles_path: list[str] = self.config.default_roles_path.copy()
+            collections_path: list[str] = self.config.collections_paths.copy()
         except AttributeError as exc:
             raise RuntimeError("Unexpected ansible configuration") from exc
 
         alterations_list = [
             (library_paths, "plugins/modules", True),
             (roles_path, "roles", True),
         ]
@@ -521,15 +545,15 @@
         alterations_list.extend(
             [
                 (roles_path, f"{self.cache_dir}/roles", False),
                 (library_paths, f"{self.cache_dir}/modules", False),
                 (collections_path, f"{self.cache_dir}/collections", False),
             ]
             if self.isolated
-            else []
+            else [],
         )
 
         for path_list, path, must_be_present in alterations_list:
             if not os.path.exists(path):
                 if must_be_present:
                     continue
                 os.makedirs(path, exist_ok=True)
@@ -554,15 +578,18 @@
         if self.cache_dir:
             path = pathlib.Path(f"{self.cache_dir}/roles")
         else:
             path = pathlib.Path(os.path.expanduser(self.config.default_roles_path[0]))
         return path
 
     def _install_galaxy_role(
-        self, project_dir: str, role_name_check: int = 0, ignore_errors: bool = False
+        self,
+        project_dir: str,
+        role_name_check: int = 0,
+        ignore_errors: bool = False,
     ) -> None:
         """Detect standalone galaxy role and installs it.
 
         :param: role_name_check: logic to used to check role name
             0: exit with error if name is not compliant (default)
             1: warn if name is not compliant
             2: bypass any name checking
@@ -620,15 +647,15 @@
             # https://github.com/python/cpython/issues/73843
             link_path.symlink_to(str(target), target_is_directory=True)
         _logger.info(
             "Using %s symlink to current repository in order to enable Ansible to find the role using its expected full name.",
             link_path,
         )
 
-    def _update_env(self, varname: str, value: List[str], default: str = "") -> None:
+    def _update_env(self, varname: str, value: list[str], default: str = "") -> None:
         """Update colon based environment variable if needed.
 
         New values are prepended to make sure they take precedence.
         """
         if not value:
             return
         orig_value = self.environ.get(varname, default)
@@ -636,29 +663,30 @@
             value = [*value, *orig_value.split(":")]
         value_str = ":".join(value)
         if value_str != self.environ.get(varname, ""):
             self.environ[varname] = value_str
             _logger.info("Set %s=%s", varname, value_str)
 
 
-def _get_role_fqrn(galaxy_infos: Dict[str, Any], project_dir: str) -> str:
+def _get_role_fqrn(galaxy_infos: dict[str, Any], project_dir: str) -> str:
     """Compute role fqrn."""
     role_namespace = _get_galaxy_role_ns(galaxy_infos)
     role_name = _get_galaxy_role_name(galaxy_infos)
 
     if len(role_name) == 0:
         role_name = pathlib.Path(project_dir).absolute().name
         role_name = re.sub(r"(ansible-|ansible-role-)", "", role_name).split(
-            ".", maxsplit=2
+            ".",
+            maxsplit=2,
         )[-1]
 
     return f"{role_namespace}{role_name}"
 
 
-def _get_galaxy_role_ns(galaxy_infos: Dict[str, Any]) -> str:
+def _get_galaxy_role_ns(galaxy_infos: dict[str, Any]) -> str:
     """Compute role namespace from meta/main.yml, including trailing dot."""
     role_namespace = galaxy_infos.get("namespace", "")
     if len(role_namespace) == 0:
         role_namespace = galaxy_infos.get("author", "")
     if not isinstance(role_namespace, str):
         raise AnsibleCompatError(f"Role namespace must be string, not {role_namespace}")
     # if there's a space in the name space, it's likely author name
@@ -666,10 +694,10 @@
     if not role_namespace or re.match(r"^\w+ \w+", role_namespace):
         role_namespace = ""
     else:
         role_namespace = f"{role_namespace}."
     return role_namespace
 
 
-def _get_galaxy_role_name(galaxy_infos: Dict[str, Any]) -> str:
+def _get_galaxy_role_name(galaxy_infos: dict[str, Any]) -> str:
     """Compute role name from meta/main.yml."""
     return galaxy_infos.get("role_name", "")
```

### Comparing `ansible-compat-3.0.2/src/ansible_compat/schema.py` & `ansible-compat-4.0.0/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.0.0/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 3.0.2
+Version: 4.0.0
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
@@ -14,25 +14,24 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # ansible-compat
```

### Comparing `ansible-compat-3.0.2/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.0.0/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 .prettierignore
 .prettierrc.yaml
 .readthedocs.yml
 .yamllint
 LICENSE
```

### Comparing `ansible-compat-3.0.2/test/assets/validate0_expected.json` & `ansible-compat-4.0.0/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/test/conftest.py` & `ansible-compat-4.0.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/test/test_config.py` & `ansible-compat-4.0.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/test/test_runtime.py` & `ansible-compat-4.0.0/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/test/test_runtime_example.py` & `ansible-compat-4.0.0/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/test/test_schema.py` & `ansible-compat-4.0.0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-3.0.2/tox.ini` & `ansible-compat-4.0.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 [tox]
 minversion = 4.0.0
 envlist =
   lint
   pkg
   docs
   # matrix assumed current (implicit) is 2.13:
-  py38-ansible212
-  py39{,-devel}
-  py310{,-devel}
-  py311{,-devel}
+  py{39,310,311}{,-devel,-ansible212,-ansible213,-ansible214}
 isolated_build = true
 skip_missing_interpreters = True
 skipsdist = true
 
 [testenv]
 description =
   Run the tests with {basepython}
@@ -55,15 +52,14 @@
   LC_ALL
   LC_CTYPE
 setenv =
   ANSIBLE_DEVEL_WARNING='false'
   COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
   PIP_DISABLE_PIP_VERSION_CHECK = 1
   PIP_CONSTRAINT = {toxinidir}/requirements.txt
-  py38: PIP_CONSTRAINT = /dev/null
   PRE_COMMIT_COLOR = always
   PYTEST_REQPASS = 80
   FORCE_COLOR = 1
 allowlist_externals =
   ansible
   git
   sh
@@ -119,15 +115,15 @@
     {toxinidir}
   # Validate metadata using twine
   twine check --strict {toxinidir}/dist/*
   # Install the wheel
   sh -c "python3 -m pip install {toxinidir}/dist/*.whl"
   pip uninstall -y ansible-compat
 
-[testenv:py{39,38,37,36}]
+[testenv:py]
 description = Run the tests with {basepython} ansible-core 2.12+
 deps =
   {[testenv]deps}
   ansible-core>=2.12
 
 [testenv:docs]
 description = Build docs
```

