# Comparing `tmp/ansible-navigator-3.0.2.tar.gz` & `tmp/ansible-navigator-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.0.2.tar", last modified: Tue Apr  4 14:58:21 2023, max compression
+gzip compressed data, was "ansible-navigator-3.1.0.tar", last modified: Fri Apr 28 11:51:14 2023, max compression
```

## Comparing `ansible-navigator-3.0.2.tar` & `ansible-navigator-3.1.0.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.454183 ansible-navigator-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.414183 ansible-navigator-3.0.2/.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.414183 ansible-navigator-3.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-04 14:58:21.454183 ansible-navigator-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.418183 ansible-navigator-3.0.2/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/contributing/guidelines.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.422183 ansible-navigator-3.0.2/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:58:21.454183 ansible-navigator-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.406183 ansible-navigator-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.426183 ansible-navigator-3.0.2/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 14:58:20.000000 ansible-navigator-3.0.2/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.434183 ansible-navigator-3.0.2/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    26953 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.434183 ansible-navigator-3.0.2/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.434183 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (123)    31546 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    49134 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.434183 ansible-navigator-3.0.2/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (123)    23528 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.438183 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.438183 ansible-navigator-3.0.2/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.442183 ansible-navigator-3.0.2/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/image_manager/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.442183 ansible-navigator-3.0.2/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.446183 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.450183 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.450183 ansible-navigator-3.0.2/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.454183 ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:58:21.426183 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-04 14:58:21.000000 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-04 14:58:21.000000 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:58:21.000000 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-04 14:58:21.000000 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-04 14:58:21.000000 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 14:58:21.000000 ansible-navigator-3.0.2/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-04 14:57:54.000000 ansible-navigator-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.954349 ansible-navigator-3.1.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.958350 ansible-navigator-3.1.0/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.962350 ansible-navigator-3.1.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.962350 ansible-navigator-3.1.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/contributing/guidelines.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.962350 ansible-navigator-3.1.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.950349 ansible-navigator-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.966349 ansible-navigator-3.1.0/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.974350 ansible-navigator-3.1.0/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.974350 ansible-navigator-3.1.0/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.974350 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31546 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49134 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.978350 ansible-navigator-3.1.0/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.982350 ansible-navigator-3.1.0/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.986350 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.990350 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.994350 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:51:14.966349 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 11:51:14.000000 ansible-navigator-3.1.0/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 11:50:53.000000 ansible-navigator-3.1.0/tox.ini
```

### Comparing `ansible-navigator-3.0.2/.config/dictionary.txt` & `ansible-navigator-3.1.0/.config/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.flake8` & `ansible-navigator-3.1.0/.flake8`

 * *Files 9% similar despite different names*

```diff
@@ -32,39 +32,27 @@
   # Metadata of `pip wheel` cmd is autogenerated
   pip-wheel-metadata,
   # adjacent venv
   venv
 
 # IMPORTANT: avoid using ignore option, always use extend-ignore instead
 # Completely and unconditionally ignore the following errors:
-extend-ignore =
-  # Safeguard neutering of flake8-quotes : https://github.com/zheller/flake8-quotes/issues/105
-  Q,
-  # annoy black by allowing white space before : https://github.com/psf/black/issues/315
-  E203,
-  # duplicate of pylint W0611 (unused-import)
-  F401,
-  # duplicate of pylint E0602 (undefined-variable)
-  F821,
-  # duplicate of pylint W0612 (unused-variable)
-  F841,
+extend-ignore = F, E203
 
 # Accessibility/large fonts and PEP8 unfriendly:
 max-line-length = 100
 
 # Allow certain violations in certain files:
 # Please keep both sections of this list sorted, as it will be easier for others to find and add entries in the future
 per-file-ignores =
   # The following ignores have been researched and should be considered permanent
   # each should be preceeded with an explanation of each of the error codes
   # If other ignores are added for a specific file in the section following this,
   # these will need to be added to that line as well.
 
