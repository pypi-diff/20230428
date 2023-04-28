# Comparing `tmp/xchembku-1.2.0.tar.gz` & `tmp/xchembku-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.2.0.tar", last modified: Mon Apr 24 09:51:29 2023, max compression
+gzip compressed data, was "xchembku-1.3.0.tar", last modified: Fri Apr 28 07:41:31 2023, max compression
```

## Comparing `xchembku-1.2.0.tar` & `xchembku-1.3.0.tar`

### file list

```diff
@@ -1,148 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.734961 xchembku-1.2.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-24 09:51:15.000000 xchembku-1.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-24 09:51:15.000000 xchembku-1.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.730960 xchembku-1.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-24 09:51:15.000000 xchembku-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-24 09:51:15.000000 xchembku-1.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-24 09:51:15.000000 xchembku-1.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 09:51:15.000000 xchembku-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-24 09:51:29.750962 xchembku-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 09:51:15.000000 xchembku-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-24 09:51:15.000000 xchembku-1.2.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.730960 xchembku-1.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-24 09:51:15.000000 xchembku-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:51:29.750962 xchembku-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.734961 xchembku-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_crystal_well_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_soakdb3_crystal_well.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.815016 xchembku-1.3.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 07:41:21.000000 xchembku-1.3.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-28 07:41:21.000000 xchembku-1.3.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.803016 xchembku-1.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-28 07:41:21.000000 xchembku-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-28 07:41:21.000000 xchembku-1.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-28 07:41:21.000000 xchembku-1.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 07:41:21.000000 xchembku-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-28 07:41:31.835016 xchembku-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-28 07:41:21.000000 xchembku-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-28 07:41:21.000000 xchembku-1.3.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.807016 xchembku-1.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-28 07:41:21.000000 xchembku-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:41:31.835016 xchembku-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.811016 xchembku-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_crystal_well_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_soakdb3_crystal_well.py
```

### Comparing `xchembku-1.2.0/.dae-devops/Makefile` & `xchembku-1.3.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/docs/conventions.rst` & `xchembku-1.3.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/docs/developing.rst` & `xchembku-1.3.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/docs/devops.rst` & `xchembku-1.3.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/docs/docs_structure.rst` & `xchembku-1.3.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/docs/installing.rst` & `xchembku-1.3.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/docs/testing.rst` & `xchembku-1.3.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.dae-devops/project.yaml` & `xchembku-1.3.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.devcontainer/Dockerfile` & `xchembku-1.3.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.devcontainer/devcontainer.json` & `xchembku-1.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/CONTRIBUTING.rst` & `xchembku-1.3.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/actions/install_requirements/action.yml` & `xchembku-1.3.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/dependabot.yml` & `xchembku-1.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/pages/make_switcher.py` & `xchembku-1.3.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/workflows/code.yml` & `xchembku-1.3.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/workflows/docs.yml` & `xchembku-1.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/workflows/docs_clean.yml` & `xchembku-1.3.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.github/workflows/linkcheck.yml` & `xchembku-1.3.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.gitignore` & `xchembku-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.gitlab-ci.yml` & `xchembku-1.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/.vscode/launch.json` & `xchembku-1.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/LICENSE` & `xchembku-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/PKG-INFO` & `xchembku-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.2.0
+Version: 1.3.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.2.0/README.rst` & `xchembku-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/configurations/development.yaml` & `xchembku-1.3.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/docs/conf.py` & `xchembku-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/docs/images/dls-favicon.ico` & `xchembku-1.3.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/docs/images/dls-logo.svg` & `xchembku-1.3.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/docs/index.rst` & `xchembku-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.3.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/docs/user/index.rst` & `xchembku-1.3.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/pyproject.toml` & `xchembku-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.3.0/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.2.0
+Version: 1.3.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.2.0/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.3.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 src/xchembku.egg-info/entry_points.txt
 src/xchembku.egg-info/requires.txt
 src/xchembku.egg-info/top_level.txt
 src/xchembku_api/__init__.py
 src/xchembku_api/aiohttp_client.py
 src/xchembku_api/context_base.py
 src/xchembku_api/exceptions.py
