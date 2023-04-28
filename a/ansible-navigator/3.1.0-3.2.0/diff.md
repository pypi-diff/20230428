# Comparing `tmp/ansible-navigator-3.1.0.tar.gz` & `tmp/ansible-navigator-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.1.0.tar", last modified: Fri Apr 28 11:51:14 2023, max compression
+gzip compressed data, was "ansible-navigator-3.2.0.tar", last modified: Fri Apr 28 20:08:58 2023, max compression
```

## Comparing `ansible-navigator-3.1.0.tar` & `ansible-navigator-3.2.0.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.954349 ansible-navigator-3.1.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.962350 ansible-navigator-3.1.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.962350 ansible-navigator-3.1.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/contributing/guidelines.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.962350 ansible-navigator-3.1.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.950349 ansible-navigator-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.966349 ansible-navigator-3.1.0/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.974350 ansible-navigator-3.1.0/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.974350 ansible-navigator-3.1.0/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.974350 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (123)    31546 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    49134 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.978350 ansible-navigator-3.1.0/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.986350 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.990350 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.966349 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.362619 ansible-navigator-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.326619 ansible-navigator-3.2.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.326619 ansible-navigator-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/contributing/guidelines.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.334619 ansible-navigator-3.2.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:08:58.362619 ansible-navigator-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.322618 ansible-navigator-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.334619 ansible-navigator-3.2.0/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 20:08:57.000000 ansible-navigator-3.2.0/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.342619 ansible-navigator-3.2.0/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.342619 ansible-navigator-3.2.0/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.342619 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31546 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49134 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.346619 ansible-navigator-3.2.0/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.346619 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.350619 ansible-navigator-3.2.0/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.350619 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.350619 ansible-navigator-3.2.0/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.354619 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.334619 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/tox.ini
```

### Comparing `ansible-navigator-3.1.0/.config/dictionary.txt` & `ansible-navigator-3.2.0/.config/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.flake8` & `ansible-navigator-3.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.git_archival.txt` & `ansible-navigator-3.2.0/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.github/CONTRIBUTING.md` & `ansible-navigator-3.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.github/SECURITY.md` & `ansible-navigator-3.2.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.github/dependabot.yml` & `ansible-navigator-3.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.github/workflows/release.yml` & `ansible-navigator-3.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.github/workflows/tox.yml` & `ansible-navigator-3.2.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.gitignore` & `ansible-navigator-3.2.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+
+# builder context dirs
+context
+
+# test output
 /tests/output/
 
 # tmux integration test logs
 .test_logs
 
 
 # Byte-compiled / optimized / DLL files
```

### Comparing `ansible-navigator-3.1.0/.pre-commit-config.yaml` & `ansible-navigator-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.prettierignore` & `ansible-navigator-3.2.0/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/.vscode/launch.json` & `ansible-navigator-3.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/LICENSE` & `ansible-navigator-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/PKG-INFO` & `ansible-navigator-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.1.0
+Version: 3.2.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.1.0/README.md` & `ansible-navigator-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/cspell.config.yaml` & `ansible-navigator-3.2.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.2.0/docs/_ext/regenerate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/contributing/guidelines.md` & `ansible-navigator-3.2.0/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/contributing/security.md` & `ansible-navigator-3.2.0/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/faq.md` & `ansible-navigator-3.2.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/index.md` & `ansible-navigator-3.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/installation.md` & `ansible-navigator-3.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/settings.md` & `ansible-navigator-3.2.0/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/docs/subcommands.md` & `ansible-navigator-3.2.0/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.2.0/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/mkdocs.yml` & `ansible-navigator-3.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/mypy.ini` & `ansible-navigator-3.2.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/pyproject.toml` & `ansible-navigator-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/requirements.txt` & `ansible-navigator-3.2.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --strip-extras setup.cfg
 #
-ansible-builder==1.2.0
+ansible-builder==3.0.0rc1
 ansible-core==2.14.3
 ansible-runner==2.3.2
 attrs==22.2.0
 beautifulsoup4==4.12.0
 bindep==2.11.0
 cairocffi==1.5.0
 cairosvg==2.7.0
```

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.2.0/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/action_base.py` & `ansible-navigator-3.2.0/src/ansible_navigator/action_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.2.0/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.2.0/src/ansible_navigator/action_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/_actions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/back.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/exec.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/filter.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/help_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/images.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/lint.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/log.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/open_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/quit.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/refresh.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/rerun.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/rerun.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/run.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_notification.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_working.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/save.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/select.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_json.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/settings.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/stdout.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/template.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/welcome.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.2.0/src/ansible_navigator/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/app_public.py` & `ansible-navigator-3.2.0/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/cli.py` & `ansible-navigator-3.2.0/src/ansible_navigator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.2.0/src/ansible_navigator/command_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/constants.py` & `ansible-navigator-3.2.0/src/ansible_navigator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.2.0/src/ansible_navigator/content_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/ansible-navigator.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'title'": "'ansible-navigator settings v3.1'", "'version'": "'3.1'"}*

```diff
@@ -516,11 +516,11 @@
                 }
             }
         }
     },
     "required": [
         "ansible-navigator"
     ],
-    "title": "ansible-navigator settings v3.0",
+    "title": "ansible-navigator settings v3.1",
     "type": "object",
-    "version": "3.0"
+    "version": "3.1"
 }
```

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.2.0/src/ansible_navigator/data/catalog_collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/help.md` & `ansible-navigator-3.2.0/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.2.0/src/ansible_navigator/data/image_introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.2.0/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.2.0/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.2.0/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.2.0/src/ansible_navigator/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspect.py` & `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/puller.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/initialization.py` & `ansible-navigator-3.2.0/src/ansible_navigator/initialization.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/logger.py` & `ansible-navigator-3.2.0/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.2.0/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/steps.py` & `ansible-navigator-3.2.0/src/ansible_navigator/steps.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/fchainmap.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/fchainmap.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/state.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/colorize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/validators.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/dict_merge.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/dot_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/functions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/key_value_store.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/settings_file.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.2.0/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.1.0
+Version: 3.2.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.1.0/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.2.0/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.1.0/tox.ini` & `ansible-navigator-3.2.0/tox.ini`

 * *Files identical despite different names*