-  # S101: Allow the use of assert within the tests directory, since tests require it.
-  tests/**.py: S101
 
   # The tokenization code is vendored and not a priority for docstrings.
   src/ansible_navigator/tm_tokenize/__init__.py: D104
   src/ansible_navigator/tm_tokenize/compiler.py: D100, D101, D102
   src/ansible_navigator/tm_tokenize/fchainmap.py: D100, D101, D105
   src/ansible_navigator/tm_tokenize/grammars.py: D100, D101, D102
   src/ansible_navigator/tm_tokenize/reg.py: D100, D103
```

### Comparing `ansible-navigator-3.0.2/.git_archival.txt` & `ansible-navigator-3.1.0/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.github/CONTRIBUTING.md` & `ansible-navigator-3.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.github/SECURITY.md` & `ansible-navigator-3.1.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.github/dependabot.yml` & `ansible-navigator-3.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.github/workflows/release.yml` & `ansible-navigator-3.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.github/workflows/tox.yml` & `ansible-navigator-3.1.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.gitignore` & `ansible-navigator-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.pre-commit-config.yaml` & `ansible-navigator-3.1.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 ---
 default_language_version:
   # ensures that we get same behavior on CI(s) as on local machines
   python: python3.11
 repos:
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        name: Sort import statements using isort
-
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.6"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         # Original hook implementation is flaky due to *several* bugs described
         # in https://github.com/prettier/prettier/issues/12364
         # a) CI=1 needed to avoid incomplete output
         # b) two executions are needed because --list-different works correctly
         # only when run with --check as with --write the output will also
@@ -31,27 +25,34 @@
         pass_filenames: false
         args: []
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
 
   - repo: https://github.com/psf/black.git
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
 
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.263"
+    hooks:
+      - id: ruff
+        args:
+          - "--exit-non-zero-on-fix"
+
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v6.30.1
+    rev: v6.31.0
     hooks:
       - id: cspell
         name: Spell check with cspell
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks.git
-    rev: v1.4.2
+    rev: v1.5.1
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
     rev: v4.4.0
     hooks:
       # Side-effects:
@@ -112,40 +113,38 @@
             (
               tests/fixtures/integration/actions/.*\.json|
               src/ansible_navigator/data/grammar/.*\.json
             )
           $
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.30.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - --strict
         types: [file, yaml]
 
   - repo: https://github.com/PyCQA/flake8.git
     rev: 6.0.0
     hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - darglint
-          - flake8-2020 >= 1.6.0
           - flake8-docstrings # uses pydocstyle
-          - flake8-future-annotations>=0.0.3
-          - flake8-isort >= 4.1.1
+
   - repo: https://github.com/asottile/pyupgrade
     # keep it after flake8
     rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: ["--py39-plus"]
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies:
           - jinja2
           - libtmux
           - pytest
           - pytest-mock
@@ -153,15 +152,15 @@
           - types-docutils
           - types-mock
           - types-PyYAML
           - types-setuptools # Needed logging version
           - types-typed-ast
 
   - repo: https://github.com/pycqa/pylint.git
-    rev: v2.17.1
+    rev: v3.0.0a6
     hooks:
       - id: pylint
         args:
           - docs/
           - src/
           - tests/
         additional_dependencies:
```

### Comparing `ansible-navigator-3.0.2/.prettierignore` & `ansible-navigator-3.1.0/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/.vscode/launch.json` & `ansible-navigator-3.1.0/.vscode/launch.json`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,55 @@
     {
       "name": "Debug tests",
       "type": "python",
       "request": "launch",
       "purpose": ["debug-test"],
       "console": "integratedTerminal"
     },
-    // Configuration for pure debugging (use args attribute accordingly)
+    // Configuration for pure debugging (use args and cwd attributes accordingly)
     {
       "name": "Debug subcommand: collections",
       "type": "python",
       "request": "launch",
       "module": "ansible_navigator",
-      "args": ["collections"],
+      "args": ["collections", "--ee", "false"],
       "cwd": "${workspaceFolder}/src",
       "justMyCode": false
     },
     {
       "name": "Debug subcommand: exec",
       "type": "python",
       "request": "launch",
       "module": "ansible_navigator",
       "args": ["exec", "--", "pwd"],
       "cwd": "${workspaceFolder}/src",
       "justMyCode": false
+    },
+    {
+      "name": "Debug subcommand: images",
+      "type": "python",
+      "request": "launch",
+      "module": "ansible_navigator",
+      "args": ["images"],
+      "cwd": "${workspaceFolder}/src",
+      "justMyCode": false
+    },
+    {
+      "name": "Debug subcommand: lint",
+      "type": "python",
+      "request": "launch",
+      "module": "ansible_navigator",
+      "args": ["lint", "tests/fixtures/integration/actions/lint"],
+      "cwd": "${workspaceFolder}",
+      "justMyCode": false
+    },
+    {
+      "name": "Debug subcommand: run",
+      "type": "python",
+      "request": "launch",
+      "module": "ansible_navigator",
+      "args": ["run", "ping.yml"],
+      "cwd": "/home/user/../path/to/the/playbook",
+      "justMyCode": false
     }
   ]
 }
```

### Comparing `ansible-navigator-3.0.2/.vscode/settings.json` & `ansible-navigator-3.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/LICENSE` & `ansible-navigator-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/PKG-INFO` & `ansible-navigator-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.0.2
+Version: 3.1.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
@@ -70,15 +70,15 @@
 [ansible-core]: https://docs.ansible.com/ansible-core/devel
 [Python venv doc]: https://docs.python.org/3/library/venv.html
 
 Additional `Linux`, `macOS` and `Windows with WSL2` installation
 instructions are available in the [Installation guide].
 
 [Installation guide]:
-https://ansible-navigator.readthedocs.io/en/latest/installation
+https://ansible-navigator.readthedocs.io/installation/
 
 ## Welcome
 
 When running `ansible-navigator` with no arguments, you will be presented with
 the *welcome page*. From this page, you can run playbooks, browse collections,
 explore inventories, read Ansible documentation, and more.
 
@@ -95,15 +95,15 @@
   output to the terminal's standard output stream, as Ansible's commands
   would.
 
 The **interactive** mode is the default and this default can be overwritten by
 passing `--mode stdout` (`-m stdout`) or setting `mode` in
 [configuration][settings documentation].
 
-[settings documentation]: https://ansible-navigator.readthedocs.io/en/latest/settings
+[settings documentation]: https://ansible-navigator.readthedocs.io/settings/
 
 ## Example commands
 
 All of ansible-navigator's features can be accessed from the *welcome page*
 described above, but as a shortcut, commands can also be provided directly as
 command-line arguments.
 
@@ -126,15 +126,15 @@
   `ansible-navigator config dump -m stdout`
 * Show documentation: `ansible-navigator doc sudo -t become  -m stdout`
 
 ... and so on. A full list of subcommands and their relation to Ansible
 commands can be found in the [subcommand documentation].
 
 [subcommand documentation]:
-https://ansible-navigator.readthedocs.io/en/latest/subcommands
+https://ansible-navigator.readthedocs.io/subcommands/
 
 ## Configuring ansible-navigator
 
 There are several ways to configure ansible-navigator and users and projects
 are free to choose the most convenient method for them. The full hierarchy of
 how various configuration sources are applied can be found in the FAQ mentioned
 below.
@@ -146,15 +146,15 @@
 
 ## Frequently Asked Questions (FAQ)
 
 We maintain a [list of common questions][FAQ] which provides a good
 resource to check if something is tripping you up. We also encourage additions
 to this document for the greater community!
 
-[FAQ]: https://ansible-navigator.readthedocs.io/en/latest/faq
+[FAQ]: https://ansible-navigator.readthedocs.io/faq/
 
 ## License
 
 ansible-navigator is released under the Apache License version 2. See the
 [LICENSE] file for more details.
 
 [LICENSE]: https://github.com/ansible/ansible-navigator/blob/main/LICENSE
```

### Comparing `ansible-navigator-3.0.2/README.md` & `ansible-navigator-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 [ansible-core]: https://docs.ansible.com/ansible-core/devel
 [Python venv doc]: https://docs.python.org/3/library/venv.html
 
 Additional `Linux`, `macOS` and `Windows with WSL2` installation
 instructions are available in the [Installation guide].
 
 [Installation guide]:
-https://ansible-navigator.readthedocs.io/en/latest/installation
+https://ansible-navigator.readthedocs.io/installation/
 
 ## Welcome
 
 When running `ansible-navigator` with no arguments, you will be presented with
 the *welcome page*. From this page, you can run playbooks, browse collections,
 explore inventories, read Ansible documentation, and more.
 
@@ -61,15 +61,15 @@
   output to the terminal's standard output stream, as Ansible's commands
   would.
 
 The **interactive** mode is the default and this default can be overwritten by
 passing `--mode stdout` (`-m stdout`) or setting `mode` in
 [configuration][settings documentation].
 
-[settings documentation]: https://ansible-navigator.readthedocs.io/en/latest/settings
+[settings documentation]: https://ansible-navigator.readthedocs.io/settings/
 
 ## Example commands
 
 All of ansible-navigator's features can be accessed from the *welcome page*
 described above, but as a shortcut, commands can also be provided directly as
 command-line arguments.
 
@@ -92,15 +92,15 @@
   `ansible-navigator config dump -m stdout`
 * Show documentation: `ansible-navigator doc sudo -t become  -m stdout`
 
 ... and so on. A full list of subcommands and their relation to Ansible
 commands can be found in the [subcommand documentation].
 
 [subcommand documentation]:
-https://ansible-navigator.readthedocs.io/en/latest/subcommands
+https://ansible-navigator.readthedocs.io/subcommands/
 
 ## Configuring ansible-navigator
 
 There are several ways to configure ansible-navigator and users and projects
 are free to choose the most convenient method for them. The full hierarchy of
 how various configuration sources are applied can be found in the FAQ mentioned
 below.
@@ -112,15 +112,15 @@
 
 ## Frequently Asked Questions (FAQ)
 
 We maintain a [list of common questions][FAQ] which provides a good
 resource to check if something is tripping you up. We also encourage additions
 to this document for the greater community!
 
-[FAQ]: https://ansible-navigator.readthedocs.io/en/latest/faq
+[FAQ]: https://ansible-navigator.readthedocs.io/faq/
 
 ## License
 
 ansible-navigator is released under the Apache License version 2. See the
 [LICENSE] file for more details.
 
 [LICENSE]: https://github.com/ansible/ansible-navigator/blob/main/LICENSE
```

### Comparing `ansible-navigator-3.0.2/cspell.config.yaml` & `ansible-navigator-3.1.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.1.0/docs/_ext/regenerate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/contributing/guidelines.md` & `ansible-navigator-3.1.0/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/contributing/security.md` & `ansible-navigator-3.1.0/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/faq.md` & `ansible-navigator-3.1.0/docs/faq.md`

 * *Files 2% similar despite different names*

```diff
@@ -253,16 +253,17 @@
 $ touch ~/.vault_password
 $ chmod 600 ~/.vault_password
 # The leading space here is necessary to keep the command out of the command history
 $  echo my_password >> ~/.vault_password
 # Link the password file into the current working directory
 $ ln ~/.vault_password .
 # Set the environment variable to the location of the file
-$ ANSIBLE_VAULT_PASSWORD_FILE=.vault_password
-$ ansible-navigator run site.yml
+$ export ANSIBLE_VAULT_PASSWORD_FILE=.vault_password
+# Pass the variable into the execution-environment
+$ ansible-navigator run --pass-environment-variable ANSIBLE_VAULT_PASSWORD_FILE site.yml
 ```
 
 2. Store the vault password in an environment variable
 
 ```bash
 $ touch ~/.vault_password.sh
 $ chmod 700 ~/.vault_password.sh
```

### Comparing `ansible-navigator-3.0.2/docs/index.md` & `ansible-navigator-3.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/installation.md` & `ansible-navigator-3.1.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/settings.md` & `ansible-navigator-3.1.0/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/docs/subcommands.md` & `ansible-navigator-3.1.0/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.1.0/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/mkdocs.yml` & `ansible-navigator-3.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/mypy.ini` & `ansible-navigator-3.1.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/requirements.txt` & `ansible-navigator-3.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.1.0/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/action_base.py` & `ansible-navigator-3.1.0/src/ansible_navigator/action_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import logging
 
 from copy import deepcopy
 from re import Pattern
 
 from ansible_navigator.actions import kegexes
+
 from .action_defs import RunStdoutReturn
 from .app_public import AppPublic
 from .configuration_subsystem import Constants as C
 from .configuration_subsystem.definitions import ApplicationConfiguration
 from .initialization import parse_and_update
 from .steps import Steps
 from .ui_framework import Interaction
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.1.0/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.1.0/src/ansible_navigator/action_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ``:quit`` is requested by the user.
 """
 
 from typing import TYPE_CHECKING
 
 from ansible_navigator.actions import kegexes
 from ansible_navigator.actions import run_action
+
 from .action_base import ActionBase
 from .configuration_subsystem.definitions import ApplicationConfiguration
 from .constants import GRAMMAR_DIR
 from .constants import TERMINAL_COLORS_PATH
 from .constants import THEME_PATH
 from .steps import Steps
 from .ui_framework import Interaction
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/_actions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/back.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,22 @@
         print_to_stdout(
             content=collections_info,
             content_format=getattr(ContentFormat, self._args.format.upper()),
             use_color=self._args.display_color,
         )
         return RunStdoutReturn(message="", return_code=0)
 
+    def notify_failed(self):
+        """Notify collection cataloging failed."""
+        msgs = ["humph. Something went really wrong while cataloging collections."]
+        msgs.append("Details have been added to the log file")
+        closing = ["[HINT] Please log an issue about this one, it shouldn't have happened"]
+        warning = warning_notification(messages=msgs + closing)
+        self._interaction.ui.show_form(warning)
+
     def notify_none(self):
         """Notify no collections were found."""
         msgs = ["humph. no collections were found in the following paths:"]
         paths = []
         for path in self._collection_scanned_paths:
             if path.startswith(self._args.internals.cache_path):
                 continue
@@ -224,15 +232,15 @@
                     paths.append(f"- {path} (bind_mount)")
                 else:
                     paths.append(f"- {path} (contained)")
             else:
                 paths.append(f"- {path}")
         closing = ["[HINT] Try installing some or try a different execution environment"]
         warning = warning_notification(messages=msgs + paths + closing)
-        self._interaction.ui.show(warning)
+        self._interaction.ui.show_form(warning)
 
     def _take_step(self) -> None:
         """Take a step based on the current step or step back."""
         result = None
         if isinstance(self.steps.current, Interaction):
             result = run_action(self.steps.current.name, self.app, self.steps.current)
         elif isinstance(self.steps.current, Step):
@@ -483,19 +491,22 @@
 
         self._logger.debug(
             "Invoke runner with executable_cmd: %s and kwargs: %s",
             python_exec_path,
             kwargs,
         )
         _runner = Command(executable_cmd=python_exec_path, **kwargs)
-        output, error, _ = _runner.run()
+        output, error, ret_code = _runner.run()
 
         if error:
             msg = f"Error while running catalog collection script: {error}"
             self._logger.error(msg)
+        if ret_code:
+            self._logger.error(output)
+            self.notify_failed()
         if output:
             self._parse(output)
 
     def _parse(self, output) -> None:
         """Load and process the ``json`` output from the collection cataloging process.
 
         :param output: The output from the collection cataloging process
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,40 +20,53 @@
 logger = logging.getLogger(__name__)
 
 
 def _generate_command(
     exec_command: str,
     exec_shell: bool,
     extra_args: Constants | list[str],
+    exec_command_is_default: bool,
 ) -> GeneratedCommand:
     """Generate the command and args.
 
     :param exec_command: The command to run
     :param exec_shell: Should the command be wrapped in a shell
     :param extra_args: Any unknown or extra arguments passed on the command line
+    :param exec_command_is_default: If the exec_command is set to its default value
     :returns: The command and any pass through arguments
     """
     logger.debug("exec_command: %s", exec_command)
     logger.debug("exec_shell: %s", exec_shell)
     logger.debug("extra_args: %s", extra_args)
-    if exec_shell and exec_command:
+    if exec_shell:
         command = "/bin/bash"
         # Determine if any extra args were picked up
-        _extra_args = extra_args if isinstance(extra_args, list) else ()
-        pass_command = " ".join((exec_command, *_extra_args))
-        pass_through_args = ["-c", pass_command]
+        _extra_args = []
+        if not exec_command_is_default:
+            _extra_args.append(exec_command)
+        if isinstance(extra_args, list):
+            _extra_args.extend(extra_args)
+        if _extra_args:
+            pass_command = " ".join(_extra_args)
+            pass_through_args = ["-c", pass_command]
+        else:
+            pass_through_args = []
+
     else:
-        parts = shlex.split(exec_command)
-        command = parts[0]
-        if len(parts) == 1 and isinstance(extra_args, list):
-            # Use the extra arguments
-            pass_through_args = extra_args
+        if exec_command_is_default and isinstance(extra_args, list):
+            command, pass_through_args = extra_args[0], extra_args[1:]
         else:
-            # Use the leftovers or an empty list
-            pass_through_args = parts[1:]
+            parts = shlex.split(exec_command)
+            command = parts[0]
+            if len(parts) == 1 and isinstance(extra_args, list):
+                # Use the extra arguments
+                pass_through_args = extra_args
+            else:
+                # Use the leftovers or an empty list
+                pass_through_args = parts[1:]
     logger.debug("runner command: %s", command)
     logger.debug("runner passthrough: %s", pass_through_args)
     return (command, pass_through_args)
 
 
 @actions.register
 class Action(ActionBase):
@@ -124,13 +137,15 @@
         if isinstance(self._args.container_options, list):
             kwargs["container_options"] = self._args.container_options
 
         command, pass_through_args = _generate_command(
             exec_command=self._args.exec_command,
             exec_shell=self._args.exec_shell,
             extra_args=self._args.cmdline,
+            exec_command_is_default=self._args.entry("exec_command").value.source
+            is Constants.DEFAULT_CFG,
         )
         if isinstance(pass_through_args, list):
             kwargs["cmdline"] = pass_through_args
 
         runner = Command(executable_cmd=command, **kwargs)
         return runner.run()
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/filter.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/help_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``:help`` command implementation."""
 
 from ansible_navigator.content_defs import ContentFormat
+
 from ..action_base import ActionBase
 from ..app_public import AppPublic
 from ..configuration_subsystem.definitions import ApplicationConfiguration
 from ..ui_framework import Interaction
 from ..utils.packaged_data import retrieve_content
 from . import _actions as actions
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,8 +574,8 @@
 
     def notify_failed(self):
         """Notify image introspection failed."""
         msgs = ["humph. Something went really wrong while introspecting the image."]
         msgs.append("Details have been added to the log file")
         closing = ["[HINT] Please log an issue about this one, it shouldn't have happened"]
         warning = warning_notification(messages=msgs + closing)
-        self._interaction.ui.show(warning)
+        self._interaction.ui.show_form(warning)
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import shlex
 import shutil
 
 from pathlib import Path
 from typing import Any
 
 from ansible_navigator.content_defs import ContentFormat
+
 from ..action_base import ActionBase
 from ..action_defs import RunStdoutReturn
 from ..app_public import AppPublic
 from ..configuration_subsystem.definitions import ApplicationConfiguration
 from ..runner import AnsibleInventory
 from ..runner import Command
 from ..steps import Step
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/lint.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``:log`` command implementation."""
 from ansible_navigator.content_defs import ContentFormat
+
 from ..action_base import ActionBase
 from ..app_public import AppPublic
 from ..configuration_subsystem.definitions import ApplicationConfiguration
 from ..ui_framework import Interaction
 from . import _actions as actions
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/open_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/quit.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/refresh.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/rerun.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/rerun.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/run.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_notification.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/sample_working.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/sample_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/save.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/select.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_json.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``:yaml`` command implementation."""
 import logging
 
 from ansible_navigator.content_defs import ContentFormat
+
 from ..app_public import AppPublic
 from ..configuration_subsystem.definitions import ApplicationConfiguration
 from ..ui_framework import Interaction
 from . import _actions as actions
 
 
 @actions.register
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """The ``settings`` subcommand action."""
 from __future__ import annotations
 
 from dataclasses import asdict
 from functools import partial
 
 from ansible_navigator.configuration_subsystem.definitions import Constants
+
 from ..action_base import ActionBase
 from ..action_defs import RunStdoutReturn
 from ..app_public import AppPublic
 from ..configuration_subsystem import PresentableSettingsEntries
 from ..configuration_subsystem import PresentableSettingsEntry
 from ..configuration_subsystem import to_effective
 from ..configuration_subsystem import to_presentable
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/stdout.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/template.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/welcome.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.1.0/src/ansible_navigator/actions/write_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import re
 
 from pathlib import Path
 
 from ansible_navigator.content_defs import ContentView
+
 from ..app_public import AppPublic
 from ..configuration_subsystem.definitions import ApplicationConfiguration
 from ..content_defs import SerializationFormat
 from ..ui_framework import Interaction
 from ..utils.functions import remove_dbl_un
 from ..utils.serialize import serialize_write_file
 from . import _actions as actions
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/app_public.py` & `ansible-navigator-3.1.0/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/cli.py` & `ansible-navigator-3.1.0/src/ansible_navigator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.1.0/src/ansible_navigator/command_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,18 +278,26 @@
                     message = f"'{entry.name}' cannot be reconfigured. (environment variables)"
                     self._messages.append(LogMessage(level=logging.INFO, message=message))
 
     def _apply_cli_params(self) -> None:
         """Apply the cli params."""
         parser = Parser(self._config).parser
         setattr(parser, "error", self._argparse_error_handler)
-        parser_response = parser.parse_known_args(self._params)
+        try:
+            # split the _params on double-dash
+            index = self._params.index("--")
+            before, after = self._params[:index], self._params[index + 1 :]
+        except ValueError:
+            before, after = self._params, []
+
+        parser_response = parser.parse_known_args(before)
         if parser_response is None:
             return
-        args, cmdline = parser_response
+        args, unknown = parser_response
+        cmdline = unknown + after
         if cmdline:
             # In the case a subcommand is not a positional, remove the --
             additional_args = [arg for arg in cmdline if arg != "--"]
             self._config.entry("cmdline").value.current = additional_args
             self._config.entry("cmdline").value.source = C.USER_CLI
         for param, value in vars(args).items():
             if self._config.entry(param).subcommand_value is True and value is None:
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.1.0/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/constants.py` & `ansible-navigator-3.1.0/src/ansible_navigator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.1.0/src/ansible_navigator/content_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/ansible-navigator.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.1.0/src/ansible_navigator/data/catalog_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,16 @@
         collection_name: str = collection["known_as"]
         collection["roles"] = []
         roles_directory = Path(collection["path"], "roles")
         if not roles_directory.is_dir():
             return
 
         for role_directory in roles_directory.iterdir():
+            if not role_directory.is_dir():
+                continue
             role: dict[str, str | dict[str, Any]] = {
                 "short_name": role_directory.name,
                 "full_name": f"{collection_name}.{role_directory.name}",
             }
             error_cataloging_role = False
 
             # Argument spec cataloging, it is not required
@@ -422,14 +424,15 @@
                         ),
                     )
                 handled.add(checksum)
     return handled, missing, plugin_count
 
 
 def parse_args() -> tuple[argparse.Namespace, list[Path]]:
+    # pylint: disable=used-before-assignment
     """Parse the arguments from the command line.
 
     :returns: The parsed arguments and all directories to search
     """
     parser = argparse.ArgumentParser(description="Catalog collections.")
     parser.add_argument(
         "-d",
@@ -544,14 +547,15 @@
         return {"stdout": proc_out.stdout}
     except subprocess.CalledProcessError as exc:
         return {"error": str(exc)}
 
 
 def main() -> dict:
     # pylint: disable=protected-access
+    # pylint: disable=used-before-assignment
     """Run the collection catalog process.
 
     :returns: The results from the completed collection cataloging process
     """
     stats = {}
     stats["cache_added_success"] = 0
     stats["cache_added_errors"] = 0
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/help.md` & `ansible-navigator-3.1.0/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.1.0/src/ansible_navigator/data/image_introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.1.0/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.1.0/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.1.0/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.1.0/src/ansible_navigator/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/image_manager/introspect.py` & `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/introspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.1.0/src/ansible_navigator/image_manager/puller.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/initialization.py` & `ansible-navigator-3.1.0/src/ansible_navigator/initialization.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/logger.py` & `ansible-navigator-3.1.0/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.1.0/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/steps.py` & `ansible-navigator-3.1.0/src/ansible_navigator/steps.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import annotations
 
 import functools
 
 from typing import TYPE_CHECKING
-from typing import Dict
-from typing import List
-from typing import Tuple
 
 from .fchainmap import FChainMap
 from .reg import make_regset
 from .rules import EndRule
 from .rules import Entry
 from .rules import MatchRule
 from .rules import PatternRule
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/fchainmap.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/fchainmap.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from __future__ import annotations
 
 import json
 import os
 
 from typing import Any
-from typing import Dict
-from typing import FrozenSet
-from typing import List
 from typing import NamedTuple
-from typing import Tuple
 from typing import TypeVar
 
 from .compiler import Compiler
 from .fchainmap import FChainMap
 from .reg import _Reg
 from .reg import make_reg
 from .rules import Rule
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import functools
 import re
 
 from re import Match
 from typing import TYPE_CHECKING
 from typing import Optional
-from typing import Tuple
 
 import onigurumacffi
 
 from .region import Region
 
 
 if TYPE_CHECKING:
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from __future__ import annotations
 
 from re import Match
 from typing import TYPE_CHECKING
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import NamedTuple
 from typing import Optional
-from typing import Tuple
 
 from ._types import Protocol
 from .fchainmap import FChainMap
 from .reg import ERR_REG
 from .reg import _Reg
 from .reg import _RegSet
 from .reg import do_regset
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import NamedTuple
-from typing import Tuple
 
 
 if TYPE_CHECKING:
     from .rules import Entry
     from .rules import WhileRule
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.1.0/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
-from typing import List
-from typing import Tuple
 
 from .region import Region
 from .region import Regions
 from .state import State
 
 
 if TYPE_CHECKING:
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/colorize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/field_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import textwrap
 
 from functools import partial
 
 from ansible_navigator.utils.definitions import ExitMessage
 from ansible_navigator.utils.definitions import ExitMessages
 from ansible_navigator.utils.definitions import ExitPrefix
+
 from ..utils.functions import console_width
 from .colorize import ansi_to_curses
 from .curses_defs import CursesLines
 from .field_checks import FieldChecks
 from .field_curses_information import FieldCursesInformation
 from .field_information import FieldInformation
 from .field_option import FieldOption
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.1.0/src/ansible_navigator/ui_framework/validators.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/dict_merge.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/dot_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/functions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/json_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Functionality to perform json schema validation."""
 from __future__ import annotations
 
 import json
 
+from collections import deque
 from dataclasses import dataclass
 from typing import Any
-from typing import Deque
 
 from jsonschema import SchemaError
 from jsonschema import ValidationError
 from jsonschema.validators import validator_for
 
 from .functions import ExitMessage
 
 
-def to_path(schema_path: Deque[str]):
+def to_path(schema_path: deque):
     """Flatten a path to a dot delimited string.
 
     :param schema_path: The schema path
     :returns: The dot delimited path
     """
     return ".".join(str(index) for index in schema_path)
 
 
-def json_path(absolute_path: Deque[str]):
+def json_path(absolute_path: deque):
     """Flatten a data path to a dot delimited string.
 
     :param absolute_path: The path
     :returns: The dot delimited string
     """
     path = "$"
     for elem in absolute_path:
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/key_value_store.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/settings_file.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.1.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.1.0/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.0.2
+Version: 3.1.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
@@ -70,15 +70,15 @@
 [ansible-core]: https://docs.ansible.com/ansible-core/devel
 [Python venv doc]: https://docs.python.org/3/library/venv.html
 
 Additional `Linux`, `macOS` and `Windows with WSL2` installation
 instructions are available in the [Installation guide].
 
 [Installation guide]:
-https://ansible-navigator.readthedocs.io/en/latest/installation
+https://ansible-navigator.readthedocs.io/installation/
 
 ## Welcome
 
 When running `ansible-navigator` with no arguments, you will be presented with
 the *welcome page*. From this page, you can run playbooks, browse collections,
 explore inventories, read Ansible documentation, and more.
 
@@ -95,15 +95,15 @@
   output to the terminal's standard output stream, as Ansible's commands
   would.
 
 The **interactive** mode is the default and this default can be overwritten by
 passing `--mode stdout` (`-m stdout`) or setting `mode` in
 [configuration][settings documentation].
 
-[settings documentation]: https://ansible-navigator.readthedocs.io/en/latest/settings
+[settings documentation]: https://ansible-navigator.readthedocs.io/settings/
 
 ## Example commands
 
 All of ansible-navigator's features can be accessed from the *welcome page*
 described above, but as a shortcut, commands can also be provided directly as
 command-line arguments.
 
@@ -126,15 +126,15 @@
   `ansible-navigator config dump -m stdout`
 * Show documentation: `ansible-navigator doc sudo -t become  -m stdout`
 
 ... and so on. A full list of subcommands and their relation to Ansible
 commands can be found in the [subcommand documentation].
 
 [subcommand documentation]:
-https://ansible-navigator.readthedocs.io/en/latest/subcommands
+https://ansible-navigator.readthedocs.io/subcommands/
 
 ## Configuring ansible-navigator
 
 There are several ways to configure ansible-navigator and users and projects
 are free to choose the most convenient method for them. The full hierarchy of
 how various configuration sources are applied can be found in the FAQ mentioned
 below.
@@ -146,15 +146,15 @@
 
 ## Frequently Asked Questions (FAQ)
 
 We maintain a [list of common questions][FAQ] which provides a good
 resource to check if something is tripping you up. We also encourage additions
 to this document for the greater community!
 
-[FAQ]: https://ansible-navigator.readthedocs.io/en/latest/faq
+[FAQ]: https://ansible-navigator.readthedocs.io/faq/
 
 ## License
 
 ansible-navigator is released under the Apache License version 2. See the
 [LICENSE] file for more details.
 
 [LICENSE]: https://github.com/ansible/ansible-navigator/blob/main/LICENSE
```

### Comparing `ansible-navigator-3.0.2/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.1.0/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.0.2/tox.ini` & `ansible-navigator-3.1.0/tox.ini`

 * *Files identical despite different names*