+src/xchembku_api/crystal_plate_objects/__init__.py
+src/xchembku_api/crystal_plate_objects/constants.py
 src/xchembku_api/databases/__init__.py
 src/xchembku_api/databases/constants.py
 src/xchembku_api/datafaces/__init__.py
 src/xchembku_api/datafaces/aiohttp.py
 src/xchembku_api/datafaces/constants.py
 src/xchembku_api/datafaces/context.py
 src/xchembku_api/datafaces/datafaces.py
@@ -79,14 +81,16 @@
 src/xchembku_lib/__main__.py
 src/xchembku_lib/_version.py
 src/xchembku_lib/base_aiohttp.py
 src/xchembku_lib/envvar.py
 src/xchembku_lib/version.py
 src/xchembku_lib/contexts/__init__.py
 src/xchembku_lib/contexts/base.py
+src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+src/xchembku_lib/crystal_plate_objects/swiss3.py
 src/xchembku_lib/databases/__init__.py
 src/xchembku_lib/databases/constants.py
 src/xchembku_lib/databases/database_definition.py
 src/xchembku_lib/databases/databases.py
 src/xchembku_lib/databases/normsql.py
 src/xchembku_lib/databases/table_definitions.py
 src/xchembku_lib/datafaces/__init__.py
```

### Comparing `xchembku-1.2.0/src/xchembku_api/context_base.py` & `xchembku-1.3.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.3.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/datafaces/context.py` & `xchembku-1.3.0/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.3.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/exceptions.py` & `xchembku-1.3.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.3.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     # Directory stem where wells were mined from.
     # Also used by echolocator to format the export csv filename.
     rockminer_collected_stem: Optional[str] = None
     # The 4-letter barcode.
     barcode: str
     # The visit gleaned from the Formulatrix database.
     visit: str
+    # A string which allows the CrytsalPlateObjects factory to make an instance.
+    thing_type: Optional[str] = None
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
```

### Comparing `xchembku-1.2.0/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.3.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.3.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.3.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.3.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_cli/main.py` & `xchembku-1.3.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_cli/subcommands/base.py` & `xchembku-1.3.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_cli/subcommands/service.py` & `xchembku-1.3.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_cli/version.py` & `xchembku-1.3.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/__main__.py` & `xchembku-1.3.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/contexts/base.py` & `xchembku-1.3.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/databases/database_definition.py` & `xchembku-1.3.0/src/xchembku_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/databases/databases.py` & `xchembku-1.3.0/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/databases/normsql.py` & `xchembku-1.3.0/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.3.0/src/xchembku_lib/databases/table_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
                 self.fields[field_name] = {"type": sql_type}
 
         # Add indexes.
         self.fields["formulatrix__plate__id"]["index"] = True
         self.fields["barcode"]["index"] = True
         self.fields["visit"]["index"] = True
+        self.fields["thing_type"]["index"] = True
         self.fields[CommonFieldnames.CREATED_ON]["index"] = True
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalWellsTable(TableDefinition):
     # ----------------------------------------------------------------------------------------
     def __init__(self):
```

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/context.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import copy
 import logging
 from typing import Any, Dict, List
 
 from dls_normsql.constants import CommonFieldnames
-from dls_utilpack.describe import describe
 
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 from xchembku_api.models.crystal_well_model import CrystalWellModel
 from xchembku_api.models.crystal_well_needing_droplocation_model import (
     CrystalWellNeedingDroplocationModel,
 )
 from xchembku_lib.datafaces.direct_base import DirectBase
@@ -289,13 +288,11 @@
         query += f"\nORDER BY crystal_wells.{created_on} {sql_direction}"
 
         if filter.limit is not None:
             query += f"\nLIMIT {filter.limit}"
 
         records = await self.query(query, subs=subs, why=why)
 
-        logger.debug(describe("records", records))
-
         # Parse the records returned by sql into models.
         models = [CrystalWellNeedingDroplocationModel(**record) for record in records]
 
         return models
```

### Comparing `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/src/xchembku_lib/version.py` & `xchembku-1.3.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/base.py` & `xchembku-1.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/configurations/direct.yaml` & `xchembku-1.3.0/tests/configurations/direct.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/configurations/service.yaml` & `xchembku-1.3.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/conftest.py` & `xchembku-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/test_crystal_plate.py` & `xchembku-1.3.0/tests/test_crystal_plate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import logging
 from typing import Optional
 
 # Base class for the tester.
 from tests.base import Base
 
+# Types which the CrystalPlateObjects factory can use to build an instance.
+from xchembku_api.crystal_plate_objects.constants import (
+    ThingTypes as CrystalPlateObjectThingTypes,
+)
+
 # Client context creator.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 
 # Object managing datafaces.
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
+# Crystal plate objects factory.
+from xchembku_lib.crystal_plate_objects.crystal_plate_objects import CrystalPlateObjects
+
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
@@ -96,21 +104,33 @@
 
         # Reference the dataface object which the context has set up as the default.
         dataface = xchembku_datafaces_get_default()
 
         visit = "cm00001-1"
         models = []
         models.append(
-            CrystalPlateModel(formulatrix__plate__id=10, barcode="xyz1", visit=visit)
+            CrystalPlateModel(
+                formulatrix__plate__id=10,
+                barcode="xyz1",
+                visit=visit,
+            )
         )
         models.append(
-            CrystalPlateModel(formulatrix__plate__id=20, barcode="xyz2", visit=visit)
+            CrystalPlateModel(
+                formulatrix__plate__id=20,
+                barcode="xyz2",
+                visit=visit,
+            )
         )
         models.append(
-            CrystalPlateModel(formulatrix__plate__id=30, barcode="xyz3", visit=visit)
+            CrystalPlateModel(
+                formulatrix__plate__id=30,
+                barcode="xyz3",
+                visit=visit,
+            )
         )
 
         await dataface.upsert_crystal_plates(models)
 
         # Check the filtered queries.
         await self.__check(
             dataface,
@@ -161,15 +181,18 @@
             "from plate_id",
             formulatrix__plate__id=20,
         )
 
         # ------------------------------------------------------------------------------------
         # Create an object to be upserted.
         upserted_model = CrystalPlateModel(
-            formulatrix__plate__id=40, barcode="xyz4", visit=visit
+            formulatrix__plate__id=40,
+            barcode="xyz4",
+            visit=visit,
+            thing_type=CrystalPlateObjectThingTypes.SWISS3,
         )
 
         # First upsert is an insert.
         await dataface.upsert_crystal_plates([upserted_model])
         upserted_models = await self.__check(
             dataface,
             CrystalPlateFilterModel(limit=1, direction=-1),
@@ -203,14 +226,19 @@
             formulatrix__plate__id=40,
         )
 
         assert upserted_models[0].uuid == upserted_model.uuid
         assert upserted_models[0].created_on == created_on
         assert upserted_models[0].visit == upserted_model.visit
 
+        # Make sure that the model which came out of the database can be instantiated.
+        specification = {"type": upserted_models[0].thing_type}
+        o = CrystalPlateObjects().build_object(specification)
+        assert o.get_well_count() == 288
+
     # ----------------------------------------------------------------------------------------
 
     async def __check(
         self,
         dataface,
         filter: CrystalPlateFilterModel,
         expected: int,
```

### Comparing `xchembku-1.2.0/tests/test_crystal_well_autolocation.py` & `xchembku-1.3.0/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/test_crystal_well_droplocation.py` & `xchembku-1.3.0/tests/test_crystal_well_droplocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.2.0/tests/test_soakdb3_crystal_well.py` & `xchembku-1.3.0/tests/test_soakdb3_crystal_well.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 from pathlib import Path
 
 # Soakdb3 database.
 from soakdb3_api.databases.constants import Tablenames
 
-# The model which describes the crystal wells to be injected into soakdb3.
 # Client for direct access to the soakdb3 database for seeding it.
 from soakdb3_api.datafaces.context import Context as Soakdb3DatafaceClientContext
 from soakdb3_api.datafaces.datafaces import (
     datafaces_get_default as soakdb3_datafaces_get_default,
 )
+
+# The model which describes the crystal wells to be injected into soakdb3.
 from soakdb3_api.models.crystal_well_model import (
     CrystalWellModel as Soakdb3CrystalWellModel,
 )
 
 # The service process startup/teardown context.
 from soakdb3_lib.datafaces.context import Context as Soakdb3DatafaceServerContext
```

