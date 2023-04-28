# Comparing `tmp/nf-core-2.7.2.tar.gz` & `tmp/nf-core-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nf-core-2.7.2.tar", last modified: Mon Dec 19 12:04:16 2022, max compression
+gzip compressed data, was "nf-core-2.8.tar", last modified: Fri Apr 28 14:12:19 2023, max compression
```

## Comparing `nf-core-2.7.2.tar` & `nf-core-2.8.tar`

### file list

```diff
@@ -1,263 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-19 12:03:43.000000 nf-core-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-19 12:03:43.000000 nf-core-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    64585 2022-12-19 12:04:16.000000 nf-core-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    64156 2022-12-19 12:03:43.000000 nf-core-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/.pre-commit-prettier-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55034 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/bump_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/components_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/components_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/components_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/components_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    46181 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/components/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    23606 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)    37161 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/licences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/lint/
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/actions_awsfulltest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/actions_awstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/actions_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/actions_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/files_exist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/files_unchanged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/merge_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/modules_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/multiqc_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/nextflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/pipeline_name_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/pipeline_todos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/schema_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/schema_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/schema_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/template_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint/version_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/lint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17244 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/module-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/module-template/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/module-template/modules/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/module-template/modules/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/module-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/module-template/tests/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/module-template/tests/nextflow.config
--rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/module-template/tests/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/bump_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/modules/lint/
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22345 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/main_nf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/meta_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/module_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/module_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/module_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/module_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/module_todos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/lint/module_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18275 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/modules_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)    53634 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    20047 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/modules_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/modules_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/modules_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/mulled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/nfcore_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    15723 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/test_yml_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/.dockstore.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/awsfulltest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/awstest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/branch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/fix-linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/linting_comment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      918 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.nf-core.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      373 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/CITATIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/adaptivecard.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/email_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/email_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/methods_description_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/multiqc_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/samplesheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/schema_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/sendmail_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/assets/slackreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9573 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/bin/check_samplesheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/conf/base.config
--rw-r--r--   0 runner    (1001) docker     (123)    35028 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/conf/igenomes.config
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/conf/modules.config
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/conf/test.config
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/conf/test_full.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23458 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    33918 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    55769 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/output.md
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    21971 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/NfcoreSchema.groovy
--rwxr-xr-x   0 runner    (1001) docker     (123)    16592 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/NfcoreTemplate.groovy
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/Utils.groovy
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/WorkflowMain.groovy
--rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/WorkflowPipeline.groovy
--rw-r--r--   0 runner    (1001) docker     (123)  2291171 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/main.nf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/local/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/local/samplesheet_check.nf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/fastqc/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/multiqc/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/modules.json
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/nextflow.config
--rw-r--r--   0 runner    (1001) docker     (123)    16048 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/nextflow_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/subworkflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/subworkflows/local/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/subworkflows/local/input_check.nf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/pipeline-template/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/pipeline-template/workflows/pipeline.nf
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/refgenie.py
--rw-r--r--   0 runner    (1001) docker     (123)    37324 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/subworkflow-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/subworkflow-template/subworkflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflow-template/subworkflows/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflow-template/subworkflows/meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/subworkflow-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflow-template/tests/main.nf
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflow-template/tests/nextflow.config
--rw-r--r--   0 runner    (1001) docker     (123)      621 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflow-template/tests/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core/subworkflows/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/subworkflows_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16622 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/test_yml_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/subworkflows/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    41350 2022-12-19 12:03:43.000000 nf-core-2.7.2/nf_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    64585 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 12:03:48.000000 nf-core-2.7.2/nf_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      258 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-19 12:04:16.000000 nf-core-2.7.2/nf_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-19 12:03:43.000000 nf-core-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2022-12-19 12:03:43.000000 nf-core-2.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 12:04:16.000000 nf-core-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-19 12:03:43.000000 nf-core-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/tests/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/actions_awsfulltest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/actions_awstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/actions_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/actions_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/files_exist.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/files_unchanged.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/merge_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/nextflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/lint/version_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/bump_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/create_test_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/modules_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/modules_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 12:04:16.000000 nf-core-2.7.2/tests/subworkflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/subworkflows_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15466 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/subworkflows/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    25709 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_lint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_mulled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_refgenie.py
--rw-r--r--   0 runner    (1001) docker     (123)    20207 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_subworkflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    17732 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2022-12-19 12:03:43.000000 nf-core-2.7.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.062879 nf-core-2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-28 14:11:53.000000 nf-core-2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 14:11:53.000000 nf-core-2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    65673 2023-04-28 14:12:19.062879 nf-core-2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    65246 2023-04-28 14:11:53.000000 nf-core-2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.026879 nf-core-2.8/nf_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/.pre-commit-prettier-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53727 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.030879 nf-core-2.8/nf_core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/components_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/components_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/components_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/components/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23874 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37152 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31865 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/licences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.034879 nf-core-2.8/nf_core/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)    23357 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_awsfulltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_awstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/actions_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/files_exist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/files_unchanged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/merge_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/modules_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/multiqc_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/nextflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/pipeline_name_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/pipeline_todos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/schema_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/schema_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/schema_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/system_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/template_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint/version_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/lint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/module-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.034879 nf-core-2.8/nf_core/module-template/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/modules/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/modules/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.034879 nf-core-2.8/nf_core/module-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/tests/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/tests/nextflow.config
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/module-template/tests/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.038879 nf-core-2.8/nf_core/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/bump_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/modules/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24400 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/main_nf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/meta_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_todos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/lint/module_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54053 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/modules_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/nfcore_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15466 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/test_yml_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/.dockstore.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.046879 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/awsfulltest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/awstest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/branch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/clean-up.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/fix-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting_comment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.nf-core.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/CITATIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/adaptivecard.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/email_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/email_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/methods_description_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/multiqc_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/samplesheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/schema_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/sendmail_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/assets/slackreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9429 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/bin/check_samplesheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/base.config
+-rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/igenomes.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/modules.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/conf/test_full.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23458 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33918 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55769 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/output.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.050879 nf-core-2.8/nf_core/pipeline-template/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22038 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/NfcoreSchema.groovy
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16592 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/NfcoreTemplate.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/Utils.groovy
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3876 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/WorkflowMain.groovy
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3625 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/WorkflowPipeline.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)  2291171 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/main.nf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/local/samplesheet_check.nf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/modules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/nextflow.config
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/nextflow_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/pipeline-template/subworkflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/subworkflows/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/subworkflows/local/input_check.nf
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/tower.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/pipeline-template/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/pipeline-template/workflows/pipeline.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/refgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37926 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.022879 nf-core-2.8/nf_core/subworkflow-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/subworkflow-template/subworkflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/subworkflows/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/subworkflows/meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.054879 nf-core-2.8/nf_core/subworkflow-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/tests/main.nf
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/tests/nextflow.config
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflow-template/tests/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.058879 nf-core-2.8/nf_core/subworkflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/subworkflows_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/test_yml_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/subworkflows/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41429 2023-04-28 14:11:53.000000 nf-core-2.8/nf_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.026879 nf-core-2.8/nf_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    65673 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-04-28 14:12:19.000000 nf-core-2.8/nf_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:12:00.000000 nf-core-2.8/nf_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 14:12:18.000000 nf-core-2.8/nf_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 14:11:53.000000 nf-core-2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 14:11:53.000000 nf-core-2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:12:19.062879 nf-core-2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 14:11:53.000000 nf-core-2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.058879 nf-core-2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.058879 nf-core-2.8/tests/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_awsfulltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_awstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/actions_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/files_exist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/files_unchanged.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/merge_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/nextflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 14:11:53.000000 nf-core-2.8/tests/lint/version_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.062879 nf-core-2.8/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/bump_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/create_test_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/modules_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16521 2023-04-28 14:11:53.000000 nf-core-2.8/tests/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:12:19.062879 nf-core-2.8/tests/subworkflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/create_test_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/subworkflows_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-04-28 14:11:53.000000 nf-core-2.8/tests/subworkflows/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_lint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_refgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_subworkflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17732 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-28 14:11:53.000000 nf-core-2.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-28 14:11:53.000000 nf-core-2.8/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nf-core-2.7.2/LICENSE` & `nf-core-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/PKG-INFO` & `nf-core-2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nf-core
-Version: 2.7.2
+Version: 2.8
 Summary: Helper tools for use with nf-core Nextflow pipelines.
 Home-page: https://github.com/nf-core/tools
 Author: Phil Ewels
 Author-email: phil.ewels@scilifelab.se
 License: MIT
 Keywords: nf-core,nextflow,bioinformatics,workflow,pipeline,biology,sequencing,NGS,next generation sequencing
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![nf-core/tools](docs/images/nfcore-tools_logo_light.png#gh-light-mode-only) ![nf-core/tools](docs/images/nfcore-tools_logo_dark.png#gh-dark-mode-only) <!-- omit in toc -->
 
 [![Python tests](https://github.com/nf-core/tools/workflows/Python%20tests/badge.svg?branch=master&event=push)](https://github.com/nf-core/tools/actions?query=workflow%3A%22Python+tests%22+branch%3Amaster)
 [![codecov](https://codecov.io/gh/nf-core/tools/branch/master/graph/badge.svg)](https://codecov.io/gh/nf-core/tools)
@@ -51,15 +51,14 @@
   - [`modules remove` - Remove a module from a pipeline](#remove-a-module-from-a-pipeline)
   - [`modules patch` - Create a patch file for a module](#create-a-patch-file-for-a-module)
   - [`modules create` - Create a module from the template](#create-a-new-module)
   - [`modules create-test-yml` - Create the `test.yml` file for a module](#create-a-module-test-config-file)
   - [`modules lint` - Check a module against nf-core guidelines](#check-a-module-against-nf-core-guidelines)
   - [`modules test` - Run the tests for a module](#run-the-tests-for-a-module-using-pytest)
   - [`modules bump-versions` - Bump software versions of modules](#bump-bioconda-and-container-versions-of-modules-in)
-  - [`modules mulled` - Generate the name for a multi-tool container image](#generate-the-name-for-a-multi-tool-container-image)
 
 - [`nf-core subworkflows` - commands for dealing with subworkflows](#subworkflows)
   - [`subworkflows list` - List available subworkflows](#list-subworkflows)
     - [`subworkflows list remote` - List remote subworkflows](#list-remote-subworkflows)
     - [`subworkflows list local` - List installed subworkflows](#list-installed-subworkflows)
   - [`subworkflows info` - Show information about a subworkflow](#show-information-about-a-subworkflow)
   - [`subworkflows install` - Install subworkflows in a pipeline](#install-subworkflows-in-a-pipeline)
@@ -353,14 +352,16 @@
 
 You can run the pipeline by simply providing the directory path for the `workflow` folder to your `nextflow run` command:
 
 ```bash
 nextflow run /path/to/download/nf-core-rnaseq-dev/workflow/ --input mydata.csv --outdir results  # usual parameters here
 ```
 
+> Note that if you downloaded singularity images, you will need to use `-profile singularity` or have it enabled in your config file.
+
 ### Downloaded nf-core configs
 
 The pipeline files are automatically updated (`params.custom_config_base` is set to `../configs`), so that the local copy of institutional configs are available when running the pipeline.
 So using `-profile <NAME>` should work if available within [nf-core/configs](https://github.com/nf-core/configs).
 
 ### Downloading singularity containers
 
@@ -394,15 +395,15 @@
 The Singularity image download finds containers using two methods:
 
 1. It runs `nextflow config` on the downloaded workflow to look for a `process.container` statement for the whole pipeline.
    This is the typical method used for DSL1 pipelines.
 2. It scrapes any files it finds with a `.nf` file extension in the workflow `modules` directory for lines
    that look like `container = "xxx"`. This is the typical method for DSL2 pipelines, which have one container per process.
 
-Some DSL2 modules have container addresses for docker (eg. `quay.io/biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
+Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
 Where both are found, the download URL is preferred.
 
 Once a full list of containers is found, they are processed in the following order:
 
 1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` specified)
 2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` is _not_ specified, they are copied to the output directory
 3. If they start with `http` they are downloaded directly within Python (default 4 at a time, you can customise this with `--parallel-downloads`)
@@ -617,34 +618,45 @@
 
 ### Add new parameters to the pipeline schema
 
 If you want to add a parameter to the schema, you first have to add the parameter and its default value to the `nextflow.config` file with the `params` scope. Afterwards, you run the command `nf-core schema build` to add the parameters to your schema and open the graphical interface to easily modify the schema.
 
 The graphical interface is oganzised in groups and within the groups the single parameters are stored. For a better overview you can collapse all groups with the `Collapse groups` button, then your new parameters will be the only remaining one at the bottom of the page. Now you can either create a new group with the `Add group` button or drag and drop the paramters in an existing group. Therefor the group has to be expanded. The group title will be displayed, if you run your pipeline with the `--help` flag and its description apears on the parameter page of your pipeline.
 
-Now you can start to change the parameter itself. The description is a short explanation about the parameter, that apears if you run your pipeline with the `--help` flag. By clicking on the dictionary icon you can add a longer explanation for the parameter page of your pipeline. If you want to specify some conditions for your parameter, like the file extension, you can use the nut icon to open the settings. This menu depends on the `type` you assigned to your parameter. For intergers you can define a min and max value, and for strings the file extension can be specified.
+Now you can start to change the parameter itself. The `ID` of a new parameter should be defined in small letters without whitespaces. The description is a short free text explanation about the parameter, that appears if you run your pipeline with the `--help` flag. By clicking on the dictionary icon you can add a longer explanation for the parameter page of your pipeline. Usually, they contain a small paragraph about the parameter settings or a used datasource, like databases or references. If you want to specify some conditions for your parameter, like the file extension, you can use the nut icon to open the settings. This menu depends on the `type` you assigned to your parameter. For integers you can define a min and max value, and for strings the file extension can be specified.
+
+The `type` field is one of the most important points in your pipeline schema, since it defines the datatype of your input and how it will be interpreted. This allows extensive testing prior to starting the pipeline.
+
+The basic datatypes for a pipeline schema are:
+
+- `string`
+- `number`
+- `integer`
+- `boolean`
+
+For the `string` type you have three different options in the settings (nut icon): `enumerated values`, `pattern` and `format`. The first option, `enumerated values`, allows you to specify a list of specific input values. The list has to be separated with a pipe. The `pattern` and `format` settings can depend on each other. The `format` has to be either a directory or a file path. Depending on the `format` setting selected, specifying the `pattern` setting can be the most efficient and time saving option, especially for `file paths`. The `number` and `integer` types share the same settings. Similarly to `string`, there is an `enumerated values` option with the possibility of specifying a `min` and `max` value. For the `boolean` there is no further settings and the default value is usually `false`. The `boolean` value can be switched to `true` by adding the flag to the command. This parameter type is often used to skip specific sections of a pipeline.
 
-After you filled your schema, click on the `Finished` button in the top rigth corner, this will automatically update your `nextflow_schema.json`. If this is not working you can copy the schema from the graphical interface and paste it in your `nextflow_schema.json` file.
+After filling the schema, click on the `Finished` button in the top right corner, this will automatically update your `nextflow_schema.json`. If this is not working, the schema can be copied from the graphical interface and pasted in your `nextflow_schema.json` file.
 
 ### Update existing pipeline schema
 
-Important for the update of a pipeline schema is, that if you want to change the default value of a parameter, you should change it in the `nextflow.config` file, since the value in the config file overwrites the value in the pipeline schema. To change any other parameter use `nf-core schema build --web-only` to open the graphical interface without rebuilding the pipeline schema. Now, you can change your parameters as mentioned above but keep in mind that changing the parameter datatype is depending on the default value you specified in the `nextflow.config` file.
+It's important to change the default value of a parameter in the `nextflow.config` file first and then in the pipeline schema, because the value in the config file overwrites the value in the pipeline schema. To change any other parameter use `nf-core schema build --web-only` to open the graphical interface without rebuilding the pipeline schema. Now, the parameters can be changed as mentioned above but keep in mind that changing the parameter datatype depends on the default value specified in the `nextflow.config` file.
 
 ### Linting a pipeline schema
 
 The pipeline schema is linted as part of the main pipeline `nf-core lint` command,
 however sometimes it can be useful to quickly check the syntax of the JSONSchema without running a full lint run.
 
-Usage is `nf-core schema lint <schema>`, eg:
+Usage is `nf-core schema lint <schema>` (defaulting to `nextflow_schema.json`), eg:
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
 -->
 
-![`nf-core schema lint nextflow_schema.json`](docs/images/nf-core-schema-lint.svg)
+![`nf-core schema lint`](docs/images/nf-core-schema-lint.svg)
 
 ## Bumping a pipeline version number
 
 When releasing a new version of a nf-core pipeline, version numbers have to be updated in several different places. The helper command `nf-core bump-version` automates this for you to avoid manual errors (and frustration!).
 
 The command uses results from the linting process, so will only work with workflows that pass these tests.
 
@@ -968,25 +980,14 @@
 If you want this module to be updated only to a specific version (or downgraded), you could instead specifiy the version:
 
 ```yaml
 bump-versions:
   star/align: "2.6.1d"
 ```
 
-### Generate the name for a multi-tool container image
-
-When you want to use an image of a multi-tool container and you know the specific dependencies and their versions of that container, for example, by looking them up in the [BioContainers hash.tsv](https://github.com/BioContainers/multi-package-containers/blob/master/combinations/hash.tsv), you can use the `nf-core modules mulled` helper tool. This tool generates the name of a BioContainers mulled image.
-
-<!-- RICH-CODEX
-working_dir: tmp/modules
-after_command: cd ../../ && rm -rf tmp
--->
-
-![`nf-core modules mulled pysam==0.16.0.1 biopython==1.78`](docs/images/nf-core-modules-mulled.svg)
-
 ## Subworkflows
 
 After the launch of nf-core modules, we can provide now also nf-core subworkflows to fully utilize the power of DSL2 modularization.
 Subworkflows are chains of multiple module definitions that can be imported into any pipeline.
 This allows multiple pipelines to use the same code for a the same tasks, and gives a greater degree of reusability and unit testing.
 
 To allow us to test modules and subworkflows together we put the nf-core DSL2 subworkflows into the `subworkflows` directory of the modules repository is at <https://github.com/nf-core/modules>.
@@ -1039,38 +1040,44 @@
 
 #### List installed subworkflows
 
 To list subworkflows installed in a local pipeline directory you can use `nf-core subworkflows list local`. This will list the subworkflows install in the current working directory by default. If you want to specify another directory, use the `--dir <pipeline_dir>` flag.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 head: 25
 -->
 
 ![`nf-core subworkflows list local`](docs/images/nf-core-subworkflows-list-local.svg)
 
 ## Show information about a subworkflow
 
 For quick help about how a subworkflow works, use `nf-core subworkflows info <subworkflow_name>`.
 This shows documentation about the subworkflow on the command line, similar to what's available on the
 [nf-core website](https://nf-co.re/subworkflows).
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows info bam_rseqc`](docs/images/nf-core-subworkflows-info.svg)
 
 ### Install subworkflows in a pipeline
 
 You can install subworkflows from [nf-core/modules](https://github.com/nf-core/modules) in your pipeline using `nf-core subworkflows install`.
 A subworkflow installed this way will be installed to the `./subworkflows/nf-core` directory.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows install bam_rseqc`](docs/images/nf-core-subworkflows-install.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows install` like above or select it from a list of available subworkflows by only running `nf-core subworkflows install`.
 
 There are four additional flags that you can use when installing a subworkflow:
@@ -1082,14 +1089,16 @@
 
 ### Update subworkflows in a pipeline
 
 You can update subworkflows installed from a remote repository in your pipeline using `nf-core subworkflows update`.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows update --all --no-preview`](docs/images/nf-core-subworkflows-update.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows update` like above or select it from the list of available subworkflows by only running `nf-core subworkflows update`.
 
 There are six additional flags that you can use with this command:
@@ -1141,14 +1150,16 @@
 
 ### Remove a subworkflow from a pipeline
 
 To delete a subworkflow from your pipeline, run `nf-core subworkflows remove`.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows remove bam_rseqc`](docs/images/nf-core-subworkflows-remove.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows remove` like above or select it from the list of available subworkflows by only running `nf-core subworkflows remove`. To specify the pipeline directory, use `--dir <pipeline_dir>`.
 
 ### Create a new subworkflow
@@ -1169,41 +1180,41 @@
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core subworkflows create` command will prompt you with the relevant questions in order to create all of the necessary subworkflow files.
 
 <!-- RICH-CODEX
 working_dir: tmp
 before_command: git clone https://github.com/nf-core/modules.git && cd modules
-fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot  --label process_low --meta --force
+fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force
 -->
 
-![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot  --label process_low --meta --force`](docs/images/nf-core-subworkflows-create.svg)
+![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
 
 ### Create a subworkflow test config file
 
 All subworkflows on [nf-core/modules](https://github.com/nf-core/modules) have a strict requirement of being unit tested using minimal test data.
 To help developers build new subworkflows, the `nf-core subworkflows create-test-yml` command automates the creation of the yaml file required to document the output file `md5sum` and other information generated by the testing.
 After you have written a minimal Nextflow script to test your subworkflow in `/tests/subworkflow/<subworkflow_name>/main.nf`, this command will run the tests for you and create the `/tests/subworkflow/<tool>/<subtool>/test.yml` file.
 
 <!-- RICH-CODEX
-working_dir: tmp/subworkflows
+working_dir: tmp/modules
 extra_env:
   PROFILE: 'conda'
 -->
 
 ![`nf-core subworkflows create-test-yml bam_stats_samtools --no-prompts --force`](docs/images/nf-core-subworkflows-create-test.svg)
 
 ### Run the tests for a subworkflow using pytest
 
 To run unit tests of a subworkflow that you have installed or the test created by the command [`nf-core subworkflow create-test-yml`](#create-a-subworkflow-test-config-file), you can use `nf-core subworkflows test` command. This command runs the tests specified in `tests/subworkflows/<subworkflow_name>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
 You can specify the subworkflow name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
-working_dir: tmp/subworkflows
+working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
 -->
 
 ![`nf-core subworkflows test bam_rseqc --no-prompts`](docs/images/nf-core-subworkflows-test.svg)
```

### Comparing `nf-core-2.7.2/README.md` & `nf-core-2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
   - [`modules remove` - Remove a module from a pipeline](#remove-a-module-from-a-pipeline)
   - [`modules patch` - Create a patch file for a module](#create-a-patch-file-for-a-module)
   - [`modules create` - Create a module from the template](#create-a-new-module)
   - [`modules create-test-yml` - Create the `test.yml` file for a module](#create-a-module-test-config-file)
   - [`modules lint` - Check a module against nf-core guidelines](#check-a-module-against-nf-core-guidelines)
   - [`modules test` - Run the tests for a module](#run-the-tests-for-a-module-using-pytest)
   - [`modules bump-versions` - Bump software versions of modules](#bump-bioconda-and-container-versions-of-modules-in)
-  - [`modules mulled` - Generate the name for a multi-tool container image](#generate-the-name-for-a-multi-tool-container-image)
 
 - [`nf-core subworkflows` - commands for dealing with subworkflows](#subworkflows)
   - [`subworkflows list` - List available subworkflows](#list-subworkflows)
     - [`subworkflows list remote` - List remote subworkflows](#list-remote-subworkflows)
     - [`subworkflows list local` - List installed subworkflows](#list-installed-subworkflows)
   - [`subworkflows info` - Show information about a subworkflow](#show-information-about-a-subworkflow)
   - [`subworkflows install` - Install subworkflows in a pipeline](#install-subworkflows-in-a-pipeline)
@@ -340,14 +339,16 @@
 
 You can run the pipeline by simply providing the directory path for the `workflow` folder to your `nextflow run` command:
 
 ```bash
 nextflow run /path/to/download/nf-core-rnaseq-dev/workflow/ --input mydata.csv --outdir results  # usual parameters here
 ```
 
+> Note that if you downloaded singularity images, you will need to use `-profile singularity` or have it enabled in your config file.
+
 ### Downloaded nf-core configs
 
 The pipeline files are automatically updated (`params.custom_config_base` is set to `../configs`), so that the local copy of institutional configs are available when running the pipeline.
 So using `-profile <NAME>` should work if available within [nf-core/configs](https://github.com/nf-core/configs).
 
 ### Downloading singularity containers
 
@@ -381,15 +382,15 @@
 The Singularity image download finds containers using two methods:
 
 1. It runs `nextflow config` on the downloaded workflow to look for a `process.container` statement for the whole pipeline.
    This is the typical method used for DSL1 pipelines.
 2. It scrapes any files it finds with a `.nf` file extension in the workflow `modules` directory for lines
    that look like `container = "xxx"`. This is the typical method for DSL2 pipelines, which have one container per process.
 
-Some DSL2 modules have container addresses for docker (eg. `quay.io/biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
+Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
 Where both are found, the download URL is preferred.
 
 Once a full list of containers is found, they are processed in the following order:
 
 1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` specified)
 2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` is _not_ specified, they are copied to the output directory
 3. If they start with `http` they are downloaded directly within Python (default 4 at a time, you can customise this with `--parallel-downloads`)
@@ -604,34 +605,45 @@
 
 ### Add new parameters to the pipeline schema
 
 If you want to add a parameter to the schema, you first have to add the parameter and its default value to the `nextflow.config` file with the `params` scope. Afterwards, you run the command `nf-core schema build` to add the parameters to your schema and open the graphical interface to easily modify the schema.
 
 The graphical interface is oganzised in groups and within the groups the single parameters are stored. For a better overview you can collapse all groups with the `Collapse groups` button, then your new parameters will be the only remaining one at the bottom of the page. Now you can either create a new group with the `Add group` button or drag and drop the paramters in an existing group. Therefor the group has to be expanded. The group title will be displayed, if you run your pipeline with the `--help` flag and its description apears on the parameter page of your pipeline.
 
-Now you can start to change the parameter itself. The description is a short explanation about the parameter, that apears if you run your pipeline with the `--help` flag. By clicking on the dictionary icon you can add a longer explanation for the parameter page of your pipeline. If you want to specify some conditions for your parameter, like the file extension, you can use the nut icon to open the settings. This menu depends on the `type` you assigned to your parameter. For intergers you can define a min and max value, and for strings the file extension can be specified.
+Now you can start to change the parameter itself. The `ID` of a new parameter should be defined in small letters without whitespaces. The description is a short free text explanation about the parameter, that appears if you run your pipeline with the `--help` flag. By clicking on the dictionary icon you can add a longer explanation for the parameter page of your pipeline. Usually, they contain a small paragraph about the parameter settings or a used datasource, like databases or references. If you want to specify some conditions for your parameter, like the file extension, you can use the nut icon to open the settings. This menu depends on the `type` you assigned to your parameter. For integers you can define a min and max value, and for strings the file extension can be specified.
+
+The `type` field is one of the most important points in your pipeline schema, since it defines the datatype of your input and how it will be interpreted. This allows extensive testing prior to starting the pipeline.
+
+The basic datatypes for a pipeline schema are:
+
+- `string`
+- `number`
+- `integer`
+- `boolean`
+
+For the `string` type you have three different options in the settings (nut icon): `enumerated values`, `pattern` and `format`. The first option, `enumerated values`, allows you to specify a list of specific input values. The list has to be separated with a pipe. The `pattern` and `format` settings can depend on each other. The `format` has to be either a directory or a file path. Depending on the `format` setting selected, specifying the `pattern` setting can be the most efficient and time saving option, especially for `file paths`. The `number` and `integer` types share the same settings. Similarly to `string`, there is an `enumerated values` option with the possibility of specifying a `min` and `max` value. For the `boolean` there is no further settings and the default value is usually `false`. The `boolean` value can be switched to `true` by adding the flag to the command. This parameter type is often used to skip specific sections of a pipeline.
 
-After you filled your schema, click on the `Finished` button in the top rigth corner, this will automatically update your `nextflow_schema.json`. If this is not working you can copy the schema from the graphical interface and paste it in your `nextflow_schema.json` file.
+After filling the schema, click on the `Finished` button in the top right corner, this will automatically update your `nextflow_schema.json`. If this is not working, the schema can be copied from the graphical interface and pasted in your `nextflow_schema.json` file.
 
 ### Update existing pipeline schema
 
-Important for the update of a pipeline schema is, that if you want to change the default value of a parameter, you should change it in the `nextflow.config` file, since the value in the config file overwrites the value in the pipeline schema. To change any other parameter use `nf-core schema build --web-only` to open the graphical interface without rebuilding the pipeline schema. Now, you can change your parameters as mentioned above but keep in mind that changing the parameter datatype is depending on the default value you specified in the `nextflow.config` file.
+It's important to change the default value of a parameter in the `nextflow.config` file first and then in the pipeline schema, because the value in the config file overwrites the value in the pipeline schema. To change any other parameter use `nf-core schema build --web-only` to open the graphical interface without rebuilding the pipeline schema. Now, the parameters can be changed as mentioned above but keep in mind that changing the parameter datatype depends on the default value specified in the `nextflow.config` file.
 
 ### Linting a pipeline schema
 
 The pipeline schema is linted as part of the main pipeline `nf-core lint` command,
 however sometimes it can be useful to quickly check the syntax of the JSONSchema without running a full lint run.
 
-Usage is `nf-core schema lint <schema>`, eg:
+Usage is `nf-core schema lint <schema>` (defaulting to `nextflow_schema.json`), eg:
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
 -->
 
-![`nf-core schema lint nextflow_schema.json`](docs/images/nf-core-schema-lint.svg)
+![`nf-core schema lint`](docs/images/nf-core-schema-lint.svg)
 
 ## Bumping a pipeline version number
 
 When releasing a new version of a nf-core pipeline, version numbers have to be updated in several different places. The helper command `nf-core bump-version` automates this for you to avoid manual errors (and frustration!).
 
 The command uses results from the linting process, so will only work with workflows that pass these tests.
 
@@ -955,25 +967,14 @@
 If you want this module to be updated only to a specific version (or downgraded), you could instead specifiy the version:
 
 ```yaml
 bump-versions:
   star/align: "2.6.1d"
 ```
 
-### Generate the name for a multi-tool container image
-
-When you want to use an image of a multi-tool container and you know the specific dependencies and their versions of that container, for example, by looking them up in the [BioContainers hash.tsv](https://github.com/BioContainers/multi-package-containers/blob/master/combinations/hash.tsv), you can use the `nf-core modules mulled` helper tool. This tool generates the name of a BioContainers mulled image.
-
-<!-- RICH-CODEX
-working_dir: tmp/modules
-after_command: cd ../../ && rm -rf tmp
--->
-
-![`nf-core modules mulled pysam==0.16.0.1 biopython==1.78`](docs/images/nf-core-modules-mulled.svg)
-
 ## Subworkflows
 
 After the launch of nf-core modules, we can provide now also nf-core subworkflows to fully utilize the power of DSL2 modularization.
 Subworkflows are chains of multiple module definitions that can be imported into any pipeline.
 This allows multiple pipelines to use the same code for a the same tasks, and gives a greater degree of reusability and unit testing.
 
 To allow us to test modules and subworkflows together we put the nf-core DSL2 subworkflows into the `subworkflows` directory of the modules repository is at <https://github.com/nf-core/modules>.
@@ -1026,38 +1027,44 @@
 
 #### List installed subworkflows
 
 To list subworkflows installed in a local pipeline directory you can use `nf-core subworkflows list local`. This will list the subworkflows install in the current working directory by default. If you want to specify another directory, use the `--dir <pipeline_dir>` flag.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 head: 25
 -->
 
 ![`nf-core subworkflows list local`](docs/images/nf-core-subworkflows-list-local.svg)
 
 ## Show information about a subworkflow
 
 For quick help about how a subworkflow works, use `nf-core subworkflows info <subworkflow_name>`.
 This shows documentation about the subworkflow on the command line, similar to what's available on the
 [nf-core website](https://nf-co.re/subworkflows).
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows info bam_rseqc`](docs/images/nf-core-subworkflows-info.svg)
 
 ### Install subworkflows in a pipeline
 
 You can install subworkflows from [nf-core/modules](https://github.com/nf-core/modules) in your pipeline using `nf-core subworkflows install`.
 A subworkflow installed this way will be installed to the `./subworkflows/nf-core` directory.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows install bam_rseqc`](docs/images/nf-core-subworkflows-install.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows install` like above or select it from a list of available subworkflows by only running `nf-core subworkflows install`.
 
 There are four additional flags that you can use when installing a subworkflow:
@@ -1069,14 +1076,16 @@
 
 ### Update subworkflows in a pipeline
 
 You can update subworkflows installed from a remote repository in your pipeline using `nf-core subworkflows update`.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows update --all --no-preview`](docs/images/nf-core-subworkflows-update.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows update` like above or select it from the list of available subworkflows by only running `nf-core subworkflows update`.
 
 There are six additional flags that you can use with this command:
@@ -1128,14 +1137,16 @@
 
 ### Remove a subworkflow from a pipeline
 
 To delete a subworkflow from your pipeline, run `nf-core subworkflows remove`.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows remove bam_rseqc`](docs/images/nf-core-subworkflows-remove.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows remove` like above or select it from the list of available subworkflows by only running `nf-core subworkflows remove`. To specify the pipeline directory, use `--dir <pipeline_dir>`.
 
 ### Create a new subworkflow
@@ -1156,41 +1167,41 @@
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core subworkflows create` command will prompt you with the relevant questions in order to create all of the necessary subworkflow files.
 
 <!-- RICH-CODEX
 working_dir: tmp
 before_command: git clone https://github.com/nf-core/modules.git && cd modules
-fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot  --label process_low --meta --force
+fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force
 -->
 
-![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot  --label process_low --meta --force`](docs/images/nf-core-subworkflows-create.svg)
+![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
 
 ### Create a subworkflow test config file
 
 All subworkflows on [nf-core/modules](https://github.com/nf-core/modules) have a strict requirement of being unit tested using minimal test data.
 To help developers build new subworkflows, the `nf-core subworkflows create-test-yml` command automates the creation of the yaml file required to document the output file `md5sum` and other information generated by the testing.
 After you have written a minimal Nextflow script to test your subworkflow in `/tests/subworkflow/<subworkflow_name>/main.nf`, this command will run the tests for you and create the `/tests/subworkflow/<tool>/<subtool>/test.yml` file.
 
 <!-- RICH-CODEX
-working_dir: tmp/subworkflows
+working_dir: tmp/modules
 extra_env:
   PROFILE: 'conda'
 -->
 
 ![`nf-core subworkflows create-test-yml bam_stats_samtools --no-prompts --force`](docs/images/nf-core-subworkflows-create-test.svg)
 
 ### Run the tests for a subworkflow using pytest
 
 To run unit tests of a subworkflow that you have installed or the test created by the command [`nf-core subworkflow create-test-yml`](#create-a-subworkflow-test-config-file), you can use `nf-core subworkflows test` command. This command runs the tests specified in `tests/subworkflows/<subworkflow_name>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
 You can specify the subworkflow name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
-working_dir: tmp/subworkflows
+working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
 -->
 
 ![`nf-core subworkflows test bam_rseqc --no-prompts`](docs/images/nf-core-subworkflows-test.svg)
```

### Comparing `nf-core-2.7.2/nf_core/__main__.py` & `nf-core-2.8/nf_core/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "nf-core modules": [
         {
             "name": "For pipelines",
             "commands": ["list", "info", "install", "update", "remove", "patch"],
         },
         {
             "name": "Developing new modules",
-            "commands": ["create", "create-test-yml", "lint", "bump-versions", "mulled", "test"],
+            "commands": ["create", "create-test-yml", "lint", "bump-versions", "test"],
         },
     ],
     "nf-core subworkflows": [
         {
             "name": "For pipelines",
             "commands": ["info", "install", "list", "remove", "update"],
         },
@@ -337,15 +337,15 @@
     """
     Check pipeline code against nf-core guidelines.
 
     Runs a large number of automated tests to ensure that the supplied pipeline
     meets the nf-core guidelines. Documentation of all lint tests can be found
     on the nf-core website: [link=https://nf-co.re/tools-docs/]https://nf-co.re/tools-docs/[/]
 
-    You can ignore tests using a file called [blue].nf-core-lint.yaml[/] [i](if you have a good reason!)[/].
+    You can ignore tests using a file called [blue].nf-core.yml[/] [i](if you have a good reason!)[/].
     See the documentation for details.
     """
 
     # Check if pipeline directory is a pipeline
     try:
         nf_core.utils.is_pipeline_directory(dir)
     except UserWarning as e:
@@ -614,29 +614,33 @@
 @click.option(
     "-d",
     "--dir",
     type=click.Path(exists=True),
     default=".",
     help=r"Pipeline directory. [dim]\[default: current working directory][/]",
 )
-def patch(ctx, tool, dir):
+@click.option("-r", "--remove", is_flag=True, default=False)
+def patch(ctx, tool, dir, remove):
     """
     Create a patch file for minor changes in a module
 
     Checks if a module has been modified locally and creates a patch file
     describing how the module has changed from the remote version
     """
     try:
         module_patch = nf_core.modules.ModulePatch(
             dir,
             ctx.obj["modules_repo_url"],
             ctx.obj["modules_repo_branch"],
             ctx.obj["modules_repo_no_pull"],
         )
-        module_patch.patch(tool)
+        if remove:
+            module_patch.remove(tool)
+        else:
+            module_patch.patch(tool)
     except (UserWarning, LookupError) as e:
         log.error(e)
         sys.exit(1)
 
 
 # nf-core modules remove
 @modules.command()
@@ -674,15 +678,24 @@
 @click.option("-a", "--author", type=str, metavar="<author>", help="Module author's GitHub username prefixed with '@'")
 @click.option("-l", "--label", type=str, metavar="<process label>", help="Standard resource label for process")
 @click.option("-m", "--meta", is_flag=True, default=False, help="Use Groovy meta map for sample information")
 @click.option("-n", "--no-meta", is_flag=True, default=False, help="Don't use meta map for sample information")
 @click.option("-f", "--force", is_flag=True, default=False, help="Overwrite any files if they already exist")
 @click.option("-c", "--conda-name", type=str, default=None, help="Name of the conda package to use")
 @click.option("-p", "--conda-package-version", type=str, default=None, help="Version of conda package to use")
-def create_module(ctx, tool, dir, author, label, meta, no_meta, force, conda_name, conda_package_version):
+@click.option(
+    "-i",
+    "--empty-template",
+    is_flag=True,
+    default=False,
+    help="Create a module from the template without TODOs or examples",
+)
+def create_module(
+    ctx, tool, dir, author, label, meta, no_meta, force, conda_name, conda_package_version, empty_template
+):
     """
     Create a new DSL2 module from the nf-core template.
 
     If the specified directory is a pipeline, this function creates a file called
     'modules/local/tool_subtool.nf'
 
     If the specified directory is a clone of nf-core/modules, it creates or modifies files
@@ -696,15 +709,15 @@
         has_meta = True
     elif no_meta:
         has_meta = False
 
     # Run function
     try:
         module_create = nf_core.modules.ModuleCreate(
-            dir, tool, author, label, has_meta, force, conda_name, conda_package_version
+            dir, tool, author, label, has_meta, force, conda_name, conda_package_version, empty_template
         )
         module_create.create()
     except UserWarning as e:
         log.critical(e)
         sys.exit(1)
     except LookupError as e:
         log.error(e)
@@ -862,57 +875,14 @@
         log.error(e)
         sys.exit(1)
     except (UserWarning, LookupError) as e:
         log.critical(e)
         sys.exit(1)
 
 
-# nf-core modules mulled
-@modules.command()
-@click.argument("specifications", required=True, nargs=-1, metavar="<tool==version> <...>")
-@click.option(
-    "--build-number",
-    type=int,
-    default=0,
-    show_default=True,
-    metavar="<number>",
-    help="The build number for this image. This is an incremental value that starts at zero.",
-)
-def mulled(specifications, build_number):
-    """
-    Generate the name of a BioContainers mulled image version 2.
-
-    When you know the specific dependencies and their versions of a multi-tool container image and you need the name of
-    that image, this command can generate it for you.
-
-    """
-    from nf_core.modules.mulled import MulledImageNameGenerator
-
-    try:
-        image_name = MulledImageNameGenerator.generate_image_name(
-            MulledImageNameGenerator.parse_targets(specifications), build_number=build_number
-        )
-    except ValueError as e:
-        log.error(e)
-        sys.exit(1)
-    if not MulledImageNameGenerator.image_exists(image_name):
-        log.error("The generated multi-tool container image name does not seem to exist yet.")
-        log.info(
-            "Please double check that your provided combination of tools and versions exists in the file: "
-            "[link=https://github.com/BioContainers/multi-package-containers/blob/master/combinations/hash.tsv]BioContainers/multi-package-containers 'combinations/hash.tsv'[/link]"
-        )
-        log.info(
-            "If it does not, please add your desired combination as detailed at: "
-            "https://github.com/BioContainers/multi-package-containers"
-        )
-        sys.exit(1)
-    log.info("Mulled container hash:")
-    stdout.print(image_name)
-
-
 # nf-core modules test
 @modules.command("test")
 @click.pass_context
 @click.argument("tool", type=str, required=False, metavar="<tool> or <tool/subtool>")
 @click.option("-p", "--no-prompts", is_flag=True, default=False, help="Use defaults without prompting")
 @click.option("-a", "--pytest_args", type=str, required=False, multiple=True, help="Additional pytest arguments")
 def test_module(ctx, tool, no_prompts, pytest_args):
@@ -1385,24 +1355,28 @@
     except (UserWarning, AssertionError) as e:
         log.error(e)
         sys.exit(1)
 
 
 # nf-core schema lint
 @schema.command()
-@click.argument("schema_path", type=click.Path(exists=True), required=True, metavar="<pipeline schema>")
+@click.argument(
+    "schema_path", type=click.Path(exists=True), default="nextflow_schema.json", metavar="<pipeline schema>"
+)
 def lint(schema_path):
     """
     Check that a given pipeline schema is valid.
 
     Checks whether the pipeline schema validates as JSON Schema Draft 7
     and adheres to the additional nf-core schema requirements.
 
     This function runs as part of the nf-core lint command, this is a convenience
     command that does just the schema linting nice and quickly.
+
+    If no schema path is provided, "nextflow_schema.json" will be used (if it exists).
     """
     schema_obj = nf_core.schema.PipelineSchema()
     try:
         schema_obj.get_schema_path(schema_path)
         schema_obj.load_lint_schema()
         # Validate title and description - just warnings as schema should still work fine
         try:
@@ -1442,16 +1416,15 @@
         log.error("Could not find 'nextflow_schema.json' in current directory. Please specify a path.")
         sys.exit(1)
 
     schema_obj = nf_core.schema.PipelineSchema()
     # Assume we're in a pipeline dir root if schema path not set
     schema_obj.get_schema_path(schema_path)
     schema_obj.load_schema()
-    if not output:
-        stdout.print(schema_obj.print_documentation(output, format, force, columns.split(",")))
+    schema_obj.print_documentation(output, format, force, columns.split(","))
 
 
 # nf-core bump-version
 @nf_core_cli.command("bump-version")
 @click.argument("new_version", required=True, metavar="<new version>")
 @click.option(
     "-d",
```

### Comparing `nf-core-2.7.2/nf_core/bump_version.py` & `nf-core-2.8/nf_core/bump_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,20 +129,18 @@
             content = fh.read()
     except FileNotFoundError:
         log.warning(f"File not found: '{fn}'")
         return
 
     replacements = []
     for pattern in patterns:
-
         found_match = False
 
         newcontent = []
         for line in content.splitlines():
-
             # Match the pattern
             matches_pattern = re.findall(rf"^.*{pattern[0]}.*$", line)
             if matches_pattern:
                 found_match = True
 
                 # Replace the match
                 newline = re.sub(pattern[0], pattern[1], line)
```

### Comparing `nf-core-2.7.2/nf_core/components/components_command.py` & `nf-core-2.8/nf_core/components/components_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import mmap
 import os
 import shutil
 from pathlib import Path
 
 import yaml
 
+import nf_core.utils
 from nf_core.modules.modules_json import ModulesJson
 from nf_core.modules.modules_repo import ModulesRepo
 
 from .components_utils import get_repo_info
 
 log = logging.getLogger(__name__)
 
@@ -158,32 +159,21 @@
             (bool): Whether the operation was successful of not
         """
         return modules_repo.install_component(component_name, install_dir, component_version, self.component_type)
 
     def load_lint_config(self):
         """Parse a pipeline lint config file.
 
-        Look for a file called either `.nf-core-lint.yml` or
-        `.nf-core-lint.yaml` in the pipeline root directory and parse it.
-        (`.yml` takes precedence).
+        Load the '.nf-core.yml'  config file and extract
+        the lint config from it
 
         Add parsed config to the `self.lint_config` class attribute.
         """
-        config_fn = os.path.join(self.dir, ".nf-core-lint.yml")
-
-        # Pick up the file if it's .yaml instead of .yml
-        if not os.path.isfile(config_fn):
-            config_fn = os.path.join(self.dir, ".nf-core-lint.yaml")
-
-        # Load the YAML
-        try:
-            with open(config_fn, "r") as fh:
-                self.lint_config = yaml.safe_load(fh)
-        except FileNotFoundError:
-            log.debug(f"No lint config file found: {config_fn}")
+        _, tools_config = nf_core.utils.load_tools_config(self.dir)
+        self.lint_config = tools_config.get("lint", {})
 
     def check_modules_structure(self):
         """
         Check that the structure of the modules directory in a pipeline is the correct one:
             modules/nf-core/TOOL/SUBTOOL
 
         Prior to nf-core/tools release 2.6 the directory structure had an additional level of nesting:
```

### Comparing `nf-core-2.7.2/nf_core/components/components_test.py` & `nf-core-2.8/nf_core/components/components_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,13 +176,16 @@
     def _run_pytests(self):
         """Given a module/subworkflow name, run tests."""
         # Print nice divider line
         console = rich.console.Console()
         console.rule(self.component_name, style="black")
 
         # Set pytest arguments
-        command_args = ["--tag", f"{self.component_name}", "--symlink", "--keep-workflow-wd", "--git-aware"]
+        tag = self.component_name
+        if self.component_type == "subworkflows":
+            tag = "subworkflows/" + tag
+        command_args = ["--tag", f"{tag}", "--symlink", "--keep-workflow-wd", "--git-aware"]
         command_args += self.pytest_args
 
         # Run pytest
         log.info(f"Running pytest for {self.component_type[:-1]} '{self.component_name}'")
         sys.exit(pytest.main(command_args))
```

### Comparing `nf-core-2.7.2/nf_core/components/components_utils.py` & `nf-core-2.8/nf_core/components/components_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/components/info.py` & `nf-core-2.8/nf_core/components/info.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import questionary
 import yaml
 from rich import box
 from rich.console import Group
 from rich.markdown import Markdown
 from rich.panel import Panel
+from rich.syntax import Syntax
 from rich.table import Table
 from rich.text import Text
 
 import nf_core.utils
 from nf_core.components.components_command import ComponentCommand
 from nf_core.modules.modules_json import ModulesJson
 from nf_core.modules.modules_repo import NF_CORE_MODULES_REMOTE
@@ -124,14 +125,27 @@
             while component not in components:
                 log.info(f"'{component}' is not a valid {self.component_type[:-1]} name")
                 component = questionary.autocomplete(
                     f"Please select a new {self.component_type[:-1]}",
                     choices=components,
                     style=nf_core.utils.nfcore_question_style,
                 ).unsafe_ask()
+        else:
+            if self.repo_type == "pipeline":
+                # check if the module is locally installed
+                local_paths = self.modules_json.get_all_components(self.component_type).get(
+                    self.modules_repo.remote_url, {}
+                )
+                for directory, comp in local_paths:
+                    if comp == component:
+                        component_base_path = Path(self.dir, self.component_type)
+                        self.local_path = Path(component_base_path, directory, component)
+                        break
+                if self.local_path:
+                    self.local = True
 
         return component
 
     def get_component_info(self):
         """Given the name of a module/subworkflow, parse meta.yml and print usage help."""
 
         # Running with a local install, try to find the local meta
@@ -279,16 +293,41 @@
                         Markdown(info["description"] if info["description"] else ""),
                         info.get("pattern", ""),
                     )
 
             renderables.append(outputs_table)
 
         # Installation command
-        if self.remote_location:
+        if self.remote_location and not self.local:
             cmd_base = f"nf-core {self.component_type}"
             if self.remote_location != NF_CORE_MODULES_REMOTE:
                 cmd_base = f"nf-core {self.component_type} --git-remote {self.remote_location}"
             renderables.append(
                 Text.from_markup(f"\n :computer:  Installation command: [magenta]{cmd_base} install {self.component}\n")
             )
 
+        # Print include statement
+        if self.local_path:
+            install_folder = Path(self.dir, self.component_type, self.modules_repo.repo_path)
+            component_name = "_".join(self.component.upper().split("/"))
+            renderables.append(
+                Text.from_markup(f"\n [blue]Use the following statement to include this {self.component_type[:-1]}:")
+            )
+            renderables.append(
+                Syntax(
+                    f"include {{ {component_name} }} from '../{Path(install_folder, self.component).relative_to(self.dir)}/main'",
+                    "groovy",
+                    theme="ansi_dark",
+                    padding=1,
+                )
+            )
+            if self.component_type == "subworkflows":
+                subworkflow_config = Path(install_folder, self.component, "nextflow.config").relative_to(self.dir)
+                if os.path.isfile(subworkflow_config):
+                    renderables.append(
+                        Text.from_markup("\n [blue]Add the following config statement to use this subworkflow:")
+                    )
+                    renderables.append(
+                        Syntax(f"includeConfig '{subworkflow_config}'", "groovy", theme="ansi_dark", padding=1)
+                    )
+
         return Group(*renderables)
```

### Comparing `nf-core-2.7.2/nf_core/components/install.py` & `nf-core-2.8/nf_core/components/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import re
 from pathlib import Path
 
 import questionary
 from rich.console import Console
 from rich.syntax import Syntax
 
 import nf_core.modules.modules_utils
@@ -55,14 +54,20 @@
             self.check_modules_structure()
 
         # Verify that 'modules.json' is consistent with the installed modules and subworkflows
         modules_json = ModulesJson(self.dir)
         if not silent:
             modules_json.check_up_to_date()
 
+        # Verify that the remote repo's org_path does not match the org_path of any alternate repo among the installed modules
+        if self.check_alternate_remotes(modules_json):
+            err_msg = f"You are trying to install {self.component_type} from different repositories with the same organization name '{self.modules_repo.repo_path}' (set in the `.nf-core.yml` file in the `org_path` field).\nThis is not supported, and will likely cause problems. org_path should be set to the github account/organization name."
+            log.error(err_msg)
+            return False
+
         # Verify SHA
         if not self.modules_repo.verify_sha(self.prompt, self.sha):
             return False
 
         # Check and verify component name
         component = self.collect_and_verify_name(component, self.modules_repo)
         if not component:
@@ -70,18 +75,18 @@
 
         # Get current version
         current_version = modules_json.get_component_version(
             self.component_type, component, self.modules_repo.remote_url, self.modules_repo.repo_path
         )
 
         # Set the install folder based on the repository name
-        install_folder = os.path.join(self.dir, self.component_type, self.modules_repo.repo_path)
+        install_folder = Path(self.dir, self.component_type, self.modules_repo.repo_path)
 
         # Compute the component directory
-        component_dir = os.path.join(install_folder, component)
+        component_dir = Path(install_folder, component)
 
         # Check that the component is not already installed
         component_not_installed = self.check_component_installed(
             component, current_version, component_dir, self.modules_repo, self.force, self.prompt, silent
         )
         if not component_not_installed:
             log.debug(
@@ -165,27 +170,27 @@
         """
         Collect component name.
         Check that the supplied name is an available module/subworkflow.
         """
         if component is None:
             component = questionary.autocomplete(
                 f"{'Tool' if self.component_type == 'modules' else 'Subworkflow'} name:",
-                choices=sorted(modules_repo.get_avail_components(self.component_type)),
+                choices=sorted(modules_repo.get_avail_components(self.component_type, commit=self.sha)),
                 style=nf_core.utils.nfcore_question_style,
             ).unsafe_ask()
 
         # Check that the supplied name is an available module/subworkflow
-        if component and component not in modules_repo.get_avail_components(self.component_type):
+        if component and component not in modules_repo.get_avail_components(self.component_type, commit=self.sha):
             log.error(
                 f"{self.component_type[:-1].title()} '{component}' not found in list of available {self.component_type}."
             )
             log.info(f"Use the command 'nf-core {self.component_type} list' to view available software")
             return False
 
-        if not modules_repo.component_exists(component, self.component_type):
+        if not modules_repo.component_exists(component, self.component_type, commit=self.sha):
             warn_msg = f"{self.component_type[:-1].title()} '{component}' not found in remote '{modules_repo.remote_url}' ({modules_repo.branch})"
             log.warning(warn_msg)
             return False
 
         return component
 
     def check_component_installed(self, component, current_version, component_dir, modules_repo, force, prompt, silent):
@@ -261,7 +266,24 @@
                         log.debug(
                             f"Removing {self.component_type[:-1]} '{modules_repo.repo_path}/{component}' from repo '{repo_to_remove}' from modules.json."
                         )
                         modules_json.remove_entry(
                             self.component_type, component, repo_to_remove, modules_repo.repo_path
                         )
                         return component_values["installed_by"]
+
+    def check_alternate_remotes(self, modules_json):
+        """
+        Check whether there are previously installed components with the same org_path but different remote urls
+        Log error if multiple remotes exist.
+
+        Return:
+            True: if problematic components are found
+            False: if problematic components are not found
+        """
+        modules_json.load()
+        for repo_url, repo_content in modules_json.modules_json.get("repos", dict()).items():
+            for component_type in repo_content:
+                for dir in repo_content.get(component_type, dict()).keys():
+                    if dir == self.modules_repo.repo_path and repo_url != self.modules_repo.remote_url:
+                        return True
+        return False
```

### Comparing `nf-core-2.7.2/nf_core/components/list.py` & `nf-core-2.8/nf_core/components/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/components/remove.py` & `nf-core-2.8/nf_core/components/remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                         style=nf_core.utils.nfcore_question_style,
                     ).unsafe_ask():
                         # add the component back to modules.json
                         if not ComponentInstall(self.dir, self.component_type, force=True).install(
                             component, silent=True
                         ):
                             log.warning(
-                                f"Could not install the {self.component_type[:-1]} '{component}', please install it manually with 'nf-core {component_type} install  {component}'."
+                                f"Could not install the {self.component_type[:-1]} '{component}', please install it manually with 'nf-core {self.component_type} install  {component}'."
                             )
                         removed_components.append(component)
                         return removed
             # Remove the component files of all entries removed from modules.json
             removed = (
                 True if self.clear_component_dir(component, Path(self.dir, removed_component_dir)) or removed else False
             )
```

### Comparing `nf-core-2.7.2/nf_core/components/update.py` & `nf-core-2.8/nf_core/components/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         # Check if component is installed before trying to update
         if component not in choices:
             raise LookupError(
                 f"{self.component_type[:-1].title()} '{component}' is not installed in pipeline and could therefore not be updated"
             )
 
         # Check that the supplied name is an available module/subworkflow
-        if component and component not in self.modules_repo.get_avail_components(self.component_type):
+        if component and component not in self.modules_repo.get_avail_components(self.component_type, commit=self.sha):
             raise LookupError(
                 f"{self.component_type[:-1].title()} '{component}' not found in list of available {self.component_type}."
                 f"Use the command 'nf-core {self.component_type} list remote' to view available software"
             )
 
         sha = self.sha
         config_entry = None
@@ -875,44 +875,53 @@
             self.update(s_update, silent=True, updated=updated, check_diff_exist=check_diff_exist)
             self._reset_component_type(original_component_type, original_update_all)
 
         for m_update in modules_to_update:
             if m_update in updated:
                 continue
             original_component_type, original_update_all = self._change_component_type("modules")
-            self.update(m_update, silent=True, updated=updated, check_diff_exist=check_diff_exist)
-            self._reset_component_type(original_component_type, original_update_all)
+            try:
+                self.update(m_update, silent=True, updated=updated, check_diff_exist=check_diff_exist)
+            except LookupError as e:
+                # If the module to be updated is not available, check if there has been a name change
+                if "not found in list of available" in str(e):
+                    # Skip update, we check for name changes with manage_changes_in_linked_components
+                    pass
+                else:
+                    raise
+            finally:
+                self._reset_component_type(original_component_type, original_update_all)
 
     def manage_changes_in_linked_components(self, component, modules_to_update, subworkflows_to_update):
         """Check for linked components added or removed in the new subworkflow version"""
         if self.component_type == "subworkflows":
             subworkflow_directory = Path(self.dir, self.component_type, self.modules_repo.repo_path, component)
             included_modules, included_subworkflows = get_components_to_install(subworkflow_directory)
-            # If a new module/subworkflow is included in the subworklfow and wasn't included before
-            for module in included_modules:
-                if module not in modules_to_update:
-                    log.info(f"Installing newly included module '{module}' for '{component}'")
-                    install_module_object = ComponentInstall(self.dir, "modules", installed_by=component)
-                    install_module_object.install(module, silent=True)
-            for subworkflow in included_subworkflows:
-                if subworkflow not in subworkflows_to_update:
-                    log.info(f"Installing newly included subworkflow '{subworkflow}' for '{component}'")
-                    install_subworkflow_object = ComponentInstall(self.dir, "subworkflows", installed_by=component)
-                    install_subworkflow_object.install(subworkflow, silent=True)
             # If a module/subworkflow has been removed from the subworkflow
             for module in modules_to_update:
                 if module not in included_modules:
                     log.info(f"Removing module '{module}' which is not included in '{component}' anymore.")
                     remove_module_object = ComponentRemove("modules", self.dir)
                     remove_module_object.remove(module, removed_by=component)
             for subworkflow in subworkflows_to_update:
                 if subworkflow not in included_subworkflows:
                     log.info(f"Removing subworkflow '{subworkflow}' which is not included in '{component}' anymore.")
                     remove_subworkflow_object = ComponentRemove("subworkflows", self.dir)
                     remove_subworkflow_object.remove(subworkflow, removed_by=component)
+            # If a new module/subworkflow is included in the subworklfow and wasn't included before
+            for module in included_modules:
+                if module not in modules_to_update:
+                    log.info(f"Installing newly included module '{module}' for '{component}'")
+                    install_module_object = ComponentInstall(self.dir, "modules", installed_by=component)
+                    install_module_object.install(module, silent=True)
+            for subworkflow in included_subworkflows:
+                if subworkflow not in subworkflows_to_update:
+                    log.info(f"Installing newly included subworkflow '{subworkflow}' for '{component}'")
+                    install_subworkflow_object = ComponentInstall(self.dir, "subworkflows", installed_by=component)
+                    install_subworkflow_object.install(subworkflow, silent=True)
 
     def _change_component_type(self, new_component_type):
         original_component_type = self.component_type
         self.component_type = new_component_type
         self.modules_json.pipeline_components = None
         # also reset update_all in case it's set
         original_update_all = self.update_all
```

### Comparing `nf-core-2.7.2/nf_core/create.py` & `nf-core-2.8/nf_core/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         no_git=False,
         force=False,
         outdir=None,
         template_yaml_path=None,
         plain=False,
         default_branch=None,
     ):
-        self.template_params, skip_paths_keys = self.create_param_dict(
+        self.template_params, skip_paths_keys, self.template_yaml = self.create_param_dict(
             name, description, author, version, template_yaml_path, plain
         )
 
         skippable_paths = {
             "github": [
                 ".github/",
                 ".gitignore",
@@ -168,21 +168,21 @@
 
         _, config_yml = nf_core.utils.load_tools_config()
         if (
             "lint" in config_yml
             and "nextflow_config" in config_yml["lint"]
             and "manifest.name" in config_yml["lint"]["nextflow_config"]
         ):
-            return param_dict, skip_paths
+            return param_dict, skip_paths, template_yaml
         if param_dict["prefix"] == "nf-core":
             # Check that the pipeline name matches the requirements
             if not re.match(r"^[a-z]+$", param_dict["short_name"]):
                 raise UserWarning("[red]Invalid workflow name: must be lowercase without punctuation.")
 
-        return param_dict, skip_paths
+        return param_dict, skip_paths, template_yaml
 
     def customize_template(self, template_areas):
         """Customizes the template parameters.
 
         Args:
             name (str): Name for the pipeline.
             description (str): Description for the pipeline.
@@ -279,15 +279,14 @@
         rename_files = {
             "workflows/pipeline.nf": f"workflows/{short_name}.nf",
             "lib/WorkflowPipeline.groovy": f"lib/Workflow{short_name[0].upper()}{short_name[1:]}.groovy",
         }
 
         # Set the paths to skip according to customization
         for template_fn_path_obj in template_files:
-
             template_fn_path = str(template_fn_path_obj)
 
             # Skip files that are in the self.skip_paths list
             for skip_path in self.skip_paths:
                 if os.path.relpath(template_fn_path, template_dir).startswith(skip_path):
                     break
             else:
@@ -345,14 +344,19 @@
                 # Remove field mentioning nf-core docs
                 # in the github bug report template
                 self.remove_nf_core_in_bug_report_template()
 
             # Update the .nf-core.yml with linting configurations
             self.fix_linting()
 
+        log.debug("Dumping pipeline template yml to file")
+        if self.template_yaml:
+            with open(self.outdir / "pipeline_template.yml", "w") as fh:
+                yaml.safe_dump(self.template_yaml, fh)
+
     def update_nextflow_schema(self):
         """
         Removes unused parameters from the nextflow schema.
         """
         schema_path = self.outdir / "nextflow_schema.json"
 
         schema = nf_core.schema.PipelineSchema()
```

### Comparing `nf-core-2.7.2/nf_core/download.py` & `nf-core-2.8/nf_core/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
             } else {
                 container "quay.io/biocontainers/fastqc:0.11.9--0"
             }
 
         Later DSL2:
             container "${ workflow.containerEngine == 'singularity' && !task.ext.singularity_pull_docker_container ?
                 'https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0' :
-                'quay.io/biocontainers/fastqc:0.11.9--0' }"
+                'biocontainers/fastqc:0.11.9--0' }"
 
         DSL1 / Special case DSL2:
             container "nfcore/cellranger:6.0.2"
         """
 
         log.debug("Fetching container names for workflow")
         containers_raw = []
@@ -502,15 +502,14 @@
 
                 # Organise containers based on what we need to do with them
                 containers_exist = []
                 containers_cache = []
                 containers_download = []
                 containers_pull = []
                 for container in self.containers:
-
                     # Fetch the output and cached filenames for this container
                     out_path, cache_path = self.singularity_image_filenames(container)
 
                     # Check that the directories exist
                     out_path_dir = os.path.dirname(out_path)
                     if not os.path.isdir(out_path_dir):
                         log.debug(f"Output directory not found, creating: {out_path_dir}")
```

### Comparing `nf-core-2.7.2/nf_core/launch.py` & `nf-core-2.8/nf_core/launch.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
             }
         }
         self.nxf_flags = {}
         self.params_user = {}
         self.cli_launch = True
 
     def launch_pipeline(self):
-
         # Prompt for pipeline if not supplied and no web launch ID
         if self.pipeline is None and self.web_id is None:
             launch_type = questionary.select(
                 "Launch local pipeline or remote GitHub pipeline?",
                 choices=["Remote pipeline", "Local path"],
                 style=nf_core.utils.nfcore_question_style,
             ).unsafe_ask()
@@ -457,15 +456,14 @@
         Returns:
           Dict of param_id:val answers
         """
         while_break = False
         answers = {}
         error_msgs = []
         while not while_break:
-
             if len(error_msgs) == 0:
                 self.print_param_header(group_id, group_obj, True)
 
             question = {
                 "type": "list",
                 "name": group_id,
                 "qmark": "",
@@ -694,15 +692,14 @@
                 self.nextflow_cmd += f" {flag}"
             # String values
             elif not isinstance(val, bool):
                 self.nextflow_cmd += ' {} "{}"'.format(flag, val.replace('"', '\\"'))
 
         # Pipeline parameters
         if len(self.schema_obj.input_params) > 0:
-
             # Write the user selection to a file and run nextflow with that
             if self.use_params_file:
                 dump_json_with_prettier(self.params_out, self.schema_obj.input_params)
                 self.nextflow_cmd += f' -params-file "{os.path.relpath(self.params_out)}"'
 
             # Call nextflow with a list of command line flags
             else:
```

### Comparing `nf-core-2.7.2/nf_core/licences.py` & `nf-core-2.8/nf_core/licences.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/__init__.py` & `nf-core-2.8/nf_core/lint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
     from .nextflow_config import nextflow_config
     from .pipeline_name_conventions import pipeline_name_conventions
     from .pipeline_todos import pipeline_todos
     from .readme import readme
     from .schema_description import schema_description
     from .schema_lint import schema_lint
     from .schema_params import schema_params
+    from .system_exit import system_exit
     from .template_strings import template_strings
     from .version_consistency import version_consistency
 
     def __init__(
         self, wf_path, release_mode=False, fix=(), key=None, fail_ignored=False, fail_warned=False, hide_progress=False
     ):
         """Initialise linting object"""
@@ -219,14 +220,15 @@
             "actions_awsfulltest",
             "readme",
             "pipeline_todos",
             "pipeline_name_conventions",
             "template_strings",
             "schema_lint",
             "schema_params",
+            "system_exit",
             "schema_description",
             "actions_schema_validation",
             "merge_markers",
             "modules_json",
             "multiqc_config",
             "modules_structure",
         ] + (["version_consistency"] if release_mode else [])
@@ -430,15 +432,14 @@
                     title_align="left",
                     style="red",
                     padding=1,
                 )
             )
 
     def _print_summary(self):
-
         # Summary table
         summary_colour = "red" if len(self.failed) > 0 else "green"
         table = Table(box=rich.box.ROUNDED, style=summary_colour)
         table.add_column("LINT RESULTS SUMMARY", no_wrap=True)
         table.add_row(rf"[green][✔] {len(self.passed):>3} Test{_s(self.passed)} Passed")
         if len(self.fix):
             table.add_row(rf"[bright blue][?] {len(self.fixed):>3} Test{_s(self.fixed)} Fixed")
```

### Comparing `nf-core-2.7.2/nf_core/lint/actions_awsfulltest.py` & `nf-core-2.8/nf_core/lint/actions_awsfulltest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/actions_awstest.py` & `nf-core-2.8/nf_core/lint/actions_awstest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/actions_ci.py` & `nf-core-2.8/nf_core/lint/actions_ci.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/actions_schema_validation.py` & `nf-core-2.8/nf_core/lint/actions_schema_validation.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/files_exist.py` & `nf-core-2.8/nf_core/lint/files_exist.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/files_unchanged.py` & `nf-core-2.8/nf_core/lint/files_unchanged.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
 
     def _tf(file_path):
         """Helper function - get file path for template file"""
         return os.path.join(test_pipeline_dir, file_path)
 
     # Files that must be completely unchanged from template
     for files in files_exact:
-
         # Ignore if file specified in linting config
         ignore_files = self.lint_config.get("files_unchanged", [])
         if any([f in ignore_files for f in files]):
             ignored.append(f"File ignored due to lint config: {self._wrap_quotes(files)}")
 
         # Ignore if we can't find the file
         elif not any([os.path.isfile(_pf(f)) for f in files]):
@@ -173,15 +172,14 @@
                             failed.append(f"`{f}` does not match the template")
                             could_fix = True
                 except FileNotFoundError:
                     pass
 
     # Files that can be added to, but that must contain the template contents
     for files in files_partial:
-
         # Ignore if file specified in linting config
         ignore_files = self.lint_config.get("files_unchanged", [])
         if any([f in ignore_files for f in files]):
             ignored.append(f"File ignored due to lint config: {self._wrap_quotes(files)}")
 
         # Ignore if we can't find the file
         elif not any([os.path.isfile(_pf(f)) for f in files]):
```

### Comparing `nf-core-2.7.2/nf_core/lint/merge_markers.py` & `nf-core-2.8/nf_core/lint/merge_markers.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/modules_json.py` & `nf-core-2.8/nf_core/lint/modules_json.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/modules_structure.py` & `nf-core-2.8/nf_core/lint/modules_structure.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/multiqc_config.py` & `nf-core-2.8/nf_core/lint/multiqc_config.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/nextflow_config.py` & `nf-core-2.8/nf_core/lint/nextflow_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,30 @@
         .. tip:: The ``snake_case`` convention should now be used when defining pipeline parameters
 
     **The following Nextflow syntax is depreciated and fails the test if present:**
 
     * Process-level configuration syntax still using the old Nextflow syntax, for example: ``process.$fastqc`` instead of ``process withName:'fastqc'``.
 
     .. tip:: You can choose to ignore tests for the presence or absence of specific config variables
-             by creating a file called ``.nf-core-lint.yml`` in the root of your pipeline and creating
+             by creating a file called ``.nf-core.yml`` in the root of your pipeline and creating
              a list the config variables that should be ignored. For example:
 
              .. code-block:: yaml
 
-                nextflow_config:
-                    - params.input
+                lint:
+                    nextflow_config:
+                        - params.input
 
              The other checks in this test (depreciated syntax etc) can not be individually identified,
              but you can skip the entire test block if you wish:
 
              .. code-block:: yaml
 
-                nextflow_config: False
+                lint:
+                    nextflow_config: False
     """
     passed = []
     warned = []
     failed = []
     ignored = []
 
     # Fail tests if these are missing
```

### Comparing `nf-core-2.7.2/nf_core/lint/pipeline_name_conventions.py` & `nf-core-2.8/nf_core/lint/pipeline_name_conventions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/pipeline_todos.py` & `nf-core-2.8/nf_core/lint/pipeline_todos.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/readme.py` & `nf-core-2.8/nf_core/lint/readme.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,24 +13,20 @@
       * If a badge is found but the version doesn't match the minimum version in the config file, the test fails
       * Example badge code:
 
         .. code-block:: md
 
            [![Nextflow](https://img.shields.io/badge/nextflow-%E2%89%A50.27.6-brightgreen.svg)](https://www.nextflow.io/)
 
-    * Bioconda badge
+    .. note:: This badge are a markdown image ``![alt-text](<image URL>)`` *inside* a markdown link ``[markdown image](<link URL>)``, so a bit fiddly to write.
 
-      * If your pipeline contains a file called ``environment.yml`` in the root directory, a bioconda badge is required
-      * Required badge code:
+    * Zenodo release
 
-        .. code-block:: md
-
-           [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg)](https://bioconda.github.io/)
+        * If pipeline is released but still contains a 'zenodo.XXXXXXX' tag, the test fails
 
-    .. note:: These badges are a markdown image ``![alt-text](<image URL>)`` *inside* a markdown link ``[markdown image](<link URL>)``, so a bit fiddly to write.
     """
     passed = []
     warned = []
     failed = []
 
     # Remove field that should be ignored according to the linting config
     ignore_configs = self.lint_config.get("readme", [])
@@ -58,28 +54,20 @@
                 passed.append(
                     f"README Nextflow minimum version badge matched config. Badge: `{nf_badge_version}`, "
                     f"Config: `{self.minNextflowVersion}`"
                 )
         else:
             warned.append("README did not have a Nextflow minimum version badge.")
 
-    # Check that the minimum version mentioned in the quick start section is consistent
-    # Looking for: "1. Install [`Nextflow`](https://www.nextflow.io/docs/latest/getstarted.html#installation) (`>=22.10.1`)"
-    nf_version_re = r"1\.\s*Install\s*\[`Nextflow`\]\(https://www.nextflow.io/docs/latest/getstarted.html#installation\)\s*\(`>=(\d*\.\d*\.\d*)`\)"
-    match = re.search(nf_version_re, content)
-    if match:
-        nf_quickstart_version = match.group(1)
-        try:
-            if nf_quickstart_version != self.minNextflowVersion:
-                raise AssertionError()
-        except (AssertionError, KeyError):
-            failed.append(
-                f"README Nextflow minimium version in Quick Start section does not match config. README: `{nf_quickstart_version}`, Config `{self.minNextflowVersion}`"
+    if "zenodo_doi" not in ignore_configs:
+        # Check that zenodo.XXXXXXX has been replaced with the zendo.DOI
+        zenodo_re = r"/zenodo\.X+"
+        match = re.search(zenodo_re, content)
+        if match:
+            warned.append(
+                "README contains the placeholder `zenodo.XXXXXXX`. "
+                "This should be replaced with the zenodo doi (after the first release)."
             )
         else:
-            passed.append(
-                f"README Nextflow minimum version in Quick Start section matched config. README: `{nf_quickstart_version}`, Config: `{self.minNextflowVersion}`"
-            )
-    else:
-        warned.append("README did not have a Nextflow minimum version mentioned in Quick Start section.")
+            passed.append("README Zenodo placeholder was replaced with DOI.")
 
     return {"passed": passed, "warned": warned, "failed": failed}
```

### Comparing `nf-core-2.7.2/nf_core/lint/schema_description.py` & `nf-core-2.8/nf_core/lint/schema_description.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/schema_lint.py` & `nf-core-2.8/nf_core/lint/schema_lint.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/schema_params.py` & `nf-core-2.8/nf_core/lint/schema_params.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint/template_strings.py` & `nf-core-2.8/nf_core/lint/template_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     """
     passed = []
     failed = []
 
     # Loop through files, searching for string
     num_matches = 0
     for fn in self.files:
-
         # Skip binary files
         binary_ftypes = ["image", "application/java-archive"]
         (ftype, encoding) = mimetypes.guess_type(fn)
         if encoding is not None or (ftype is not None and any([ftype.startswith(ft) for ft in binary_ftypes])):
             continue
 
         with io.open(fn, "r", encoding="latin1") as fh:
```

### Comparing `nf-core-2.7.2/nf_core/lint/version_consistency.py` & `nf-core-2.8/nf_core/lint/version_consistency.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/lint_utils.py` & `nf-core-2.8/nf_core/lint_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/list.py` & `nf-core-2.8/nf_core/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,14 @@
         self.last_pull_date = None
         self.last_pull_pretty = None
 
     def get_local_nf_workflow_details(self):
         """Get full details about a local cached workflow"""
 
         if self.local_path is None:
-
             # Try to guess the local cache directory
             if len(os.environ.get("NXF_ASSETS", "")) > 0:
                 nf_wfdir = os.path.join(os.environ.get("NXF_ASSETS"), self.full_name)
             elif len(os.environ.get("NXF_HOME", "")) > 0:
                 nf_wfdir = os.path.join(os.environ.get("NXF_HOME"), "assets", self.full_name)
             else:
                 nf_wfdir = os.path.join(os.getenv("HOME"), ".nextflow", "assets", self.full_name)
```

### Comparing `nf-core-2.7.2/nf_core/module-template/modules/main.nf` & `nf-core-2.8/nf_core/module-template/modules/main.nf`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{%- if not_empty_template -%}
 // TODO nf-core: If in doubt look at other nf-core/modules to see how we are doing things! :)
 //               https://github.com/nf-core/modules/tree/master/modules/nf-core/
 //               You can also ask for help via your pull request or on the #modules channel on the nf-core Slack workspace:
 //               https://nf-co.re/join
 // TODO nf-core: A module file SHOULD only define input and output files as command-line parameters.
 //               All other parameters MUST be provided using the "task.ext" directive, see here:
 //               https://www.nextflow.io/docs/latest/process.html#ext
@@ -10,70 +11,87 @@
 //               e.g. single-end/paired-end data MUST also be defined and evaluated appropriately.
 // TODO nf-core: Software that can be piped together SHOULD be added to separate module files
 //               unless there is a run-time, storage advantage in implementing in this way
 //               e.g. it's ok to have a single module for bwa to output BAM instead of SAM:
 //                 bwa mem | samtools view -B -T ref.fasta
 // TODO nf-core: Optional inputs are not currently supported by Nextflow. However, using an empty
 //               list (`[]`) instead of a file can be used to work around this issue.
+{%- endif %}
 
-process {{ tool_name_underscore|upper }} {
+process {{ component_name_underscore|upper }} {
     tag {{ '"$meta.id"' if has_meta else "'$bam'" }}
     label '{{ process_label }}'
 
+    {% if not_empty_template -%}
     // TODO nf-core: List required Conda package(s).
     //               Software MUST be pinned to channel (i.e. "bioconda"), version (i.e. "1.10").
     //               For Conda, the build (i.e. "h9402c20_2") must be EXCLUDED to support installation on different operating systems.
     // TODO nf-core: See section in main README for further information regarding finding and adding container addresses to the section below.
+    {% endif -%}
     conda "{{ bioconda if bioconda else 'YOUR-TOOL-HERE' }}"
     container "${ workflow.containerEngine == 'singularity' && !task.ext.singularity_pull_docker_container ?
         '{{ singularity_container if singularity_container else 'https://depot.galaxyproject.org/singularity/YOUR-TOOL-HERE' }}':
-        '{{ docker_container if docker_container else 'quay.io/biocontainers/YOUR-TOOL-HERE' }}' }"
+        '{{ docker_container if docker_container else 'biocontainers/YOUR-TOOL-HERE' }}' }"
 
     input:
+    {% if not_empty_template -%}
     // TODO nf-core: Where applicable all sample-specific information e.g. "id", "single_end", "read_group"
     //               MUST be provided as an input via a Groovy Map called "meta".
     //               This information may not be required in some instances e.g. indexing reference genome files:
     //               https://github.com/nf-core/modules/blob/master/modules/nf-core/bwa/index/main.nf
     // TODO nf-core: Where applicable please provide/convert compressed files as input/output
     //               e.g. "*.fastq.gz" and NOT "*.fastq", "*.bam" and NOT "*.sam" etc.
     {{ 'tuple val(meta), path(bam)' if has_meta else 'path bam' }}
+    {%- else -%}
+    {{ 'tuple val(meta), path(input)' if has_meta else 'path input' }}
+    {%- endif %}
 
     output:
+    {% if not_empty_template -%}
     // TODO nf-core: Named file extensions MUST be emitted for ALL output channels
     {{ 'tuple val(meta), path("*.bam")' if has_meta else 'path "*.bam"' }}, emit: bam
+    {%- else -%}
+    {{ 'tuple val(meta), path("*")' if has_meta else 'path "*"' }}, emit: output
+    {%- endif %}
+    {% if not_empty_template -%}
     // TODO nf-core: List additional required output channels/values here
+    {%- endif %}
     path "versions.yml"           , emit: versions
 
     when:
     task.ext.when == null || task.ext.when
 
     script:
     def args = task.ext.args ?: ''
     {% if has_meta -%}
     def prefix = task.ext.prefix ?: "${meta.id}"
     {%- endif %}
+    {% if not_empty_template -%}
     // TODO nf-core: Where possible, a command MUST be provided to obtain the version number of the software e.g. 1.10
     //               If the software is unable to output a version number on the command-line then it can be manually specified
     //               e.g. https://github.com/nf-core/modules/blob/master/modules/nf-core/homer/annotatepeaks/main.nf
     //               Each software used MUST provide the software name and version number in the YAML version file (versions.yml)
     // TODO nf-core: It MUST be possible to pass additional parameters to the tool as a command-line string via the "task.ext.args" directive
     // TODO nf-core: If the tool supports multi-threading then you MUST provide the appropriate parameter
     //               using the Nextflow "task" variable e.g. "--threads $task.cpus"
     // TODO nf-core: Please replace the example samtools command below with your module's command
     // TODO nf-core: Please indent the command appropriately (4 spaces!!) to help with readability ;)
+    {%- endif %}
     """
+    {% if not_empty_template -%}
     samtools \\
         sort \\
         $args \\
         -@ $task.cpus \\
         {%- if has_meta %}
         -o ${prefix}.bam \\
         -T $prefix \\
         {%- endif %}
         $bam
+    {%- endif %}
 
     cat <<-END_VERSIONS > versions.yml
     "${task.process}":
         {{ tool }}: \$(echo \$(samtools --version 2>&1) | sed 's/^.*samtools //; s/Using.*\$//' ))
     END_VERSIONS
     """
 }
```

### Comparing `nf-core-2.7.2/nf_core/module-template/modules/meta.yml` & `nf-core-2.8/nf_core/module-template/modules/meta.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-name: "{{ tool_name_underscore }}"
+---
+# yaml-language-server: $schema=https://raw.githubusercontent.com/nf-core/modules/master/modules/yaml-schema.json
+name: "{{ component_name_underscore }}"
+{% if not_empty_template -%}
 ## TODO nf-core: Add a description of the module and list keywords
+{% endif -%}
 description: write your description here
 keywords:
   - sort
+  - example
+  - genomics
 tools:
-  - "{{ tool }}":
+  - "{{ component }}":
+      {% if not_empty_template -%}
       ## TODO nf-core: Add a description and other details for the software below
+      {% endif -%}
       description: "{{ tool_description }}"
       homepage: "{{ tool_doc_url }}"
       documentation: "{{ tool_doc_url }}"
       tool_dev_url: "{{ tool_dev_url }}"
       doi: ""
       licence: "{{ tool_licence }}"
 
+{% if not_empty_template -%}
 ## TODO nf-core: Add a description of all of the variables used as input
+{% endif -%}
 input:
   #{% if has_meta %} Only when we have meta
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
         e.g. [ id:'test', single_end:false ]
-  #{% endif %}
+  {% endif %}
+  {% if not_empty_template -%}
   ## TODO nf-core: Delete / customise this example input
-  - bam:
+  {%- endif %}
+  - {{ 'bam:' if not_empty_template else "input:" }}
       type: file
-      description: BAM/CRAM/SAM file
-      pattern: "*.{bam,cram,sam}"
+      description: {{ 'Sorted BAM/CRAM/SAM file' if not_empty_template else "" }}
+      pattern: {{ '"*.{bam,cram,sam}"' if not_empty_template else "" }}
 
+{% if not_empty_template -%}
 ## TODO nf-core: Add a description of all of the variables used as output
+{% endif -%}
 output:
   #{% if has_meta -%} Only when we have meta
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
         e.g. [ id:'test', single_end:false ]
-  #{% endif %}
+  {% endif %}
   - versions:
       type: file
       description: File containing software versions
       pattern: "versions.yml"
+  {% if not_empty_template -%}
   ## TODO nf-core: Delete / customise this example output
-  - bam:
+  {%- endif %}
+  - {{ 'bam:' if not_empty_template else "output:" }}
       type: file
-      description: Sorted BAM/CRAM/SAM file
-      pattern: "*.{bam,cram,sam}"
+      description: {{ 'Sorted BAM/CRAM/SAM file' if not_empty_template else "" }}
+      pattern: {{ '"*.{bam,cram,sam}"' if not_empty_template else "" }}
 
 authors:
   - "{{ author }}"
```

### Comparing `nf-core-2.7.2/nf_core/modules/bump_versions.py` & `nf-core-2.8/nf_core/modules/bump_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,30 +168,29 @@
                 docker_img, singularity_img = nf_core.utils.get_biocontainer_tag(bioconda_tool_name, last_ver)
             except LookupError as e:
                 self.failed.append((f"Could not download container tags: {e}", module.module_name))
                 return False
 
             patterns = [
                 (bioconda_packages[0], f"'bioconda::{bioconda_tool_name}={last_ver}'"),
-                (rf"quay.io/biocontainers/{bioconda_tool_name}:[^'\"\s]+", docker_img),
+                (rf"biocontainers/{bioconda_tool_name}:[^'\"\s]+", docker_img),
                 (
                     rf"https://depot.galaxyproject.org/singularity/{bioconda_tool_name}:[^'\"\s]+",
                     singularity_img,
                 ),
             ]
 
             with open(module.main_nf, "r") as fh:
                 content = fh.read()
 
             # Go over file content of main.nf and find replacements
             for pattern in patterns:
                 found_match = False
                 newcontent = []
                 for line in content.splitlines():
-
                     # Match the pattern
                     matches_pattern = re.findall(rf"^.*{pattern[0]}.*$", line)
                     if matches_pattern:
                         found_match = True
 
                         # Replace the match
                         newline = re.sub(pattern[0], pattern[1], line)
```

### Comparing `nf-core-2.7.2/nf_core/modules/install.py` & `nf-core-2.8/nf_core/modules/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/lint/__init__.py` & `nf-core-2.8/nf_core/modules/lint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         self.lint_tests = self.get_all_lint_tests(self.repo_type == "pipeline")
 
         if self.repo_type == "pipeline":
             modules_json = ModulesJson(self.dir)
             modules_json.check_up_to_date()
             self.all_remote_modules = []
             for repo_url, components in modules_json.get_all_components(self.component_type).items():
+                if remote_url is not None and remote_url != repo_url:
+                    continue
                 for org, comp in components:
                     self.all_remote_modules.append(
                         NFCoreModule(
                             comp,
                             repo_url,
                             Path(self.dir, self.component_type, org, comp),
                             self.repo_type,
```

### Comparing `nf-core-2.7.2/nf_core/modules/lint/main_nf.py` & `nf-core-2.8/nf_core/modules/lint/main_nf.py`

 * *Files 5% similar despite different names*

```diff
@@ -231,39 +231,39 @@
     self.process_name = lines[0].split()[1]
     if all(x.upper() for x in self.process_name):
         self.passed.append(("process_capitals", "Process name is in capital letters", self.main_nf))
     else:
         self.failed.append(("process_capitals", "Process name is not in capital letters", self.main_nf))
 
     # Check that process labels are correct
-    correct_process_labels = ["process_single", "process_low", "process_medium", "process_high", "process_long"]
-    process_label = [l for l in lines if l.lstrip().startswith("label")]
-    if len(process_label) > 0:
-        try:
-            process_label = re.search("process_[A-Za-z]+", process_label[0]).group(0)
-        except AttributeError:
-            process_label = re.search("'([A-Za-z_-]+)'", process_label[0]).group(0)
-        finally:
-            if not process_label in correct_process_labels:
-                self.warned.append(
+    check_process_labels(self, lines)
+
+    # Deprecated enable_conda
+    for i, l in enumerate(lines):
+        url = None
+        l = l.strip(" '\"")
+        if _container_type(l) == "conda":
+            bioconda_packages = [b for b in l.split() if "bioconda::" in b]
+            match = re.search(r"params\.enable_conda", l)
+            if match is None:
+                self.passed.append(
                     (
-                        "process_standard_label",
-                        f"Process label ({process_label}) is not among standard labels: `{'`,`'.join(correct_process_labels)}`",
+                        "deprecated_enable_conda",
+                        f"Deprecated parameter 'params.enable_conda' correctly not found in the conda definition",
                         self.main_nf,
                     )
                 )
             else:
-                self.passed.append(("process_standard_label", "Correct process label", self.main_nf))
-    else:
-        self.warned.append(("process_standard_label", "Process label unspecified", self.main_nf))
-    for i, l in enumerate(lines):
-        url = None
-        if _container_type(l) == "bioconda":
-            bioconda_packages = [b for b in l.split() if "bioconda::" in b]
-        l = l.strip(" '\"")
+                self.failed.append(
+                    (
+                        "deprecated_enable_conda",
+                        f"Found deprecated parameter 'params.enable_conda' in the conda definition",
+                        self.main_nf,
+                    )
+                )
         if _container_type(l) == "singularity":
             # e.g. "https://containers.biocontainers.pro/s3/SingImgsRepo/biocontainers/v1.2.0_cv1/biocontainers_v1.2.0_cv1.img' :" -> v1.2.0_cv1
             # e.g. "https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0' :" -> 0.11.9--0
             match = re.search(r"(?:/)?(?:biocontainers_)?(?::)?([A-Za-z\d\-_.]+?)(?:\.img)?'", l)
             if match is not None:
                 singularity_tag = match.group(1)
                 self.passed.append(("singularity_tag", f"Found singularity tag: {singularity_tag}", self.main_nf))
@@ -286,14 +286,17 @@
             match = re.search(r"(?:[/])?(?::)?([A-Za-z\d\-_.]+)'", l)
             if match is not None:
                 docker_tag = match.group(1)
                 self.passed.append(("docker_tag", f"Found docker tag: {docker_tag}", self.main_nf))
             else:
                 self.failed.append(("docker_tag", "Unable to parse docker tag", self.main_nf))
                 docker_tag = None
+            if l.startswith("biocontainers/"):
+                # When we think it is a biocontainer, assume we are querying quay.io/biocontainers and insert quay.io as prefix
+                l = "quay.io/" + l
             url = urlparse(l.split("'")[0])
             # lint double quotes
             if l.count('"') > 2:
                 self.failed.append(
                     ("container_links", "Too many double quotes found when specifying docker container", self.main_nf)
                 )
         # lint double quotes
@@ -388,14 +391,64 @@
                     )
             else:
                 self.passed.append(("bioconda_latest", f"Conda package is the latest available: `{bp}`", self.main_nf))
 
     return docker_tag == singularity_tag
 
 
+def check_process_labels(self, lines):
+    correct_process_labels = ["process_single", "process_low", "process_medium", "process_high", "process_long"]
+    all_labels = [l.strip() for l in lines if l.lstrip().startswith("label ")]
+    bad_labels = []
+    good_labels = []
+    if len(all_labels) > 0:
+        for label in all_labels:
+            try:
+                label = re.match(r"^label\s+'?([a-zA-Z0-9_-]+)'?$", label).group(1)
+            except AttributeError:
+                self.warned.append(
+                    (
+                        "process_standard_label",
+                        f"Specified label appears to contain non-alphanumerics: {label}",
+                        self.main_nf,
+                    )
+                )
+                continue
+            if label not in correct_process_labels:
+                bad_labels.append(label)
+            else:
+                good_labels.append(label)
+        if len(good_labels) > 1:
+            self.warned.append(
+                (
+                    "process_standard_label",
+                    f"Conflicting process labels found: `{'`,`'.join(good_labels)}`",
+                    self.main_nf,
+                )
+            )
+        elif len(good_labels) == 1:
+            self.passed.append(("process_standard_label", "Correct process label", self.main_nf))
+        else:
+            self.warned.append(("process_standard_label", "Standard process label not found", self.main_nf))
+        if len(bad_labels) > 0:
+            self.warned.append(
+                ("process_standard_label", f"Non-standard labels found: `{'`,`'.join(bad_labels)}`", self.main_nf)
+            )
+        if len(all_labels) > len(set(all_labels)):
+            self.warned.append(
+                (
+                    "process_standard_label",
+                    f"Duplicate labels found: `{'`,`'.join(sorted(all_labels))}`",
+                    self.main_nf,
+                )
+            )
+    else:
+        self.warned.append(("process_standard_label", "Process label not specified", self.main_nf))
+
+
 def _parse_input(self, line_raw):
     """
     Return list of input channel names from an input line.
 
     If more than one elements in channel should work with both of:
         tuple val(meta), path(reads)
         tuple val(meta), path(reads, stageAs: "input*/*")
@@ -467,15 +520,15 @@
         lines = source.readlines()
 
     # Check if the new version + build exist and replace
     new_lines = []
     for line in lines:
         l = line.strip(" '\"")
         build_type = _container_type(l)
-        if build_type == "bioconda":
+        if build_type == "conda":
             new_lines.append(re.sub(rf"{current_version}", f"{latest_version}", line))
         elif build_type in ("singularity", "docker"):
             # Check that the new url is valid
             new_url = re.search(
                 "(?:['\"])(.+)(?:['\"])", re.sub(rf"{singularity_tag}", f"{latest_version}--{build}", line)
             ).group(1)
             try:
@@ -512,21 +565,25 @@
         if f.get("version") == latest_v:
             build_times.append((f.get("upload_time"), f.get("attrs").get("build")))
     return sorted(build_times, key=lambda tup: tup[0], reverse=True)[0][1]
 
 
 def _container_type(line):
     """Returns the container type of a build."""
-    if re.search("bioconda::", line):
-        return "bioconda"
+    if line.startswith("conda"):
+        return "conda"
     if line.startswith("https://containers") or line.startswith("https://depot"):
         # Look for a http download URL.
         # Thanks Stack Overflow for the regex: https://stackoverflow.com/a/3809435/713980
         url_regex = (
             r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)"
         )
         url_match = re.search(url_regex, line, re.S)
         if url_match:
             return "singularity"
         return None
-    if line.startswith("biocontainers/") or line.startswith("quay.io/"):
+    if (
+        line.startswith("biocontainers/")
+        or line.startswith("quay.io/")
+        or (line.count("/") == 1 and line.count(":") == 1)
+    ):
         return "docker"
```

### Comparing `nf-core-2.7.2/nf_core/modules/lint/module_changes.py` & `nf-core-2.8/nf_core/modules/lint/module_changes.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/lint/module_deprecations.py` & `nf-core-2.8/nf_core/modules/lint/module_deprecations.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/lint/module_patch.py` & `nf-core-2.8/nf_core/modules/lint/module_patch.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/lint/module_tests.py` & `nf-core-2.8/nf_core/modules/lint/module_tests.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/lint/module_todos.py` & `nf-core-2.8/nf_core/modules/lint/module_todos.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/lint/module_version.py` & `nf-core-2.8/nf_core/modules/lint/module_version.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/modules_differ.py` & `nf-core-2.8/nf_core/modules/modules_differ.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/modules_json.py` & `nf-core-2.8/nf_core/modules/modules_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,24 +415,24 @@
             subworkflow_dirs, missing_installation, "subworkflows"
         )
 
         return untracked_dirs_modules, untracked_dirs_subworkflows, missing_installation
 
     def parse_dirs(self, dirs, missing_installation, component_type):
         untracked_dirs = []
-        for dir in dirs:
+        for dir_ in dirs:
             # Check if the module/subworkflows directory exists in modules.json
-            install_dir = dir.parts[0]
-            component = str(Path(*dir.parts[1:]))
+            install_dir = dir_.parts[0]
+            component = str(Path(*dir_.parts[1:]))
             component_in_file = False
             git_url = None
             for repo in missing_installation:
                 if component_type in missing_installation[repo]:
-                    for dir_name in missing_installation[repo][component_type]:
-                        if component in missing_installation[repo][component_type][dir_name]:
+                    if install_dir in missing_installation[repo][component_type]:
+                        if component in missing_installation[repo][component_type][install_dir]:
                             component_in_file = True
                             git_url = repo
                             break
             if not component_in_file:
                 # If it is not, add it to the list of missing components
                 untracked_dirs.append(component)
             else:
@@ -490,15 +490,15 @@
     def reinstall_repo(self, install_dir, remote_url, module_entries):
         """
         Reinstall modules from a repository
 
         Args:
             install_dir (str): The name of directory where modules are installed
             remote_url (str): The git url of the remote repository
-            modules ([ dict[str, dict[str, str]] ]): Module entries with
+            module_entries ([ dict[str, dict[str, str]] ]): Module entries with
             branch and git sha info
 
         Returns:
             ([ str ]): List of modules that we failed to install
         """
         branches_and_mods = {}
         failed_to_install = []
@@ -741,14 +741,24 @@
             raise LookupError(f"Repo '{repo_url}' not present in 'modules.json'")
         if module_name not in self.modules_json["repos"][repo_url]["modules"][install_dir]:
             raise LookupError(f"Module '{install_dir}/{module_name}' not present in 'modules.json'")
         self.modules_json["repos"][repo_url]["modules"][install_dir][module_name]["patch"] = str(patch_filename)
         if write_file:
             self.dump()
 
+    def remove_patch_entry(self, module_name, repo_url, install_dir, write_file=True):
+        if self.modules_json is None:
+            self.load()
+        try:
+            del self.modules_json["repos"][repo_url]["modules"][install_dir][module_name]["patch"]
+        except KeyError:
+            log.warning("No patch entry in 'modules.json' to remove")
+        if write_file:
+            self.dump()
+
     def get_patch_fn(self, module_name, repo_url, install_dir):
         """
         Get the patch filename of a module
 
         Args:
             module_name (str): The name of the module
             repo_url (str): The URL of the repository containing the module
```

### Comparing `nf-core-2.7.2/nf_core/modules/modules_repo.py` & `nf-core-2.8/nf_core/modules/modules_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,25 +298,25 @@
         Checks out the repository at the requested commit
 
         Args:
             commit (str): Git SHA of the commit
         """
         self.repo.git.checkout(commit)
 
-    def component_exists(self, component_name, component_type, checkout=True):
+    def component_exists(self, component_name, component_type, checkout=True, commit=None):
         """
         Check if a module/subworkflow exists in the branch of the repo
 
         Args:
             component_name (str): The name of the module/subworkflow
 
         Returns:
             (bool): Whether the module/subworkflow exists in this branch of the repository
         """
-        return component_name in self.get_avail_components(component_type, checkout=checkout)
+        return component_name in self.get_avail_components(component_type, checkout=checkout, commit=commit)
 
     def get_component_dir(self, component_name, component_type):
         """
         Returns the file path of a module/subworkflow directory in the repo.
         Does not verify that the path exists.
         Args:
             component_name (str): The name of the module/subworkflow
@@ -445,24 +445,26 @@
             if commit.hexsha == sha:
                 message = commit.message.partition("\n")[0]
                 date_obj = commit.committed_datetime
                 date = str(date_obj.date())
                 return message, date
         raise LookupError(f"Commit '{sha}' not found in the '{self.remote_url}'")
 
-    def get_avail_components(self, component_type, checkout=True):
+    def get_avail_components(self, component_type, checkout=True, commit=None):
         """
         Gets the names of the modules/subworkflows in the repository. They are detected by
         checking which directories have a 'main.nf' file
 
         Returns:
             ([ str ]): The module/subworkflow names
         """
         if checkout:
             self.checkout_branch()
+        if commit is not None:
+            self.checkout(commit)
         # Get directory
         if component_type == "modules":
             directory = self.modules_dir
         elif component_type == "subworkflows":
             directory = self.subworkflows_dir
         # Module/Subworkflow directories are characterized by having a 'main.nf' file
         avail_component_names = [
```

### Comparing `nf-core-2.7.2/nf_core/modules/modules_test.py` & `nf-core-2.8/nf_core/modules/modules_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/modules_utils.py` & `nf-core-2.8/nf_core/modules/modules_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/nfcore_module.py` & `nf-core-2.8/nf_core/modules/nfcore_module.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/modules/patch.py` & `nf-core-2.8/nf_core/modules/patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -126,7 +126,84 @@
             dsp_from_dir=module_current_dir,
             dsp_to_dir=module_current_dir,
         )
 
         # Finally move the created patch file to its final location
         shutil.move(patch_temp_path, patch_path)
         log.info(f"Patch file of '{module_fullname}' written to '{patch_path}'")
+
+    def remove(self, module):
+        # Check modules directory structure
+        self.check_modules_structure()
+
+        self.modules_json.check_up_to_date()
+        self.param_check(module)
+        modules = self.modules_json.get_all_components(self.component_type)[self.modules_repo.remote_url]
+
+        if module is None:
+            choices = [
+                module if directory == self.modules_repo.repo_path else f"{directory}/{module}"
+                for directory, module in modules
+            ]
+            module = questionary.autocomplete(
+                "Tool:",
+                choices,
+                style=nf_core.utils.nfcore_question_style,
+            ).unsafe_ask()
+        module_dir = [dir for dir, m in modules if m == module][0]
+        module_fullname = str(Path("modules", module_dir, module))
+
+        # Verify that the module has an entry in the modules.json file
+        if not self.modules_json.module_present(module, self.modules_repo.remote_url, module_dir):
+            raise UserWarning(
+                f"The '{module_fullname}' module does not have an entry in the 'modules.json' file. Cannot compute patch"
+            )
+
+        module_version = self.modules_json.get_module_version(module, self.modules_repo.remote_url, module_dir)
+        if module_version is None:
+            raise UserWarning(
+                f"The '{module_fullname}' module does not have a valid version in the 'modules.json' file. Cannot compute patch"
+            )
+        # Get the module branch and reset it in the ModulesRepo object
+        module_branch = self.modules_json.get_component_branch(
+            self.component_type, module, self.modules_repo.remote_url, module_dir
+        )
+        if module_branch != self.modules_repo.branch:
+            self.modules_repo.setup_branch(module_branch)
+
+        # Set the diff filename based on the module name
+        patch_filename = f"{module.replace('/', '-')}.diff"
+        module_relpath = Path("modules", module_dir, module)
+        patch_relpath = Path(module_relpath, patch_filename)
+        patch_path = Path(self.dir, patch_relpath)
+        module_path = Path(self.dir, module_relpath)
+
+        if patch_path.exists():
+            remove = questionary.confirm(
+                f"Patch exists for module '{module_fullname}'. Are you sure you want to remove?",
+                style=nf_core.utils.nfcore_question_style,
+            ).unsafe_ask()
+            if not remove:
+                return
+
+        # Try to apply the patch in reverse and move resulting files to module dir
+        temp_module_dir = self.modules_json.try_apply_patch_reverse(
+            module, self.modules_repo.repo_path, patch_relpath, module_path
+        )
+        try:
+            for file in Path(temp_module_dir).glob("*"):
+                file.rename(module_path.joinpath(file.name))
+            os.rmdir(temp_module_dir)
+        except Exception as err:
+            raise UserWarning(f"There was a problem reverting the patched file: {err}")
+
+        log.info(f"Patch for {module} reverted!")
+        # Remove patch file if we could revert the patch
+        patch_path.unlink()
+        # Write changes to module.json
+        self.modules_json.remove_patch_entry(module, self.modules_repo.remote_url, module_dir)
+
+        if not all(self.modules_repo.module_files_identical(module, module_path, module_version).values()):
+            log.error(
+                f"Module files do not appear to match the remote for the commit sha in the 'module.json': {module_version}\n"
+                f"Recommend reinstalling with 'nf-core modules install --force --sha {module_version} {module}' "
+            )
```

### Comparing `nf-core-2.7.2/nf_core/modules/test_yml_builder.py` & `nf-core-2.8/nf_core/modules/test_yml_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,24 +209,17 @@
         if os.path.getsize(fname) == 0:
             return True
         try:
             with open(fname, "rb") as fh:
                 g_f = gzip.GzipFile(fileobj=fh, mode="rb")
                 if g_f.read() == b"":
                     return True
-        except Exception as e:
-            # Python 3.8+
-            if hasattr(gzip, "BadGzipFile"):
-                if isinstance(e, gzip.BadGzipFile):
-                    pass
-            # Python 3.7
-            elif isinstance(e, OSError):
-                pass
-            else:
-                raise e
+        except gzip.BadGzipFile:
+            pass
+
         return False
 
     def _md5(self, fname):
         """Generate md5 sum for file"""
         hash_md5 = hashlib.md5()
         with open(fname, "rb") as f:
             for chunk in iter(lambda: f.read(io.DEFAULT_BUFFER_SIZE), b""):
```

### Comparing `nf-core-2.7.2/nf_core/modules/update.py` & `nf-core-2.8/nf_core/modules/update.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.devcontainer/devcontainer.json` & `nf-core-2.8/nf_core/pipeline-template/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/CONTRIBUTING.md` & `nf-core-2.8/nf_core/pipeline-template/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     id: system
     attributes:
       label: System information
       description: |
         * Nextflow version _(eg. 22.10.1)_
         * Hardware _(eg. HPC, Desktop, Cloud)_
         * Executor _(eg. slurm, local, awsbatch)_
-        * Container engine: _(e.g. Docker, Singularity, Conda, Podman, Shifter or Charliecloud)_
+        * Container engine: _(e.g. Docker, Singularity, Conda, Podman, Shifter, Charliecloud, or Apptainer)_
         * OS _(eg. CentOS Linux, macOS, Linux Mint)_
         * Version of {{ name }} _(eg. 1.1, 1.5, 1.8.2)_
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `nf-core-2.8/nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 -->
 
 ## PR checklist
 
 - [ ] This comment contains a description of changes (with reason).
 - [ ] If you've fixed a bug or added code that should be tested, add tests!
 - [ ] If you've added a new tool - have you followed the pipeline conventions in the [contribution docs](https://github.com/{{ name }}/tree/master/.github/CONTRIBUTING.md)
-      {%- if branded -%}
-- [ ] If necessary, also make a PR on the {{ name }} _branch_ on the [nf-core/test-datasets](https://github.com/nf-core/test-datasets) repository.{% endif %}
+      {%- if branded %}
+- [ ] If necessary, also make a PR on the {{ name }} _branch_ on the [nf-core/test-datasets](https://github.com/nf-core/test-datasets) repository.
+      {%- endif %}
 - [ ] Make sure your code lints (`nf-core lint`).
 - [ ] Ensure the test suite passes (`nextflow run . -profile test,docker --outdir <OUTDIR>`).
 - [ ] Usage Documentation in `docs/usage.md` is updated.
 - [ ] Output Documentation in `docs/output.md` is updated.
 - [ ] `CHANGELOG.md` is updated.
 - [ ] `README.md` is updated (including new tool citations and authors/contributors).
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/awsfulltest.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/awsfulltest.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   run-tower:
     name: Run AWS full tests
     if: github.repository == '{{ name }}'
     runs-on: ubuntu-latest
     steps:
       - name: Launch workflow via tower
-        uses: nf-core/tower-action@v3
+        uses: seqeralabs/action-tower-launch@v1
         # TODO nf-core: You can customise AWS full pipeline tests as required
         # Add full size test data (but still relatively small datasets for few samples)
         # on the `test_full.config` test runs with only one set of parameters {%- raw %}
         with:
           workspace_id: ${{ secrets.TOWER_WORKSPACE_ID }}
           access_token: ${{ secrets.TOWER_ACCESS_TOKEN }}
           compute_env: ${{ secrets.TOWER_COMPUTE_ENV }}
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/awstest.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/awstest.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   run-tower:
     name: Run AWS tests
     if: github.repository == '{{ name }}'
     runs-on: ubuntu-latest
     steps:
       # Launch workflow using Tower CLI tool action {%- raw %}
       - name: Launch workflow via tower
-        uses: nf-core/tower-action@v3
+        uses: seqeralabs/action-tower-launch@v1
         with:
           workspace_id: ${{ secrets.TOWER_WORKSPACE_ID }}
           access_token: ${{ secrets.TOWER_ACCESS_TOKEN }}
           compute_env: ${{ secrets.TOWER_COMPUTE_ENV }}
           workdir: s3://${{ secrets.AWS_S3_BUCKET }}{% endraw %}/work/{{ short_name }}/{% raw %}work-${{ github.sha }}{% endraw %}
           parameters: |
             {
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/branch.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/branch.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   test:
     runs-on: ubuntu-latest
     steps:
       # PRs to the nf-core repo master branch are only ok if coming from the nf-core repo `dev` or any `patch` branches
       - name: Check PRs
         if: github.repository == '{{ name }}'
         run: |
-          { [[ {% raw %}${{github.event.pull_request.head.repo.full_name }}{% endraw %} == {{ name }} ]] && [[ $GITHUB_HEAD_REF = "dev" ]]; } || [[ $GITHUB_HEAD_REF == "patch" ]]
+          { [[ {% raw %}${{github.event.pull_request.head.repo.full_name }}{% endraw %} == {{ name }} ]] && [[ $GITHUB_HEAD_REF == "dev" ]]; } || [[ $GITHUB_HEAD_REF == "patch" ]]
 
       # If the above check failed, post a comment on the PR explaining the failure {%- raw %}
       # NOTE - this doesn't currently work if the PR is coming from a fork, due to limitations in GitHub actions secrets
       - name: Post PR comment
         if: failure()
         uses: mshick/add-pr-comment@v1
         with:
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/ci.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/fix-linting.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/fix-linting.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/linting.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting.yml`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         uses: actions/checkout@v3
 
       - name: Install Nextflow
         uses: nf-core/setup-nextflow@v1
 
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.7"
+          python-version: "3.8"
           architecture: "x64"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install nf-core
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.github/workflows/linting_comment.yml` & `nf-core-2.8/nf_core/pipeline-template/.github/workflows/linting_comment.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/.gitpod.yml` & `nf-core-2.8/nf_core/pipeline-template/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/CITATIONS.md` & `nf-core-2.8/nf_core/pipeline-template/CITATIONS.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/CODE_OF_CONDUCT.md` & `nf-core-2.8/nf_core/pipeline-template/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/LICENSE` & `nf-core-2.8/nf_core/pipeline-template/LICENSE`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/adaptivecard.json` & `nf-core-2.8/nf_core/pipeline-template/assets/adaptivecard.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/email_template.html` & `nf-core-2.8/nf_core/pipeline-template/assets/email_template.html`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/email_template.txt` & `nf-core-2.8/nf_core/pipeline-template/assets/email_template.txt`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/methods_description_template.yml` & `nf-core-2.8/nf_core/pipeline-template/assets/methods_description_template.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/multiqc_config.yml` & `nf-core-2.8/nf_core/pipeline-template/assets/multiqc_config.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/schema_input.json` & `nf-core-2.8/nf_core/pipeline-template/assets/schema_input.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/sendmail_template.txt` & `nf-core-2.8/nf_core/pipeline-template/assets/sendmail_template.txt`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/assets/slackreport.json` & `nf-core-2.8/nf_core/pipeline-template/assets/slackreport.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/bin/check_samplesheet.py` & `nf-core-2.8/nf_core/pipeline-template/bin/check_samplesheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,17 +154,14 @@
     .. _text file:
         https://docs.python.org/3/glossary.html#term-text-file
 
     """
     peek = read_head(handle)
     handle.seek(0)
     sniffer = csv.Sniffer()
-    if not sniffer.has_header(peek):
-        logger.critical("The given sample sheet does not appear to contain a header.")
-        sys.exit(1)
     dialect = sniffer.sniff(peek)
     return dialect
 
 
 def check_samplesheet(file_in, file_out):
     """
     Check that the tabular samplesheet has the structure expected by nf-core pipelines.
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/conf/base.config` & `nf-core-2.8/nf_core/pipeline-template/conf/base.config`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 process {
 
     // TODO nf-core: Check the defaults for all processes
     cpus   = { check_max( 1    * task.attempt, 'cpus'   ) }
     memory = { check_max( 6.GB * task.attempt, 'memory' ) }
     time   = { check_max( 4.h  * task.attempt, 'time'   ) }
 
-    errorStrategy = { task.exitStatus in [143,137,104,134,139] ? 'retry' : 'finish' }
+    errorStrategy = { task.exitStatus in ((130..145) + 104) ? 'retry' : 'finish' }
     maxRetries    = 1
     maxErrors     = '-1'
 
     // Process-specific resource requirements
     // NOTE - Please try and re-use the labels below as much as possible.
     //        These labels are used and recognised by default in DSL2 files hosted on nf-core/modules.
     //        If possible, it would be nice to keep the same label naming convention when
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/conf/igenomes.config` & `nf-core-2.8/nf_core/pipeline-template/conf/igenomes.config`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,22 @@
             bismark     = "${params.igenomes_base}/Homo_sapiens/NCBI/GRCh38/Sequence/BismarkIndex/"
             gtf         = "${params.igenomes_base}/Homo_sapiens/NCBI/GRCh38/Annotation/Genes/genes.gtf"
             bed12       = "${params.igenomes_base}/Homo_sapiens/NCBI/GRCh38/Annotation/Genes/genes.bed"
             mito_name   = "chrM"
             macs_gsize  = "2.7e9"
             blacklist   = "${projectDir}/assets/blacklists/hg38-blacklist.bed"
         }
+        'CHM13' {
+            fasta       = "${params.igenomes_base}/Homo_sapiens/UCSC/CHM13/Sequence/WholeGenomeFasta/genome.fa"
+            bwa         = "${params.igenomes_base}/Homo_sapiens/UCSC/CHM13/Sequence/BWAIndex/"
+            bwamem2     = "${params.igenomes_base}/Homo_sapiens/UCSC/CHM13/Sequence/BWAmem2Index/"
+            gtf         = "${params.igenomes_base}/Homo_sapiens/NCBI/CHM13/Annotation/Genes/genes.gtf"
+            gff         = "ftp://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/009/914/755/GCF_009914755.1_T2T-CHM13v2.0/GCF_009914755.1_T2T-CHM13v2.0_genomic.gff.gz"
+            mito_name   = "chrM"
+        }
         'GRCm38' {
             fasta       = "${params.igenomes_base}/Mus_musculus/Ensembl/GRCm38/Sequence/WholeGenomeFasta/genome.fa"
             bwa         = "${params.igenomes_base}/Mus_musculus/Ensembl/GRCm38/Sequence/BWAIndex/version0.6.0/"
             bowtie2     = "${params.igenomes_base}/Mus_musculus/Ensembl/GRCm38/Sequence/Bowtie2Index/"
             star        = "${params.igenomes_base}/Mus_musculus/Ensembl/GRCm38/Sequence/STARIndex/"
             bismark     = "${params.igenomes_base}/Mus_musculus/Ensembl/GRCm38/Sequence/BismarkIndex/"
             gtf         = "${params.igenomes_base}/Mus_musculus/Ensembl/GRCm38/Annotation/Genes/genes.gtf"
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/conf/modules.config` & `nf-core-2.8/nf_core/pipeline-template/conf/modules.config`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/conf/test.config` & `nf-core-2.8/nf_core/pipeline-template/conf/test.config`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/conf/test_full.config` & `nf-core-2.8/nf_core/pipeline-template/conf/test_full.config`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
     Use as follows:
         nextflow run {{ name }} -profile test_full,<docker/singularity> --outdir <OUTDIR>
 
 ----------------------------------------------------------------------------------------
 */
 
+cleanup = true
+
 params {
     config_profile_name        = 'Full test profile'
     config_profile_description = 'Full test dataset to check pipeline function'
 
     // Input data for full size test
     // TODO nf-core: Specify the paths to your full test data ( on nf-core/test-datasets or directly in repositories, e.g. SRA)
     // TODO nf-core: Give any required params for the test so that command line flags are not needed
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/docs/README.md` & `nf-core-2.8/nf_core/pipeline-template/docs/README.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png` & `nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_adapter.png`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png` & `nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_counts.png`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png` & `nf-core-2.8/nf_core/pipeline-template/docs/images/mqc_fastqc_quality.png`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/docs/output.md` & `nf-core-2.8/nf_core/pipeline-template/docs/output.md`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/docs/usage.md` & `nf-core-2.8/nf_core/pipeline-template/docs/usage.md`

 * *Files 18% similar despite different names*

```diff
@@ -71,14 +71,37 @@
 ```bash
 work                # Directory containing the nextflow working files
 <OUTDIR>            # Finished results in specified location (defined with --outdir)
 .nextflow_log       # Log file from Nextflow
 # Other nextflow hidden files, eg. history of pipeline runs and old logs.
 ```
 
+If you wish to repeatedly use the same parameters for multiple runs, rather than specifying each flag in the command, you can specify these in a params file.
+
+Pipeline settings can be provided in a `yaml` or `json` file via `-params-file <file>`.
+
+> ⚠️ Do not use `-c <file>` to specify parameters as this will result in errors. Custom config files specified with `-c` must only be used for [tuning process resource specifications](https://nf-co.re/docs/usage/configuration#tuning-workflow-resources), other infrastructural tweaks (such as output directories), or module arguments (args).
+> The above pipeline run specified with a params file in yaml format:
+
+```bash
+nextflow run {{ name }} -profile docker -params-file params.yaml
+```
+
+with `params.yaml` containing:
+
+```yaml
+input: './samplesheet.csv'
+outdir: './results/'
+genome: 'GRCh37'
+input: 'data'
+<...>
+```
+
+You can also generate such `YAML`/`JSON` files via [nf-core/launch](https://nf-co.re/launch).
+
 ### Updating the pipeline
 
 When you run the above command, Nextflow automatically pulls the pipeline code from GitHub and stores it as a cached version. When running the pipeline after this, it will always use the cached version if available - even if the pipeline has been updated since. To make sure that you're running the latest version of the pipeline, make sure that you regularly update the cached version of the pipeline:
 
 ```bash
 nextflow pull {{ name }}
 ```
@@ -87,23 +110,27 @@
 
 It is a good idea to specify a pipeline version when running the pipeline on your data. This ensures that a specific version of the pipeline code and software are used when you run your pipeline. If you keep using the same tag, you'll be running the same version of the pipeline, even if there have been changes to the code since.
 
 First, go to the [{{ name }} releases page](https://github.com/{{ name }}/releases) and find the latest pipeline version - numeric only (eg. `1.3.1`). Then specify this when running the pipeline with `-r` (one hyphen) - eg. `-r 1.3.1`. Of course, you can switch to another version by changing the number after the `-r` flag.
 
 This version number will be logged in reports when you run the pipeline, so that you'll know what you used when you look back in the future. For example, at the bottom of the MultiQC reports.
 
+To further assist in reproducbility, you can use share and re-use [parameter files](#running-the-pipeline) to repeat pipeline runs with the same settings without having to write out a command with every single parameter.
+
+> 💡 If you wish to share such profile (such as upload as supplementary material for academic publications), make sure to NOT include cluster specific paths to files, nor institutional specific profiles.
+
 ## Core Nextflow arguments
 
 > **NB:** These options are part of Nextflow and use a _single_ hyphen (pipeline parameters use a double-hyphen).
 
 ### `-profile`
 
 Use this parameter to choose a configuration profile. Profiles can give configuration presets for different compute environments.
 
-Several generic profiles are bundled with the pipeline which instruct the pipeline to use software packaged using different methods (Docker, Singularity, Podman, Shifter, Charliecloud, Conda) - see below.
+Several generic profiles are bundled with the pipeline which instruct the pipeline to use software packaged using different methods (Docker, Singularity, Podman, Shifter, Charliecloud, Apptainer, Conda) - see below.
 
 > We highly recommend the use of Docker or Singularity containers for full pipeline reproducibility, however when this is not possible, Conda is also supported.
 
 {%- if nf_core_configs %}
 
 The pipeline also dynamically loads configurations from [https://github.com/nf-core/configs](https://github.com/nf-core/configs) when it runs, making multiple config profiles for various institutional clusters available at run time. For more information and to see if your system is available in these configs please see the [nf-core/configs documentation](https://github.com/nf-core/configs#documentation).
 {% else %}
@@ -122,16 +149,18 @@
   - A generic configuration profile to be used with [Singularity](https://sylabs.io/docs/)
 - `podman`
   - A generic configuration profile to be used with [Podman](https://podman.io/)
 - `shifter`
   - A generic configuration profile to be used with [Shifter](https://nersc.gitlab.io/development/shifter/how-to-use/)
 - `charliecloud`
   - A generic configuration profile to be used with [Charliecloud](https://hpc.github.io/charliecloud/)
+- `apptainer`
+  - A generic configuration profile to be used with [Apptainer](https://apptainer.org/)
 - `conda`
-  - A generic configuration profile to be used with [Conda](https://conda.io/docs/). Please only use Conda as a last resort i.e. when it's not possible to run the pipeline with Docker, Singularity, Podman, Shifter or Charliecloud.
+  - A generic configuration profile to be used with [Conda](https://conda.io/docs/). Please only use Conda as a last resort i.e. when it's not possible to run the pipeline with Docker, Singularity, Podman, Shifter, Charliecloud, or Apptainer.
 
 ### `-resume`
 
 Specify this when restarting a pipeline. Nextflow will use cached results from any pipeline steps where the inputs are the same, continuing from where it got to previously. For input to be considered the same, not only the names must be identical but the files' contents as well. For more info about this parameter, see [this blog post](https://www.nextflow.io/blog/2019/demystifying-nextflow-resume.html).
 
 You can also supply a run name to resume a specific run: `-resume [run-name]`. Use the `nextflow log` command to show previous run names.
 
@@ -141,112 +170,28 @@
 
 ## Custom configuration
 
 ### Resource requests
 
 Whilst the default requirements set within the pipeline will hopefully work for most people and with most input data, you may find that you want to customise the compute resources that the pipeline requests. Each step in the pipeline has a default set of requirements for number of CPUs, memory and time. For most of the steps in the pipeline, if the job exits with any of the error codes specified [here](https://github.com/nf-core/rnaseq/blob/4c27ef5610c87db00c3c5a3eed10b1d161abf575/conf/base.config#L18) it will automatically be resubmitted with higher requests (2 x original, then 3 x original). If it still fails after the third attempt then the pipeline execution is stopped.
 
-For example, if the nf-core/rnaseq pipeline is failing after multiple re-submissions of the `STAR_ALIGN` process due to an exit code of `137` this would indicate that there is an out of memory issue:
-
-```console
-[62/149eb0] NOTE: Process `NFCORE_RNASEQ:RNASEQ:ALIGN_STAR:STAR_ALIGN (WT_REP1)` terminated with an error exit status (137) -- Execution is retried (1)
-Error executing process > 'NFCORE_RNASEQ:RNASEQ:ALIGN_STAR:STAR_ALIGN (WT_REP1)'
-
-Caused by:
-    Process `NFCORE_RNASEQ:RNASEQ:ALIGN_STAR:STAR_ALIGN (WT_REP1)` terminated with an error exit status (137)
-
-Command executed:
-    STAR \
-        --genomeDir star \
-        --readFilesIn WT_REP1_trimmed.fq.gz  \
-        --runThreadN 2 \
-        --outFileNamePrefix WT_REP1. \
-        <TRUNCATED>
-
-Command exit status:
-    137
-
-Command output:
-    (empty)
-
-Command error:
-    .command.sh: line 9:  30 Killed    STAR --genomeDir star --readFilesIn WT_REP1_trimmed.fq.gz --runThreadN 2 --outFileNamePrefix WT_REP1. <TRUNCATED>
-Work dir:
-    /home/pipelinetest/work/9d/172ca5881234073e8d76f2a19c88fb
+To change the resource requests, please see the [max resources](https://nf-co.re/docs/usage/configuration#max-resources) and [tuning workflow resources](https://nf-co.re/docs/usage/configuration#tuning-workflow-resources) section of the nf-core website.
 
-Tip: you can replicate the issue by changing to the process work dir and entering the command `bash .command.run`
-```
-
-#### For beginners
+### Custom Containers
 
-A first step to bypass this error, you could try to increase the amount of CPUs, memory, and time for the whole pipeline. Therefor you can try to increase the resource for the parameters `--max_cpus`, `--max_memory`, and `--max_time`. Based on the error above, you have to increase the amount of memory. Therefore you can go to the [parameter documentation of rnaseq](https://nf-co.re/rnaseq/3.9/parameters) and scroll down to the `show hidden parameter` button to get the default value for `--max_memory`. In this case 128GB, you than can try to run your pipeline again with `--max_memory 200GB -resume` to skip all process, that were already calculated. If you can not increase the resource of the complete pipeline, you can try to adapt the resource for a single process as mentioned below.
+In some cases you may wish to change which container or conda environment a step of the pipeline uses for a particular tool. By default nf-core pipelines use containers and software from the [biocontainers](https://biocontainers.pro/) or [bioconda](https://bioconda.github.io/) projects. However in some cases the pipeline specified version maybe out of date.
 
-#### Advanced option on process level
-
-To bypass this error you would need to find exactly which resources are set by the `STAR_ALIGN` process. The quickest way is to search for `process STAR_ALIGN` in the [nf-core/rnaseq Github repo](https://github.com/nf-core/rnaseq/search?q=process+STAR_ALIGN).
-We have standardised the structure of Nextflow DSL2 pipelines such that all module files will be present in the `modules/` directory and so, based on the search results, the file we want is `modules/nf-core/star/align/main.nf`.
-If you click on the link to that file you will notice that there is a `label` directive at the top of the module that is set to [`label process_high`](https://github.com/nf-core/rnaseq/blob/4c27ef5610c87db00c3c5a3eed10b1d161abf575/modules/nf-core/software/star/align/main.nf#L9).
-The [Nextflow `label`](https://www.nextflow.io/docs/latest/process.html#label) directive allows us to organise workflow processes in separate groups which can be referenced in a configuration file to select and configure subset of processes having similar computing requirements.
-The default values for the `process_high` label are set in the pipeline's [`base.config`](https://github.com/nf-core/rnaseq/blob/4c27ef5610c87db00c3c5a3eed10b1d161abf575/conf/base.config#L33-L37) which in this case is defined as 72GB.
-Providing you haven't set any other standard nf-core parameters to **cap** the [maximum resources](https://nf-co.re/usage/configuration#max-resources) used by the pipeline then we can try and bypass the `STAR_ALIGN` process failure by creating a custom config file that sets at least 72GB of memory, in this case increased to 100GB.
-The custom config below can then be provided to the pipeline via the [`-c`](#-c) parameter as highlighted in previous sections.
-
-```nextflow
-process {
-    withName: 'NFCORE_RNASEQ:RNASEQ:ALIGN_STAR:STAR_ALIGN' {
-        memory = 100.GB
-    }
-}
-```
+To use a different container from the default container or conda environment specified in a pipeline, please see the [updating tool versions](https://nf-co.re/docs/usage/configuration#updating-tool-versions) section of the nf-core website.
 
-> **NB:** We specify the full process name i.e. `NFCORE_RNASEQ:RNASEQ:ALIGN_STAR:STAR_ALIGN` in the config file because this takes priority over the short name (`STAR_ALIGN`) and allows existing configuration using the full process name to be correctly overridden.
->
-> If you get a warning suggesting that the process selector isn't recognised check that the process name has been specified correctly.
-
-### Updating containers (advanced users)
-
-The [Nextflow DSL2](https://www.nextflow.io/docs/latest/dsl2.html) implementation of this pipeline uses one container per process which makes it much easier to maintain and update software dependencies. If for some reason you need to use a different version of a particular tool with the pipeline then you just need to identify the `process` name and override the Nextflow `container` definition for that process using the `withName` declaration. For example, in the [nf-core/viralrecon](https://nf-co.re/viralrecon) pipeline a tool called [Pangolin](https://github.com/cov-lineages/pangolin) has been used during the COVID-19 pandemic to assign lineages to SARS-CoV-2 genome sequenced samples. Given that the lineage assignments change quite frequently it doesn't make sense to re-release the nf-core/viralrecon everytime a new version of Pangolin has been released. However, you can override the default container used by the pipeline by creating a custom config file and passing it as a command-line argument via `-c custom.config`.
-
-1. Check the default version used by the pipeline in the module file for [Pangolin](https://github.com/nf-core/viralrecon/blob/a85d5969f9025409e3618d6c280ef15ce417df65/modules/nf-core/software/pangolin/main.nf#L14-L19)
-2. Find the latest version of the Biocontainer available on [Quay.io](https://quay.io/repository/biocontainers/pangolin?tag=latest&tab=tags)
-3. Create the custom config accordingly:
-
-   - For Docker:
-
-     ```nextflow
-     process {
-         withName: PANGOLIN {
-             container = 'quay.io/biocontainers/pangolin:3.0.5--pyhdfd78af_0'
-         }
-     }
-     ```
-
-   - For Singularity:
-
-     ```nextflow
-     process {
-         withName: PANGOLIN {
-             container = 'https://depot.galaxyproject.org/singularity/pangolin:3.0.5--pyhdfd78af_0'
-         }
-     }
-     ```
-
-   - For Conda:
-
-     ```nextflow
-     process {
-         withName: PANGOLIN {
-             conda = 'bioconda::pangolin=3.0.5'
-         }
-     }
-     ```
+### Custom Tool Arguments
 
-> **NB:** If you wish to periodically update individual tool-specific results (e.g. Pangolin) generated by the pipeline then you must ensure to keep the `work/` directory otherwise the `-resume` ability of the pipeline will be compromised and it will restart from scratch.
+A pipeline might not always support every possible argument or option of a particular tool used in pipeline. Fortunately, nf-core pipelines provide some freedom to users to insert additional parameters that the pipeline does not include by default.
 
 {% if nf_core_configs -%}
+To learn how to provide additional arguments to a particular tool of the pipeline, please see the [customising tool arguments](https://nf-co.re/docs/usage/configuration#customising-tool-arguments) section of the nf-core website.
 
 ### nf-core/configs
 
 In most cases, you will only need to create a custom config as a one-off but if you and others within your organisation are likely to be running nf-core pipelines regularly and need to use the same settings regularly it may be a good idea to request that your custom config file is uploaded to the `nf-core/configs` git repository. Before you do this please can you test that the config file works with your pipeline of choice using the `-c` parameter. You can then create a pull request to the `nf-core/configs` repository with the addition of your config file, associated documentation file (see examples in [`nf-core/configs/docs`](https://github.com/nf-core/configs/tree/master/docs)), and amending [`nfcore_custom.config`](https://github.com/nf-core/configs/blob/master/nfcore_custom.config) to include your custom profile.
 
 See the main [Nextflow documentation](https://www.nextflow.io/docs/latest/config.html) for more information about creating your own configuration files.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/lib/NfcoreSchema.groovy` & `nf-core-2.8/nf_core/pipeline-template/lib/NfcoreSchema.groovy`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 //
 // This file holds several functions used to perform JSON parameter validation, help and summary rendering for the nf-core pipeline template.
 //
 
+import nextflow.Nextflow
 import org.everit.json.schema.Schema
 import org.everit.json.schema.loader.SchemaLoader
 import org.everit.json.schema.ValidationException
 import org.json.JSONObject
 import org.json.JSONTokener
 import org.json.JSONArray
 import groovy.json.JsonSlurper
@@ -79,14 +80,15 @@
             'resume',
             'revision',
             'stdin',
             'stub',
             'stub-run',
             'test',
             'w',
+            'with-apptainer',
             'with-charliecloud',
             'with-conda',
             'with-dag',
             'with-docker',
             'with-mpi',
             'with-notification',
             'with-podman',
@@ -173,15 +175,15 @@
             }
             log.warn warn_msg
             log.info "- ${colors.dim}Ignore this warning: params.schema_ignore_params = \"${unexpectedParams.join(',')}\" ${colors.reset}"
             println ''
         }
 
         if (has_error) {
-            System.exit(1)
+            Nextflow.error('Exiting!')
         }
     }
 
     //
     // Beautify parameters for --help
     //
     public static String paramsHelp(workflow, params, command, schema_filename='nextflow_schema.json') {
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/lib/NfcoreTemplate.groovy` & `nf-core-2.8/nf_core/pipeline-template/lib/NfcoreTemplate.groovy`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/lib/Utils.groovy` & `nf-core-2.8/nf_core/pipeline-template/lib/Utils.groovy`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/lib/WorkflowMain.groovy` & `nf-core-2.8/nf_core/pipeline-template/lib/WorkflowMain.groovy`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 //
 // This file holds several functions specific to the main.nf workflow in the {{ name }} pipeline
 //
 
+import nextflow.Nextflow
+
 class WorkflowMain {
 
     //
     // Citation string for pipeline
     //
     public static String citation(workflow) {
         return "If you use ${workflow.manifest.name} for your analysis please cite:\n\n" +
@@ -17,15 +19,15 @@
             "* Software dependencies\n" +
             "  https://github.com/${workflow.manifest.name}/blob/master/CITATIONS.md"
     }
 
     //
     // Generate help string
     //
-    public static String help(workflow, params, log) {
+    public static String help(workflow, params) {
         {% if igenomes -%}
         def command = "nextflow run ${workflow.manifest.name} --input samplesheet.csv --genome GRCh37 -profile docker"
         {% else -%}
         def command = "nextflow run ${workflow.manifest.name} --input samplesheet.csv --fasta reference.fa -profile docker"
         {% endif -%}
         def help_string = ''
         help_string += NfcoreTemplate.logo(workflow, params.monochrome_logs)
@@ -34,42 +36,42 @@
         help_string += NfcoreTemplate.dashedLine(params.monochrome_logs)
         return help_string
     }
 
     //
     // Generate parameter summary log string
     //
-    public static String paramsSummaryLog(workflow, params, log) {
+    public static String paramsSummaryLog(workflow, params) {
         def summary_log = ''
         summary_log += NfcoreTemplate.logo(workflow, params.monochrome_logs)
         summary_log += NfcoreSchema.paramsSummaryLog(workflow, params)
         summary_log += '\n' + citation(workflow) + '\n'
         summary_log += NfcoreTemplate.dashedLine(params.monochrome_logs)
         return summary_log
     }
 
     //
     // Validate parameters and print summary to screen
     //
     public static void initialise(workflow, params, log) {
         // Print help to screen if required
         if (params.help) {
-            log.info help(workflow, params, log)
+            log.info help(workflow, params)
             System.exit(0)
         }
 
         // Print workflow version and exit on --version
         if (params.version) {
             String workflow_version = NfcoreTemplate.version(workflow)
             log.info "${workflow.manifest.name} ${workflow_version}"
             System.exit(0)
         }
 
         // Print parameter summary log to screen
-        log.info paramsSummaryLog(workflow, params, log)
+        log.info paramsSummaryLog(workflow, params)
 
         // Validate workflow parameters via the JSON schema
         if (params.validate_params) {
             NfcoreSchema.validateParameters(workflow, params, log)
         }
 
         // Check that a -profile or Nextflow config has been provided to run the pipeline
@@ -81,16 +83,15 @@
         }
 
         // Check AWS batch settings
         NfcoreTemplate.awsBatch(workflow, params)
 
         // Check input has been provided
         if (!params.input) {
-            log.error "Please provide an input samplesheet to the pipeline e.g. '--input samplesheet.csv'"
-            System.exit(1)
+            Nextflow.error("Please provide an input samplesheet to the pipeline e.g. '--input samplesheet.csv'")
         }
     }
     {% if igenomes -%}
 
     //
     // Get attribute from genome config file e.g. fasta
     //
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/lib/WorkflowPipeline.groovy` & `nf-core-2.8/nf_core/pipeline-template/lib/WorkflowPipeline.groovy`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 //
 // This file holds several functions specific to the workflow/{{ short_name }}.nf in the {{ name }} pipeline
 //
 
+import nextflow.Nextflow
 import groovy.text.SimpleTemplateEngine
 
 class Workflow{{ short_name[0]|upper }}{{ short_name[1:] }} {
 
     //
     // Check and validate parameters
     //
     public static void initialise(params, log) {
         {% if igenomes -%}
         genomeExistsError(params, log)
 {% endif %}
 
         if (!params.fasta) {
-            log.error "Genome fasta file not specified with e.g. '--fasta genome.fa' or via a detectable config file."
-            System.exit(1)
+            Nextflow.error "Genome fasta file not specified with e.g. '--fasta genome.fa' or via a detectable config file."
         }
     }
 
     //
     // Get workflow summary for MultiQC
     //
     public static String paramsSummaryMultiqc(workflow, summary) {
@@ -59,23 +59,23 @@
         def methods_text = mqc_methods_yaml.text
 
         def engine =  new SimpleTemplateEngine()
         def description_html = engine.createTemplate(methods_text).make(meta)
 
         return description_html
     }
+    {%- if igenomes %}
 
-    {%- if igenomes -%}
     //
     // Exit pipeline if incorrect --genome key provided
     //
     private static void genomeExistsError(params, log) {
         if (params.genomes && params.genome && !params.genomes.containsKey(params.genome)) {
-            log.error "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n" +
+            def error_string = "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n" +
                 "  Genome '${params.genome}' not found in any config files provided to the pipeline.\n" +
                 "  Currently, the available genome keys are:\n" +
                 "  ${params.genomes.keySet().join(", ")}\n" +
                 "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"
-            System.exit(1)
+            Nextflow.error(error_string)
         }
     }
 {% endif -%}}
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar` & `nf-core-2.8/nf_core/pipeline-template/lib/nfcore_external_java_deps.jar`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/main.nf` & `nf-core-2.8/nf_core/pipeline-template/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env nextflow
 /*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     {{ name }}
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     Github : https://github.com/{{ name }}
-{% if branded %}
+{%- if branded %}
     Website: https://nf-co.re/{{ short_name }}
     Slack  : https://nfcore.slack.com/channels/{{ short_name }}
 {% endif -%}
 ----------------------------------------------------------------------------------------
 */
 
 nextflow.enable.dsl = 2
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/main.nf`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 process CUSTOM_DUMPSOFTWAREVERSIONS {
     label 'process_single'
 
     // Requires `pyyaml` which does not have a dedicated container but is in the MultiQC container
-    conda "bioconda::multiqc=1.13"
+    conda "bioconda::multiqc=1.14"
     container "${ workflow.containerEngine == 'singularity' && !task.ext.singularity_pull_docker_container ?
-        'https://depot.galaxyproject.org/singularity/multiqc:1.13--pyhdfd78af_0' :
-        'quay.io/biocontainers/multiqc:1.13--pyhdfd78af_0' }"
+        'https://depot.galaxyproject.org/singularity/multiqc:1.14--pyhdfd78af_0' :
+        'quay.io/biocontainers/multiqc:1.14--pyhdfd78af_0' }"
 
     input:
     path versions
 
     output:
     path "software_versions.yml"    , emit: yml
     path "software_versions_mqc.yml", emit: mqc_yml
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/meta.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+# yaml-language-server: $schema=https://raw.githubusercontent.com/nf-core/modules/master/modules/yaml-schema.json
 name: custom_dumpsoftwareversions
 description: Custom module used to dump software versions within the nf-core pipeline template
 keywords:
   - custom
+  - dump
   - version
 tools:
   - custom:
       description: Custom module used to dump software versions within the nf-core pipeline template
       homepage: https://github.com/nf-core/tools
       documentation: https://github.com/nf-core/tools
       licence: ["MIT"]
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/custom/dumpsoftwareversions/templates/dumpsoftwareversions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/fastqc/meta.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 process MULTIQC {
     label 'process_single'
 
-    conda "bioconda::multiqc=1.13"
+    conda "bioconda::multiqc=1.14"
     container "${ workflow.containerEngine == 'singularity' && !task.ext.singularity_pull_docker_container ?
-        'https://depot.galaxyproject.org/singularity/multiqc:1.13--pyhdfd78af_0' :
-        'quay.io/biocontainers/multiqc:1.13--pyhdfd78af_0' }"
+        'https://depot.galaxyproject.org/singularity/multiqc:1.14--pyhdfd78af_0' :
+        'quay.io/biocontainers/multiqc:1.14--pyhdfd78af_0' }"
 
     input:
     path  multiqc_files, stageAs: "?/*"
     path(multiqc_config)
     path(extra_multiqc_config)
     path(multiqc_logo)
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml` & `nf-core-2.8/nf_core/pipeline-template/modules/nf-core/multiqc/meta.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# yaml-language-server: $schema=https://raw.githubusercontent.com/nf-core/modules/master/modules/yaml-schema.json
 name: MultiQC
 description: Aggregate results from bioinformatics analyses across many samples into a single report
 keywords:
   - QC
   - bioinformatics tools
   - Beautiful stand-alone HTML report
 tools:
@@ -33,15 +34,15 @@
 
 output:
   - report:
       type: file
       description: MultiQC report file
       pattern: "multiqc_report.html"
   - data:
-      type: dir
+      type: directory
       description: MultiQC data dir
       pattern: "multiqc_data"
   - plots:
       type: file
       description: Plots created by MultiQC
       pattern: "*_data"
   - versions:
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/modules.json` & `nf-core-2.8/nf_core/pipeline-template/modules.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'repos'": "{'https://github.com/nf-core/modules.git': {'modules': {'nf-core': "*

 * *            "{'custom/dumpsoftwareversions': {'git_sha': "*

 * *            "'76cc4938c1f6ea5c7d83fed1eeffc146787f9543'}, 'multiqc': {'git_sha': "*

 * *            "'f2d63bd5b68925f98f572eed70993d205cc694b7'}}}}}"}*

```diff
@@ -3,29 +3,29 @@
     "name": "{{ name }}",
     "repos": {
         "https://github.com/nf-core/modules.git": {
             "modules": {
                 "nf-core": {
                     "custom/dumpsoftwareversions": {
                         "branch": "master",
-                        "git_sha": "c8e35eb2055c099720a75538d1b8adb3fb5a464c",
+                        "git_sha": "76cc4938c1f6ea5c7d83fed1eeffc146787f9543",
                         "installed_by": [
                             "modules"
                         ]
                     },
                     "fastqc": {
                         "branch": "master",
                         "git_sha": "c8e35eb2055c099720a75538d1b8adb3fb5a464c",
                         "installed_by": [
                             "modules"
                         ]
                     },
                     "multiqc": {
                         "branch": "master",
-                        "git_sha": "c8e35eb2055c099720a75538d1b8adb3fb5a464c",
+                        "git_sha": "f2d63bd5b68925f98f572eed70993d205cc694b7",
                         "installed_by": [
                             "modules"
                         ]
                     }
                 }
             }
         }
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/nextflow.config` & `nf-core-2.8/nf_core/pipeline-template/nextflow.config`

 * *Files 19% similar despite different names*

```diff
@@ -77,71 +77,98 @@
 //   includeConfig "${params.custom_config_base}/pipeline/{{ short_name }}.config"
 // } catch (Exception e) {
 //   System.err.println("WARNING: Could not load nf-core/config/{{ short_name }} profiles: ${params.custom_config_base}/pipeline/{{ short_name }}.config")
 // }
 {% endif %}
 
 profiles {
-    debug { process.beforeScript = 'echo $HOSTNAME' }
+    debug {
+        dumpHashes             = true
+        process.beforeScript   = 'echo $HOSTNAME'
+        cleanup = false
+    }
     conda {
         conda.enabled          = true
         docker.enabled         = false
         singularity.enabled    = false
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
+        apptainer.enabled      = false
     }
     mamba {
         conda.enabled          = true
         conda.useMamba         = true
         docker.enabled         = false
         singularity.enabled    = false
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
+        apptainer.enabled      = false
     }
     docker {
         docker.enabled         = true
+        docker.registry        = 'quay.io'
         docker.userEmulation   = true
+        conda.enabled          = false
         singularity.enabled    = false
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
+        apptainer.enabled      = false
     }
     arm {
         docker.runOptions = '-u $(id -u):$(id -g) --platform=linux/amd64'
     }
     singularity {
         singularity.enabled    = true
         singularity.autoMounts = true
+        conda.enabled          = false
         docker.enabled         = false
         podman.enabled         = false
         shifter.enabled        = false
         charliecloud.enabled   = false
+        apptainer.enabled      = false
     }
     podman {
         podman.enabled         = true
+        podman.registry        = 'quay.io'
+        conda.enabled          = false
         docker.enabled         = false
         singularity.enabled    = false
         shifter.enabled        = false
         charliecloud.enabled   = false
+        apptainer.enabled      = false
     }
     shifter {
         shifter.enabled        = true
+        conda.enabled          = false
         docker.enabled         = false
         singularity.enabled    = false
         podman.enabled         = false
         charliecloud.enabled   = false
+        apptainer.enabled      = false
     }
     charliecloud {
         charliecloud.enabled   = true
+        conda.enabled          = false
         docker.enabled         = false
         singularity.enabled    = false
         podman.enabled         = false
         shifter.enabled        = false
+        apptainer.enabled      = false
+    }
+    apptainer {
+        apptainer.enabled      = true
+        conda.enabled          = false
+        docker.enabled         = false
+        singularity.enabled    = false
+        podman.enabled         = false
+        shifter.enabled        = false
+        charliecloud.enabled   = false
     }
     gitpod {
         executor.name          = 'local'
         executor.cpus          = 16
         executor.memory        = 60.GB
     }
     test      { includeConfig 'conf/test.config'      }
```

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/nextflow_schema.json` & `nf-core-2.8/nf_core/pipeline-template/nextflow_schema.json`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/subworkflows/local/input_check.nf` & `nf-core-2.8/nf_core/pipeline-template/subworkflows/local/input_check.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/pipeline-template/workflows/pipeline.nf` & `nf-core-2.8/nf_core/pipeline-template/workflows/pipeline.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/refgenie.py` & `nf-core-2.8/nf_core/refgenie.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Update a nextflow.config file with refgenie genomes
 """
 
+import json
 import logging
 import os
 import re
 from pathlib import Path
 from textwrap import dedent
 
 import rich
 import rich.traceback
+import yaml
 
 import nf_core.utils
 
 # import refgenconf
 
 
 # Set up logging
@@ -41,23 +43,28 @@
     from the refgenie config file
     Adapted from: https://github.com/refgenie/refgenie_nfcore
 
     Takes a RefGenConf object as argument
     """
     abg = rgc.list_assets_by_genome()
     genomes_str = ""
+    alias_translations = _get_alias_translation_file(rgc)
     for genome, asset_list in abg.items():
         genomes_str += f"    '{genome}' {{\n"
         for asset in asset_list:
             try:
                 pth = rgc.seek(genome, asset)
             # Catch general exception instead of refgencof exception --> no refgenconf import needed
             except Exception:
                 log.warning(f"{genome}/{asset} is incomplete, ignoring...")
             else:
+                # Translate an alias name to the alias used in the pipeline
+                if asset in alias_translations.keys():
+                    log.info(f"Translating refgenie asset alias {asset} to {alias_translations[asset]}.")
+                    asset = alias_translations[asset]
                 genomes_str += f'      {asset.ljust(20, " ")} = "{pth}"\n'
         genomes_str += "    }\n"
 
     return NF_CFG_TEMPLATE.format(content=genomes_str)
 
 
 def _update_nextflow_home_config(refgenie_genomes_config_file, nxf_home):
@@ -96,14 +103,46 @@
     else:
         # create new config and add include statement
         with open(nxf_home_config, "w") as fh:
             fh.write(include_config_string)
             log.info(f"Created new nextflow config file: {nxf_home_config}")
 
 
+def _get_alias_translation_file(rgc):
+    """
+    Read a file containing alias translations.
+
+    Alias translation file should be located in the same folder as the refgenie `genome_config.yaml` file,
+    the path is set to $REFGENIE environment variable by `refgenie init`.
+    Alias translation file should be named `alias_translations.yaml`
+
+    Input file contains the name of refgenie server aliases as keys and the name of the respective nf-core pipeline aliases as values.
+    Such as:
+    ensembl_gtf: gtf
+    star_index: star
+    """
+    translations = {}
+
+    if "REFGENIE" in os.environ:
+        refgenie_genomes_config_path = os.environ.get("REFGENIE")
+        refgenie_genomes_config_directory = Path(refgenie_genomes_config_path).parents[0]
+    elif "genome_folder" in rgc:
+        refgenie_genomes_config_directory = Path(rgc["genome_folder"])
+    else:
+        return translations
+
+    try:
+        with open(refgenie_genomes_config_directory / "alias_translations.yaml") as yaml_file:
+            translations = yaml.load(yaml_file, Loader=yaml.Loader)
+    except FileNotFoundError:
+        pass
+
+    return translations
+
+
 def update_config(rgc):
     """
     Update the genomes.config file after a local refgenie database has been updated
 
     This function is executed after running 'refgenie pull <genome>/<asset>'
     The refgenie config file is transformed into a nextflow.config file, which is used to
     overwrited the 'refgenie_genomes.config' file.
```

### Comparing `nf-core-2.7.2/nf_core/schema.py` & `nf-core-2.8/nf_core/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 from __future__ import print_function
 
 import copy
 import json
 import logging
 import os
+import tempfile
 import webbrowser
 
 import jinja2
 import jsonschema
 import markdown
+import rich.console
 import yaml
 from rich.prompt import Confirm
+from rich.syntax import Syntax
 
 import nf_core.list
 import nf_core.utils
-from nf_core.lint_utils import dump_json_with_prettier
+from nf_core.lint_utils import dump_json_with_prettier, run_prettier_on_file
 
 log = logging.getLogger(__name__)
 
 
 class PipelineSchema:
     """Class to generate a schema object with
     functions to handle pipeline JSON Schema"""
@@ -460,21 +463,29 @@
         if columns is None:
             columns = ["parameter", "description", "type,", "default", "required", "hidden"]
 
         output = self.schema_to_markdown(columns)
         if format == "html":
             output = self.markdown_to_html(output)
 
-        # Print to file
-        if output_fn:
+        with tempfile.NamedTemporaryFile(mode="w+") as fh:
+            fh.write(output)
+            run_prettier_on_file(fh.name)
+            fh.seek(0)
+            prettified_docs = fh.read()
+
+        if not output_fn:
+            console = rich.console.Console()
+            console.print("\n", Syntax(prettified_docs, format), "\n")
+        else:
             if os.path.exists(output_fn) and not force:
                 log.error(f"File '{output_fn}' exists! Please delete first, or use '--force'")
                 return
-            with open(output_fn, "w") as file:
-                file.write(output)
+            with open(output_fn, "w") as fh:
+                fh.write(prettified_docs)
                 log.info(f"Documentation written to '{output_fn}'")
 
         # Return as a string
         return output
 
     def schema_to_markdown(self, columns):
         """
@@ -482,54 +493,63 @@
         """
         out = f"# {self.schema['title']}\n\n"
         out += f"{self.schema['description']}\n"
         # Grouped parameters
         for definition in self.schema.get("definitions", {}).values():
             out += f"\n## {definition.get('title', {})}\n\n"
             out += f"{definition.get('description', '')}\n\n"
-            out += "".join([f"| {column.title()} " for column in columns])
-            out += "|\n"
-            out += "".join(["|-----------" for columns in columns])
-            out += "|\n"
-            for p_key, param in definition.get("properties", {}).items():
-                for column in columns:
-                    if column == "parameter":
-                        out += f"| `{p_key}` "
-                    elif column == "description":
-                        out += f"| {param.get('description', '')} "
-                        if param.get("help_text", "") != "":
-                            out += f"<details><summary>Help</summary><small>{param['help_text']}</small></details>"
-                    elif column == "type":
-                        out += f"| `{param.get('type', '')}` "
-                    else:
-                        out += f"| {param.get(column, '')} "
-                out += "|\n"
+            required = definition.get("required", [])
+            properties = definition.get("properties", {})
+            param_table = self.markdown_param_table(properties, required, columns)
+            out += param_table
 
         # Top-level ungrouped parameters
         if len(self.schema.get("properties", {})) > 0:
             out += "\n## Other parameters\n\n"
-            out += "".join([f"| {column.title()} " for column in columns])
-            out += "|\n"
-            out += "".join(["|-----------" for columns in columns])
-            out += "|\n"
+            required = self.schema.get("required", [])
+            properties = self.schema.get("properties", {})
+            param_table = self.markdown_param_table(properties, required, columns)
+            out += param_table
 
-            for p_key, param in self.schema.get("properties", {}).items():
-                for column in columns:
-                    if column == "parameter":
-                        out += f"| `{p_key}` "
-                    elif column == "description":
-                        out += f"| {param.get('description', '')} "
-                        if param.get("help_text", "") != "":
-                            out += f"<details><summary>Help</summary><small>{param['help_text']}</small></details>"
-                    elif column == "type":
-                        out += f"| `{param.get('type', '')}` "
-                    else:
-                        out += f"| {param.get(column, '')} "
-                out += "|\n"
+        return out
 
+    def markdown_param_table(self, properties, required, columns):
+        """Creates a markdown table for params from jsonschema properties section
+
+        Args:
+            properties (dict): A jsonschema properties dictionary
+            required (list): A list of the required fields.
+                Should come from the same level of the jsonschema as properties
+            columns (list): A list of columns to write
+
+        Returns:
+            str: A string with the markdown table
+        """
+        out = ""
+        out += "".join([f"| {column.title()} " for column in columns])
+        out += "|\n"
+        out += "".join(["|-----------" for _ in columns])
+        out += "|\n"
+        for p_key, param in properties.items():
+            for column in columns:
+                if column == "parameter":
+                    out += f"| `{p_key}` "
+                elif column == "description":
+                    desc = param.get("description", "").replace("\n", "<br>")
+                    out += f"| {desc} "
+                    if param.get("help_text", "") != "":
+                        help_txt = param["help_text"].replace("\n", "<br>")
+                        out += f"<details><summary>Help</summary><small>{help_txt}</small></details>"
+                elif column == "type":
+                    out += f"| `{param.get('type', '')}` "
+                elif column == "required":
+                    out += f"| {p_key in required or ''} "
+                else:
+                    out += f"| {param.get(column, '')} "
+            out += "|\n"
         return out
 
     def markdown_to_html(self, markdown_str):
         """
         Convert markdown to html
         """
         return markdown.markdown(markdown_str, extensions=["tables"])
```

### Comparing `nf-core-2.7.2/nf_core/subworkflow-template/subworkflows/main.nf` & `nf-core-2.8/nf_core/subworkflow-template/subworkflows/main.nf`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/subworkflow-template/subworkflows/meta.yml` & `nf-core-2.8/nf_core/subworkflow-template/subworkflows/meta.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# yaml-language-server: $schema=https://raw.githubusercontent.com/nf-core/modules/master/subworkflows/yaml-schema.json
 name: "{{ subworkflow_name }}"
 ## TODO nf-core: Add a description of the subworkflow and list keywords
 description: Sort SAM/BAM/CRAM file
 keywords:
   - sort
   - bam
   - sam
```

### Comparing `nf-core-2.7.2/nf_core/subworkflow-template/tests/main.nf` & `nf-core-2.8/nf_core/subworkflow-template/tests/main.nf`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env nextflow
 
 nextflow.enable.dsl = 2
 
 include { {{ subworkflow_name|upper }} } from '../../../../subworkflows/{{ org }}/{{ subworkflow_dir }}/main.nf'
 
-workflow test_{{ subworkflow_name }} {
+workflow test_{{ component_name_underscore }} {
     {% if has_meta %}
     input = [
         [ id:'test' ], // meta map
         file(params.test_data['sarscov2']['illumina']['test_paired_end_bam'], checkIfExists: true)
     ]
     {%- else %}
     input = file(params.test_data['sarscov2']['illumina']['test_single_end_bam'], checkIfExists: true)
```

### Comparing `nf-core-2.7.2/nf_core/subworkflow-template/tests/test.yml` & `nf-core-2.8/nf_core/subworkflow-template/tests/test.yml`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/subworkflows/install.py` & `nf-core-2.8/nf_core/subworkflows/install.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/subworkflows/subworkflows_test.py` & `nf-core-2.8/nf_core/subworkflows/subworkflows_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/subworkflows/test_yml_builder.py` & `nf-core-2.8/nf_core/subworkflows/test_yml_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         log.info(f"Looking for test workflow entry points: '{self.subworkflow_test_main}'")
         with open(self.subworkflow_test_main, "r") as fh:
             for line in fh:
                 match = re.match(r"workflow\s+(\S+)\s+{", line)
                 if match:
                     self.entry_points.append(match.group(1))
         if len(self.entry_points) == 0:
-            raise UserWarning("No workflow entry points found in 'self.module_test_main'")
+            raise UserWarning(f"No workflow entry points found in '{self.subworkflow_test_main}'")
 
     def build_all_tests(self):
         """
         Go over each entry point and build structure
         """
         for entry_point in self.entry_points:
             ep_test = self.build_single_test(entry_point)
@@ -191,15 +191,15 @@
             else:
                 while len(ep_test["tags"]) == 0:
                     prompt_tags = rich.prompt.Prompt.ask(
                         "[violet]Test tags[/] (comma separated)", default=",".join(sorted(tag_defaults))
                     ).strip()
                     ep_test["tags"] = [t.strip() for t in prompt_tags.split(",")]
 
-        ep_test["files"] = self.get_md5_sums(entry_point, ep_test["command"])
+        ep_test["files"] = self.get_md5_sums(ep_test["command"])
 
         return ep_test
 
     def parse_module_tags(self):
         """
         Parse the subworkflow test main.nf file to retrieve all imported modules for adding tags.
         """
@@ -226,24 +226,17 @@
         if os.path.getsize(fname) == 0:
             return True
         try:
             with open(fname, "rb") as fh:
                 g_f = gzip.GzipFile(fileobj=fh, mode="rb")
                 if g_f.read() == b"":
                     return True
-        except Exception as e:
-            # Python 3.8+
-            if hasattr(gzip, "BadGzipFile"):
-                if isinstance(e, gzip.BadGzipFile):
-                    pass
-            # Python 3.7
-            elif isinstance(e, OSError):
-                pass
-            else:
-                raise e
+        except gzip.BadGzipFile:
+            pass
+
         return False
 
     def _md5(self, fname):
         """Generate md5 sum for file"""
         hash_md5 = hashlib.md5()
         with open(fname, "rb") as f:
             for chunk in iter(lambda: f.read(io.DEFAULT_BUFFER_SIZE), b""):
@@ -275,15 +268,15 @@
                 test_file["path"] = file_path.replace(results_dir, "output")
                 test_files.append(test_file)
 
         test_files = sorted(test_files, key=operator.itemgetter("path"))
 
         return test_files
 
-    def get_md5_sums(self, entry_point, command, results_dir=None, results_dir_repeat=None):
+    def get_md5_sums(self, command, results_dir=None, results_dir_repeat=None):
         """
         Recursively go through directories and subdirectories
         and generate tuples of (<file_path>, <md5sum>)
         returns: list of tuples
         """
 
         run_this_test = False
```

### Comparing `nf-core-2.7.2/nf_core/subworkflows/update.py` & `nf-core-2.8/nf_core/subworkflows/update.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/sync.py` & `nf-core-2.8/nf_core/sync.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/nf_core/utils.py` & `nf-core-2.8/nf_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,15 +723,16 @@
                 for k in common_keys:
                     # Get the most recent common image
                     date = max(all_docker[k]["date"], all_docker[k]["date"])
                     if docker_image is None or current_date < date:
                         docker_image = all_docker[k]["image"]
                         singularity_image = all_singularity[k]["image"]
                         current_date = date
-                return docker_image["image_name"], singularity_image["image_name"]
+                        docker_image_name = docker_image["image_name"].lstrip("quay.io/")
+                return docker_image_name, singularity_image["image_name"]
             except TypeError:
                 raise LookupError(f"Could not find docker or singularity container for {package}")
         elif response.status_code != 404:
             raise LookupError(f"Unexpected response code `{response.status_code}` for {biocontainers_api_url}")
         elif response.status_code == 404:
             raise ValueError(f"Could not find `{package}` on api.biocontainers.pro")
 
@@ -868,26 +869,24 @@
 
     wf_releases = []
     wf_branches = {}
 
     # Repo is a nf-core pipeline
     for wf in wfs.remote_workflows:
         if wf.full_name == pipeline or wf.name == pipeline:
-
             # Set to full name just in case it didn't have the nf-core/ prefix
             pipeline = wf.full_name
 
             # Store releases and stop loop
             wf_releases = list(sorted(wf.releases, key=lambda k: k.get("published_at_timestamp", 0), reverse=True))
             break
 
     # Arbitrary GitHub repo
     else:
         if pipeline.count("/") == 1:
-
             # Looks like a GitHub address - try working with this repo
             log.debug(
                 f"Pipeline '{pipeline}' not in nf-core, but looks like a GitHub address - fetching releases from API"
             )
 
             # Get releases from GitHub API
             rel_r = gh_api.safe_get(f"https://api.github.com/repos/{pipeline}/releases")
```

### Comparing `nf-core-2.7.2/nf_core.egg-info/PKG-INFO` & `nf-core-2.8/nf_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nf-core
-Version: 2.7.2
+Version: 2.8
 Summary: Helper tools for use with nf-core Nextflow pipelines.
 Home-page: https://github.com/nf-core/tools
 Author: Phil Ewels
 Author-email: phil.ewels@scilifelab.se
 License: MIT
 Keywords: nf-core,nextflow,bioinformatics,workflow,pipeline,biology,sequencing,NGS,next generation sequencing
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![nf-core/tools](docs/images/nfcore-tools_logo_light.png#gh-light-mode-only) ![nf-core/tools](docs/images/nfcore-tools_logo_dark.png#gh-dark-mode-only) <!-- omit in toc -->
 
 [![Python tests](https://github.com/nf-core/tools/workflows/Python%20tests/badge.svg?branch=master&event=push)](https://github.com/nf-core/tools/actions?query=workflow%3A%22Python+tests%22+branch%3Amaster)
 [![codecov](https://codecov.io/gh/nf-core/tools/branch/master/graph/badge.svg)](https://codecov.io/gh/nf-core/tools)
@@ -51,15 +51,14 @@
   - [`modules remove` - Remove a module from a pipeline](#remove-a-module-from-a-pipeline)
   - [`modules patch` - Create a patch file for a module](#create-a-patch-file-for-a-module)
   - [`modules create` - Create a module from the template](#create-a-new-module)
   - [`modules create-test-yml` - Create the `test.yml` file for a module](#create-a-module-test-config-file)
   - [`modules lint` - Check a module against nf-core guidelines](#check-a-module-against-nf-core-guidelines)
   - [`modules test` - Run the tests for a module](#run-the-tests-for-a-module-using-pytest)
   - [`modules bump-versions` - Bump software versions of modules](#bump-bioconda-and-container-versions-of-modules-in)
-  - [`modules mulled` - Generate the name for a multi-tool container image](#generate-the-name-for-a-multi-tool-container-image)
 
 - [`nf-core subworkflows` - commands for dealing with subworkflows](#subworkflows)
   - [`subworkflows list` - List available subworkflows](#list-subworkflows)
     - [`subworkflows list remote` - List remote subworkflows](#list-remote-subworkflows)
     - [`subworkflows list local` - List installed subworkflows](#list-installed-subworkflows)
   - [`subworkflows info` - Show information about a subworkflow](#show-information-about-a-subworkflow)
   - [`subworkflows install` - Install subworkflows in a pipeline](#install-subworkflows-in-a-pipeline)
@@ -353,14 +352,16 @@
 
 You can run the pipeline by simply providing the directory path for the `workflow` folder to your `nextflow run` command:
 
 ```bash
 nextflow run /path/to/download/nf-core-rnaseq-dev/workflow/ --input mydata.csv --outdir results  # usual parameters here
 ```
 
+> Note that if you downloaded singularity images, you will need to use `-profile singularity` or have it enabled in your config file.
+
 ### Downloaded nf-core configs
 
 The pipeline files are automatically updated (`params.custom_config_base` is set to `../configs`), so that the local copy of institutional configs are available when running the pipeline.
 So using `-profile <NAME>` should work if available within [nf-core/configs](https://github.com/nf-core/configs).
 
 ### Downloading singularity containers
 
@@ -394,15 +395,15 @@
 The Singularity image download finds containers using two methods:
 
 1. It runs `nextflow config` on the downloaded workflow to look for a `process.container` statement for the whole pipeline.
    This is the typical method used for DSL1 pipelines.
 2. It scrapes any files it finds with a `.nf` file extension in the workflow `modules` directory for lines
    that look like `container = "xxx"`. This is the typical method for DSL2 pipelines, which have one container per process.
 
-Some DSL2 modules have container addresses for docker (eg. `quay.io/biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
+Some DSL2 modules have container addresses for docker (eg. `biocontainers/fastqc:0.11.9--0`) and also URLs for direct downloads of a Singularity continaer (eg. `https://depot.galaxyproject.org/singularity/fastqc:0.11.9--0`).
 Where both are found, the download URL is preferred.
 
 Once a full list of containers is found, they are processed in the following order:
 
 1. If the target image already exists, nothing is done (eg. with `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` specified)
 2. If found in `$NXF_SINGULARITY_CACHEDIR` and `--singularity-cache-only` is _not_ specified, they are copied to the output directory
 3. If they start with `http` they are downloaded directly within Python (default 4 at a time, you can customise this with `--parallel-downloads`)
@@ -617,34 +618,45 @@
 
 ### Add new parameters to the pipeline schema
 
 If you want to add a parameter to the schema, you first have to add the parameter and its default value to the `nextflow.config` file with the `params` scope. Afterwards, you run the command `nf-core schema build` to add the parameters to your schema and open the graphical interface to easily modify the schema.
 
 The graphical interface is oganzised in groups and within the groups the single parameters are stored. For a better overview you can collapse all groups with the `Collapse groups` button, then your new parameters will be the only remaining one at the bottom of the page. Now you can either create a new group with the `Add group` button or drag and drop the paramters in an existing group. Therefor the group has to be expanded. The group title will be displayed, if you run your pipeline with the `--help` flag and its description apears on the parameter page of your pipeline.
 
-Now you can start to change the parameter itself. The description is a short explanation about the parameter, that apears if you run your pipeline with the `--help` flag. By clicking on the dictionary icon you can add a longer explanation for the parameter page of your pipeline. If you want to specify some conditions for your parameter, like the file extension, you can use the nut icon to open the settings. This menu depends on the `type` you assigned to your parameter. For intergers you can define a min and max value, and for strings the file extension can be specified.
+Now you can start to change the parameter itself. The `ID` of a new parameter should be defined in small letters without whitespaces. The description is a short free text explanation about the parameter, that appears if you run your pipeline with the `--help` flag. By clicking on the dictionary icon you can add a longer explanation for the parameter page of your pipeline. Usually, they contain a small paragraph about the parameter settings or a used datasource, like databases or references. If you want to specify some conditions for your parameter, like the file extension, you can use the nut icon to open the settings. This menu depends on the `type` you assigned to your parameter. For integers you can define a min and max value, and for strings the file extension can be specified.
+
+The `type` field is one of the most important points in your pipeline schema, since it defines the datatype of your input and how it will be interpreted. This allows extensive testing prior to starting the pipeline.
+
+The basic datatypes for a pipeline schema are:
+
+- `string`
+- `number`
+- `integer`
+- `boolean`
+
+For the `string` type you have three different options in the settings (nut icon): `enumerated values`, `pattern` and `format`. The first option, `enumerated values`, allows you to specify a list of specific input values. The list has to be separated with a pipe. The `pattern` and `format` settings can depend on each other. The `format` has to be either a directory or a file path. Depending on the `format` setting selected, specifying the `pattern` setting can be the most efficient and time saving option, especially for `file paths`. The `number` and `integer` types share the same settings. Similarly to `string`, there is an `enumerated values` option with the possibility of specifying a `min` and `max` value. For the `boolean` there is no further settings and the default value is usually `false`. The `boolean` value can be switched to `true` by adding the flag to the command. This parameter type is often used to skip specific sections of a pipeline.
 
-After you filled your schema, click on the `Finished` button in the top rigth corner, this will automatically update your `nextflow_schema.json`. If this is not working you can copy the schema from the graphical interface and paste it in your `nextflow_schema.json` file.
+After filling the schema, click on the `Finished` button in the top right corner, this will automatically update your `nextflow_schema.json`. If this is not working, the schema can be copied from the graphical interface and pasted in your `nextflow_schema.json` file.
 
 ### Update existing pipeline schema
 
-Important for the update of a pipeline schema is, that if you want to change the default value of a parameter, you should change it in the `nextflow.config` file, since the value in the config file overwrites the value in the pipeline schema. To change any other parameter use `nf-core schema build --web-only` to open the graphical interface without rebuilding the pipeline schema. Now, you can change your parameters as mentioned above but keep in mind that changing the parameter datatype is depending on the default value you specified in the `nextflow.config` file.
+It's important to change the default value of a parameter in the `nextflow.config` file first and then in the pipeline schema, because the value in the config file overwrites the value in the pipeline schema. To change any other parameter use `nf-core schema build --web-only` to open the graphical interface without rebuilding the pipeline schema. Now, the parameters can be changed as mentioned above but keep in mind that changing the parameter datatype depends on the default value specified in the `nextflow.config` file.
 
 ### Linting a pipeline schema
 
 The pipeline schema is linted as part of the main pipeline `nf-core lint` command,
 however sometimes it can be useful to quickly check the syntax of the JSONSchema without running a full lint run.
 
-Usage is `nf-core schema lint <schema>`, eg:
+Usage is `nf-core schema lint <schema>` (defaulting to `nextflow_schema.json`), eg:
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
 -->
 
-![`nf-core schema lint nextflow_schema.json`](docs/images/nf-core-schema-lint.svg)
+![`nf-core schema lint`](docs/images/nf-core-schema-lint.svg)
 
 ## Bumping a pipeline version number
 
 When releasing a new version of a nf-core pipeline, version numbers have to be updated in several different places. The helper command `nf-core bump-version` automates this for you to avoid manual errors (and frustration!).
 
 The command uses results from the linting process, so will only work with workflows that pass these tests.
 
@@ -968,25 +980,14 @@
 If you want this module to be updated only to a specific version (or downgraded), you could instead specifiy the version:
 
 ```yaml
 bump-versions:
   star/align: "2.6.1d"
 ```
 
-### Generate the name for a multi-tool container image
-
-When you want to use an image of a multi-tool container and you know the specific dependencies and their versions of that container, for example, by looking them up in the [BioContainers hash.tsv](https://github.com/BioContainers/multi-package-containers/blob/master/combinations/hash.tsv), you can use the `nf-core modules mulled` helper tool. This tool generates the name of a BioContainers mulled image.
-
-<!-- RICH-CODEX
-working_dir: tmp/modules
-after_command: cd ../../ && rm -rf tmp
--->
-
-![`nf-core modules mulled pysam==0.16.0.1 biopython==1.78`](docs/images/nf-core-modules-mulled.svg)
-
 ## Subworkflows
 
 After the launch of nf-core modules, we can provide now also nf-core subworkflows to fully utilize the power of DSL2 modularization.
 Subworkflows are chains of multiple module definitions that can be imported into any pipeline.
 This allows multiple pipelines to use the same code for a the same tasks, and gives a greater degree of reusability and unit testing.
 
 To allow us to test modules and subworkflows together we put the nf-core DSL2 subworkflows into the `subworkflows` directory of the modules repository is at <https://github.com/nf-core/modules>.
@@ -1039,38 +1040,44 @@
 
 #### List installed subworkflows
 
 To list subworkflows installed in a local pipeline directory you can use `nf-core subworkflows list local`. This will list the subworkflows install in the current working directory by default. If you want to specify another directory, use the `--dir <pipeline_dir>` flag.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 head: 25
 -->
 
 ![`nf-core subworkflows list local`](docs/images/nf-core-subworkflows-list-local.svg)
 
 ## Show information about a subworkflow
 
 For quick help about how a subworkflow works, use `nf-core subworkflows info <subworkflow_name>`.
 This shows documentation about the subworkflow on the command line, similar to what's available on the
 [nf-core website](https://nf-co.re/subworkflows).
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows info bam_rseqc`](docs/images/nf-core-subworkflows-info.svg)
 
 ### Install subworkflows in a pipeline
 
 You can install subworkflows from [nf-core/modules](https://github.com/nf-core/modules) in your pipeline using `nf-core subworkflows install`.
 A subworkflow installed this way will be installed to the `./subworkflows/nf-core` directory.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows install bam_rseqc`](docs/images/nf-core-subworkflows-install.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows install` like above or select it from a list of available subworkflows by only running `nf-core subworkflows install`.
 
 There are four additional flags that you can use when installing a subworkflow:
@@ -1082,14 +1089,16 @@
 
 ### Update subworkflows in a pipeline
 
 You can update subworkflows installed from a remote repository in your pipeline using `nf-core subworkflows update`.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows update --all --no-preview`](docs/images/nf-core-subworkflows-update.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows update` like above or select it from the list of available subworkflows by only running `nf-core subworkflows update`.
 
 There are six additional flags that you can use with this command:
@@ -1141,14 +1150,16 @@
 
 ### Remove a subworkflow from a pipeline
 
 To delete a subworkflow from your pipeline, run `nf-core subworkflows remove`.
 
 <!-- RICH-CODEX
 working_dir: tmp/nf-core-nextbigthing
+before_command: >
+  echo "repository_type: pipeline" >> .nf-core.yml
 -->
 
 ![`nf-core subworkflows remove bam_rseqc`](docs/images/nf-core-subworkflows-remove.svg)
 
 You can pass the subworkflow name as an optional argument to `nf-core subworkflows remove` like above or select it from the list of available subworkflows by only running `nf-core subworkflows remove`. To specify the pipeline directory, use `--dir <pipeline_dir>`.
 
 ### Create a new subworkflow
@@ -1169,41 +1180,41 @@
 It will start in the current working directory, or whatever is specified with `--dir <directory>`.
 
 The `nf-core subworkflows create` command will prompt you with the relevant questions in order to create all of the necessary subworkflow files.
 
 <!-- RICH-CODEX
 working_dir: tmp
 before_command: git clone https://github.com/nf-core/modules.git && cd modules
-fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot  --label process_low --meta --force
+fake_command: nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force
 -->
 
-![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot  --label process_low --meta --force`](docs/images/nf-core-subworkflows-create.svg)
+![`cd modules && nf-core subworkflows create bam_stats_samtools --author @nf-core-bot --force`](docs/images/nf-core-subworkflows-create.svg)
 
 ### Create a subworkflow test config file
 
 All subworkflows on [nf-core/modules](https://github.com/nf-core/modules) have a strict requirement of being unit tested using minimal test data.
 To help developers build new subworkflows, the `nf-core subworkflows create-test-yml` command automates the creation of the yaml file required to document the output file `md5sum` and other information generated by the testing.
 After you have written a minimal Nextflow script to test your subworkflow in `/tests/subworkflow/<subworkflow_name>/main.nf`, this command will run the tests for you and create the `/tests/subworkflow/<tool>/<subtool>/test.yml` file.
 
 <!-- RICH-CODEX
-working_dir: tmp/subworkflows
+working_dir: tmp/modules
 extra_env:
   PROFILE: 'conda'
 -->
 
 ![`nf-core subworkflows create-test-yml bam_stats_samtools --no-prompts --force`](docs/images/nf-core-subworkflows-create-test.svg)
 
 ### Run the tests for a subworkflow using pytest
 
 To run unit tests of a subworkflow that you have installed or the test created by the command [`nf-core subworkflow create-test-yml`](#create-a-subworkflow-test-config-file), you can use `nf-core subworkflows test` command. This command runs the tests specified in `tests/subworkflows/<subworkflow_name>/test.yml` file using [pytest](https://pytest-workflow.readthedocs.io/en/stable/).
 
 You can specify the subworkflow name in the form TOOL/SUBTOOL in command line or provide it later by prompts.
 
 <!-- RICH-CODEX
-working_dir: tmp/subworkflows
+working_dir: tmp/modules
 timeout: 30
 extra_env:
   PROFILE: 'conda'
 -->
 
 ![`nf-core subworkflows test bam_rseqc --no-prompts`](docs/images/nf-core-subworkflows-test.svg)
```

### Comparing `nf-core-2.7.2/nf_core.egg-info/SOURCES.txt` & `nf-core-2.8/nf_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 nf_core.egg-info/dependency_links.txt
 nf_core.egg-info/entry_points.txt
 nf_core.egg-info/not-zip-safe
 nf_core.egg-info/requires.txt
 nf_core.egg-info/top_level.txt
 nf_core/components/__init__.py
 nf_core/components/components_command.py
-nf_core/components/components_create.py
 nf_core/components/components_test.py
 nf_core/components/components_utils.py
+nf_core/components/create.py
 nf_core/components/info.py
 nf_core/components/install.py
 nf_core/components/list.py
 nf_core/components/remove.py
 nf_core/components/update.py
 nf_core/lint/__init__.py
 nf_core/lint/actions_awsfulltest.py
@@ -49,14 +49,15 @@
 nf_core/lint/nextflow_config.py
 nf_core/lint/pipeline_name_conventions.py
 nf_core/lint/pipeline_todos.py
 nf_core/lint/readme.py
 nf_core/lint/schema_description.py
 nf_core/lint/schema_lint.py
 nf_core/lint/schema_params.py
+nf_core/lint/system_exit.py
 nf_core/lint/template_strings.py
 nf_core/lint/version_consistency.py
 nf_core/module-template/modules/main.nf
 nf_core/module-template/modules/meta.yml
 nf_core/module-template/tests/main.nf
 nf_core/module-template/tests/nextflow.config
 nf_core/module-template/tests/test.yml
@@ -67,15 +68,14 @@
 nf_core/modules/install.py
 nf_core/modules/list.py
 nf_core/modules/modules_differ.py
 nf_core/modules/modules_json.py
 nf_core/modules/modules_repo.py
 nf_core/modules/modules_test.py
 nf_core/modules/modules_utils.py
-nf_core/modules/mulled.py
 nf_core/modules/nfcore_module.py
 nf_core/modules/patch.py
 nf_core/modules/remove.py
 nf_core/modules/test_yml_builder.py
 nf_core/modules/update.py
 nf_core/modules/lint/__init__.py
 nf_core/modules/lint/main_nf.py
@@ -87,37 +87,40 @@
 nf_core/modules/lint/module_todos.py
 nf_core/modules/lint/module_version.py
 nf_core/pipeline-template/.editorconfig
 nf_core/pipeline-template/.gitattributes
 nf_core/pipeline-template/.gitignore
 nf_core/pipeline-template/.gitpod.yml
 nf_core/pipeline-template/.nf-core.yml
+nf_core/pipeline-template/.pre-commit-config.yaml
 nf_core/pipeline-template/.prettierignore
 nf_core/pipeline-template/.prettierrc.yml
 nf_core/pipeline-template/CHANGELOG.md
 nf_core/pipeline-template/CITATIONS.md
 nf_core/pipeline-template/CODE_OF_CONDUCT.md
 nf_core/pipeline-template/LICENSE
 nf_core/pipeline-template/README.md
 nf_core/pipeline-template/main.nf
 nf_core/pipeline-template/modules.json
 nf_core/pipeline-template/nextflow.config
 nf_core/pipeline-template/nextflow_schema.json
 nf_core/pipeline-template/pyproject.toml
+nf_core/pipeline-template/tower.yml
 nf_core/pipeline-template/.devcontainer/devcontainer.json
 nf_core/pipeline-template/.github/.dockstore.yml
 nf_core/pipeline-template/.github/CONTRIBUTING.md
 nf_core/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
 nf_core/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.yml
 nf_core/pipeline-template/.github/ISSUE_TEMPLATE/config.yml
 nf_core/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.yml
 nf_core/pipeline-template/.github/workflows/awsfulltest.yml
 nf_core/pipeline-template/.github/workflows/awstest.yml
 nf_core/pipeline-template/.github/workflows/branch.yml
 nf_core/pipeline-template/.github/workflows/ci.yml
+nf_core/pipeline-template/.github/workflows/clean-up.yml
 nf_core/pipeline-template/.github/workflows/fix-linting.yml
 nf_core/pipeline-template/.github/workflows/linting.yml
 nf_core/pipeline-template/.github/workflows/linting_comment.yml
 nf_core/pipeline-template/assets/adaptivecard.json
 nf_core/pipeline-template/assets/email_template.html
 nf_core/pipeline-template/assets/email_template.txt
 nf_core/pipeline-template/assets/methods_description_template.yml
@@ -175,15 +178,14 @@
 tests/test_download.py
 tests/test_launch.py
 tests/test_licenses.py
 tests/test_lint.py
 tests/test_lint_utils.py
 tests/test_list.py
 tests/test_modules.py
-tests/test_mulled.py
 tests/test_refgenie.py
 tests/test_schema.py
 tests/test_subworkflows.py
 tests/test_sync.py
 tests/test_test_utils.py
 tests/test_utils.py
 tests/utils.py
@@ -209,13 +211,14 @@
 tests/modules/modules_json.py
 tests/modules/modules_test.py
 tests/modules/patch.py
 tests/modules/remove.py
 tests/modules/update.py
 tests/subworkflows/__init__.py
 tests/subworkflows/create.py
+tests/subworkflows/create_test_yml.py
 tests/subworkflows/info.py
 tests/subworkflows/install.py
 tests/subworkflows/list.py
 tests/subworkflows/remove.py
 tests/subworkflows/subworkflows_test.py
 tests/subworkflows/update.py
```

### Comparing `nf-core-2.7.2/setup.py` & `nf-core-2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
-version = "2.7.2"
+version = "2.8"
 
 with open("README.md") as f:
     readme = f.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
@@ -31,13 +31,13 @@
     author_email="phil.ewels@scilifelab.se",
     url="https://github.com/nf-core/tools",
     license="MIT",
     entry_points={
         "console_scripts": ["nf-core=nf_core.__main__:run_nf_core"],
         "refgenie.hooks.post_update": ["nf-core-refgenie=nf_core.refgenie:update_config"],
     },
-    python_requires=">=3.7, <4",
+    python_requires=">=3.8, <4",
     install_requires=required,
     packages=find_packages(exclude=("docs")),
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `nf-core-2.7.2/tests/lint/actions_awsfulltest.py` & `nf-core-2.8/tests/lint/actions_awsfulltest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/actions_awstest.py` & `nf-core-2.8/tests/lint/actions_awstest.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/actions_ci.py` & `nf-core-2.8/tests/lint/actions_ci.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/actions_schema_validation.py` & `nf-core-2.8/tests/lint/actions_schema_validation.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/files_exist.py` & `nf-core-2.8/tests/lint/files_exist.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/files_unchanged.py` & `nf-core-2.8/tests/lint/files_unchanged.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/merge_markers.py` & `nf-core-2.8/tests/lint/merge_markers.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/nextflow_config.py` & `nf-core-2.8/tests/lint/nextflow_config.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/lint/version_consistency.py` & `nf-core-2.8/tests/lint/version_consistency.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/modules/bump_versions.py` & `nf-core-2.8/tests/modules/bump_versions.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/modules/create.py` & `nf-core-2.8/tests/modules/create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 import os
 
 import pytest
-import requests_mock
+import requests_cache
+import responses
 
 import nf_core.modules
-from tests.utils import mock_api_calls
+from tests.utils import mock_anaconda_api_calls, mock_biocontainers_api_calls
 
 
 def test_modules_create_succeed(self):
     """Succeed at creating the TrimGalore! module"""
-    with requests_mock.Mocker() as mock:
-        mock_api_calls(mock, "trim-galore", "0.6.7")
+    with responses.RequestsMock() as rsps:
+        mock_anaconda_api_calls(rsps, "trim-galore", "0.6.7")
+        mock_biocontainers_api_calls(rsps, "trim-galore", "0.6.7")
         module_create = nf_core.modules.ModuleCreate(
             self.pipeline_dir, "trimgalore", "@author", "process_single", True, True, conda_name="trim-galore"
         )
-        module_create.create()
+        with requests_cache.disabled():
+            module_create.create()
     assert os.path.exists(os.path.join(self.pipeline_dir, "modules", "local", "trimgalore.nf"))
 
 
 def test_modules_create_fail_exists(self):
     """Fail at creating the same module twice"""
-    with requests_mock.Mocker() as mock:
-        mock_api_calls(mock, "trim-galore", "0.6.7")
+    with responses.RequestsMock() as rsps:
+        mock_anaconda_api_calls(rsps, "trim-galore", "0.6.7")
+        mock_biocontainers_api_calls(rsps, "trim-galore", "0.6.7")
         module_create = nf_core.modules.ModuleCreate(
             self.pipeline_dir, "trimgalore", "@author", "process_single", False, False, conda_name="trim-galore"
         )
-        module_create.create()
-        with pytest.raises(UserWarning) as excinfo:
+        with requests_cache.disabled():
             module_create.create()
+        with pytest.raises(UserWarning) as excinfo:
+            with requests_cache.disabled():
+                module_create.create()
     assert "Module file exists already" in str(excinfo.value)
 
 
 def test_modules_create_nfcore_modules(self):
     """Create a module in nf-core/modules clone"""
-    with requests_mock.Mocker() as mock:
-        mock_api_calls(mock, "fastqc", "0.11.9")
+    with responses.RequestsMock() as rsps:
+        mock_anaconda_api_calls(rsps, "fastqc", "0.11.9")
+        mock_biocontainers_api_calls(rsps, "fastqc", "0.11.9")
         module_create = nf_core.modules.ModuleCreate(
             self.nfcore_modules, "fastqc", "@author", "process_low", False, False
         )
-        module_create.create()
+        with requests_cache.disabled():
+            module_create.create()
     assert os.path.exists(os.path.join(self.nfcore_modules, "modules", "nf-core", "fastqc", "main.nf"))
     assert os.path.exists(os.path.join(self.nfcore_modules, "tests", "modules", "nf-core", "fastqc", "main.nf"))
 
 
 def test_modules_create_nfcore_modules_subtool(self):
     """Create a tool/subtool module in a nf-core/modules clone"""
-    with requests_mock.Mocker() as mock:
-        mock_api_calls(mock, "star", "2.8.10a")
+    with responses.RequestsMock() as rsps:
+        mock_anaconda_api_calls(rsps, "star", "2.8.10a")
+        mock_biocontainers_api_calls(rsps, "star", "2.8.10a")
         module_create = nf_core.modules.ModuleCreate(
             self.nfcore_modules, "star/index", "@author", "process_medium", False, False
         )
-        module_create.create()
+        with requests_cache.disabled():
+            module_create.create()
     assert os.path.exists(os.path.join(self.nfcore_modules, "modules", "nf-core", "star", "index", "main.nf"))
     assert os.path.exists(os.path.join(self.nfcore_modules, "tests", "modules", "nf-core", "star", "index", "main.nf"))
```

### Comparing `nf-core-2.7.2/tests/modules/create_test_yml.py` & `nf-core-2.8/tests/modules/create_test_yml.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,56 +7,54 @@
 
 from ..utils import GITLAB_DEFAULT_BRANCH, GITLAB_URL, with_temporary_folder
 
 
 @with_temporary_folder
 def test_modules_custom_yml_dumper(self, out_dir):
     """Try to create a yml file with the custom yml dumper"""
-    yml_output_path = os.path.join(out_dir, "test.yml")
+    yml_output_path = Path(out_dir, "test.yml")
     meta_builder = nf_core.modules.ModulesTestYmlBuilder("test/tool", self.pipeline_dir, False, "./", False, True)
     meta_builder.test_yml_output_path = yml_output_path
     meta_builder.tests = [{"testname": "myname"}]
     meta_builder.print_test_yml()
-    assert os.path.isfile(yml_output_path)
+    assert Path(yml_output_path).is_file()
 
 
 @with_temporary_folder
 def test_modules_test_file_dict(self, test_file_dir):
     """Create dict of test files and create md5 sums"""
     meta_builder = nf_core.modules.ModulesTestYmlBuilder("test/tool", self.pipeline_dir, False, "./", False, True)
-    with open(os.path.join(test_file_dir, "test_file.txt"), "w") as fh:
+    with open(Path(test_file_dir, "test_file.txt"), "w") as fh:
         fh.write("this line is just for testing")
     test_files = meta_builder.create_test_file_dict(test_file_dir)
     assert len(test_files) == 1
     assert test_files[0]["md5sum"] == "2191e06b28b5ba82378bcc0672d01786"
 
 
 @with_temporary_folder
 def test_modules_create_test_yml_get_md5(self, test_file_dir):
     """Get md5 sums from a dummy output"""
     meta_builder = nf_core.modules.ModulesTestYmlBuilder("test/tool", self.pipeline_dir, False, "./", False, True)
-    with open(os.path.join(test_file_dir, "test_file.txt"), "w") as fh:
+    with open(Path(test_file_dir, "test_file.txt"), "w") as fh:
         fh.write("this line is just for testing")
     test_files = meta_builder.get_md5_sums(command="dummy", results_dir=test_file_dir, results_dir_repeat=test_file_dir)
     assert test_files[0]["md5sum"] == "2191e06b28b5ba82378bcc0672d01786"
 
 
 def test_modules_create_test_yml_entry_points(self):
     """Test extracting test entry points from a main.nf file"""
     meta_builder = nf_core.modules.ModulesTestYmlBuilder("bpipe/test", self.pipeline_dir, False, "./", False, True)
-    meta_builder.module_test_main = os.path.join(
-        self.nfcore_modules, "tests", "modules", "nf-core", "bpipe", "test", "main.nf"
-    )
+    meta_builder.module_test_main = Path(self.nfcore_modules, "tests", "modules", "nf-core", "bpipe", "test", "main.nf")
     meta_builder.scrape_workflow_entry_points()
     assert meta_builder.entry_points[0] == "test_bpipe_test"
 
 
 def test_modules_create_test_yml_check_inputs(self):
     """Test the check_inputs() function - raise UserWarning because test.yml exists"""
     cwd = os.getcwd()
     os.chdir(self.nfcore_modules)
     meta_builder = nf_core.modules.ModulesTestYmlBuilder("bpipe/test", ".", False, "./", False, True)
-    meta_builder.module_test_main = os.path.join(self.nfcore_modules, "tests", "modules", "bpipe", "test", "main.nf")
+    meta_builder.module_test_main = Path(self.nfcore_modules, "tests", "modules", "bpipe", "test", "main.nf")
     with pytest.raises(UserWarning) as excinfo:
         meta_builder.check_inputs()
     os.chdir(cwd)
     assert "Test YAML file already exists!" in str(excinfo.value)
```

### Comparing `nf-core-2.7.2/tests/modules/info.py` & `nf-core-2.8/tests/modules/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,23 +34,23 @@
     assert "--git-remote" in output
 
 
 def test_modules_info_local(self):
     """Test getting info about a locally installed module"""
     self.mods_install.install("trimgalore")
     mods_info = nf_core.modules.ModuleInfo(self.pipeline_dir, "trimgalore")
-    mods_info.local = True
     mods_info_output = mods_info.get_component_info()
     console = Console(record=True)
     console.print(mods_info_output)
     output = console.export_text()
 
     assert "Module: trimgalore" in output
     assert "Inputs" in output
     assert "Outputs" in output
+    assert "Location" in output
 
 
 def test_modules_info_in_modules_repo(self):
     """Test getting info about a module in the modules repo"""
     mods_info = nf_core.modules.ModuleInfo(self.nfcore_modules, "fastqc")
     mods_info.local = True
     mods_info_output = mods_info.get_component_info()
```

### Comparing `nf-core-2.7.2/tests/modules/list.py` & `nf-core-2.8/tests/modules/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/modules/modules_json.py` & `nf-core-2.8/tests/modules/modules_json.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/modules/modules_test.py` & `nf-core-2.8/tests/modules/modules_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/modules/patch.py` & `nf-core-2.8/tests/modules/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import tempfile
 from pathlib import Path
+from unittest import mock
 
 import pytest
 
 import nf_core.components.components_command
 import nf_core.modules
 
 from ..utils import GITLAB_URL
@@ -12,20 +13,20 @@
 """
 Test the 'nf-core modules patch' command
 
 Uses a branch (patch-tester) in the GitLab nf-core/modules-test repo when
 testing if the update commands works correctly with patch files
 """
 
-ORG_SHA = "775fcd090fb776a0be695044f8ab1af8896c8452"
-CORRECT_SHA = "335cd32405568ca3b6d4c05ab1e8a98c21e18a4d"
-SUCCEED_SHA = "f1566140c752e9c68fffc189fbe8cb9ee942b3ca"
-FAIL_SHA = "1fc8b0f953d915d66ee40d28bc337ff0998d05bd"
+ORG_SHA = "002623ccc88a3b0cb302c7d8f13792a95354d9f2"
+CORRECT_SHA = "0245a9277d51a47c8aa68d264d294cf45312fab8"
+SUCCEED_SHA = "ba15c20c032c549d77c5773659f19c2927daf48e"
+FAIL_SHA = "67b642d4471c4005220a342cad3818d5ba2b5a73"
 BISMARK_ALIGN = "bismark/align"
-REPO_NAME = "nf-core"
+REPO_NAME = "nf-core-test"
 PATCH_BRANCH = "patch-tester"
 REPO_URL = "https://gitlab.com/nf-core/modules-test.git"
 
 
 def setup_patch(pipeline_dir, modify_module):
     install_obj = nf_core.modules.ModuleInstall(
         pipeline_dir, prompt=False, force=False, remote_url=GITLAB_URL, branch=PATCH_BRANCH, sha=ORG_SHA
@@ -108,14 +109,15 @@
     assert "+    tuple val(meta), path(reads), path(index)\n" in patch_lines
 
 
 def test_create_patch_try_apply_successful(self):
     """
     Test creating a patch file and applying it to a new version of the the files
     """
+
     setup_patch(self.pipeline_dir, True)
     module_relpath = Path("modules", REPO_NAME, BISMARK_ALIGN)
     module_path = Path(self.pipeline_dir, module_relpath)
 
     # Try creating a patch file
     patch_obj = nf_core.modules.ModulePatch(self.pipeline_dir, GITLAB_URL, PATCH_BRANCH)
     patch_obj.patch(BISMARK_ALIGN)
@@ -174,14 +176,15 @@
     assert "    tuple val(meta), path(reads), path(index)\n" in main_nf_lines
 
 
 def test_create_patch_try_apply_failed(self):
     """
     Test creating a patch file and applying it to a new version of the the files
     """
+
     setup_patch(self.pipeline_dir, True)
     module_relpath = Path("modules", REPO_NAME, BISMARK_ALIGN)
     module_path = Path(self.pipeline_dir, module_relpath)
 
     # Try creating a patch file
     patch_obj = nf_core.modules.ModulePatch(self.pipeline_dir, GITLAB_URL, PATCH_BRANCH)
     patch_obj.patch(BISMARK_ALIGN)
@@ -212,14 +215,15 @@
 def test_create_patch_update_success(self):
     """
     Test creating a patch file and the updating the module
 
     Should have the same effect as 'test_create_patch_try_apply_successful'
     but uses higher level api
     """
+
     setup_patch(self.pipeline_dir, True)
     module_path = Path(self.pipeline_dir, "modules", REPO_NAME, BISMARK_ALIGN)
 
     # Try creating a patch file
     patch_obj = nf_core.modules.ModulePatch(self.pipeline_dir, GITLAB_URL, PATCH_BRANCH)
     patch_obj.patch(BISMARK_ALIGN)
 
@@ -273,14 +277,15 @@
     assert "    tuple val(meta), path(reads), path(index)\n" in main_nf_lines
 
 
 def test_create_patch_update_fail(self):
     """
     Test creating a patch file and updating a module when there is a diff conflict
     """
+
     setup_patch(self.pipeline_dir, True)
     module_path = Path(self.pipeline_dir, "modules", REPO_NAME, BISMARK_ALIGN)
 
     # Try creating a patch file
     patch_obj = nf_core.modules.ModulePatch(self.pipeline_dir, GITLAB_URL, PATCH_BRANCH)
     patch_obj.patch(BISMARK_ALIGN)
 
@@ -318,7 +323,38 @@
             shouldbe = fh.read()
         assert installed == shouldbe
 
     # Check that the patch file is unaffected
     with open(module_path / patch_fn, "r") as fh:
         new_patch_contents = fh.read()
     assert patch_contents == new_patch_contents
+
+
+def test_remove_patch(self):
+    """Test creating a patch when there is no change to the module"""
+    setup_patch(self.pipeline_dir, True)
+
+    # Try creating a patch file
+    patch_obj = nf_core.modules.ModulePatch(self.pipeline_dir, GITLAB_URL, PATCH_BRANCH)
+    patch_obj.patch(BISMARK_ALIGN)
+
+    module_path = Path(self.pipeline_dir, "modules", REPO_NAME, BISMARK_ALIGN)
+
+    # Check that a patch file with the correct name has been created
+    patch_fn = f"{'-'.join(BISMARK_ALIGN.split('/'))}.diff"
+    assert set(os.listdir(module_path)) == {"main.nf", "meta.yml", patch_fn}
+
+    # Check the 'modules.json' contains a patch file for the module
+    modules_json_obj = nf_core.modules.modules_json.ModulesJson(self.pipeline_dir)
+    assert modules_json_obj.get_patch_fn(BISMARK_ALIGN, REPO_URL, REPO_NAME) == Path(
+        "modules", REPO_NAME, BISMARK_ALIGN, patch_fn
+    )
+
+    with mock.patch.object(nf_core.create.questionary, "confirm") as mock_questionary:
+        mock_questionary.unsafe_ask.return_value = True
+        patch_obj.remove(BISMARK_ALIGN)
+    # Check that the diff file has been removed
+    assert set(os.listdir(module_path)) == {"main.nf", "meta.yml"}
+
+    # Check that the 'modules.json' entry has been removed
+    modules_json_obj = nf_core.modules.modules_json.ModulesJson(self.pipeline_dir)
+    assert modules_json_obj.get_patch_fn(BISMARK_ALIGN, REPO_URL, REPO_NAME) is None
```

### Comparing `nf-core-2.7.2/tests/modules/remove.py` & `nf-core-2.8/tests/modules/remove.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     """Test removing TrimGalore! module without installing it"""
     assert self.mods_remove.remove("trimgalore") is False
 
 
 def test_modules_remove_multiqc_from_gitlab(self):
     """Test removing multiqc module after installing it from an alternative source"""
     self.mods_install_gitlab.install("multiqc")
-    module_path = os.path.join(self.mods_install_gitlab.dir, "modules", "nf-core", "multiqc")
+    module_path = os.path.join(self.mods_install_gitlab.dir, "modules", "nf-core-test", "multiqc")
     assert self.mods_remove_gitlab.remove("multiqc", force=True)
     assert os.path.exists(module_path) is False
```

### Comparing `nf-core-2.7.2/tests/modules/update.py` & `nf-core-2.8/tests/modules/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     mod_json = ModulesJson(self.pipeline_dir).get_modules_json()
     assert "git_sha" in mod_json["repos"][GITLAB_URL]["modules"][GITLAB_REPO]["trimgalore"]
     assert mod_json["repos"][GITLAB_URL]["modules"][GITLAB_REPO]["trimgalore"]["git_sha"] == OLD_TRIMGALORE_SHA
 
 
 def test_update_with_config_no_updates(self):
     """Don't update any nf-core modules"""
-    self.mods_install_old.install("trimgalore")
+    assert self.mods_install_old.install("trimgalore")
     old_mod_json = ModulesJson(self.pipeline_dir).get_modules_json()
 
     # Fix the version of all nf-core modules in the .nf-core.yml to an old version
     update_config = {GITLAB_URL: False}
     config_fn, tools_config = nf_core.utils.load_tools_config(self.pipeline_dir)
     tools_config["update"] = update_config
     with open(os.path.join(self.pipeline_dir, config_fn), "w") as f:
```

### Comparing `nf-core-2.7.2/tests/subworkflows/create.py` & `nf-core-2.8/tests/subworkflows/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,14 @@
         subworkflow_create.create()
     assert "Subworkflow file exists already" in str(excinfo.value)
 
 
 def test_subworkflows_create_nfcore_modules(self):
     """Create a subworkflow in nf-core/modules clone"""
     subworkflow_create = nf_core.subworkflows.SubworkflowCreate(
-        self.nfcore_modules, "test_subworkflow", "@author", True
+        self.nfcore_modules, "test_subworkflow", "@author", force=True
     )
     subworkflow_create.create()
     assert os.path.exists(os.path.join(self.nfcore_modules, "subworkflows", "nf-core", "test_subworkflow", "main.nf"))
     assert os.path.exists(
         os.path.join(self.nfcore_modules, "tests", "subworkflows", "nf-core", "test_subworkflow", "main.nf")
     )
```

### Comparing `nf-core-2.7.2/tests/subworkflows/info.py` & `nf-core-2.8/tests/subworkflows/info.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/subworkflows/install.py` & `nf-core-2.8/tests/subworkflows/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nf_core.modules.modules_json import ModulesJson
 from nf_core.subworkflows.install import SubworkflowInstall
 
 from ..utils import (
     GITLAB_BRANCH_TEST_BRANCH,
     GITLAB_REPO,
     GITLAB_SUBWORKFLOWS_BRANCH,
+    GITLAB_SUBWORKFLOWS_ORG_PATH_BRANCH,
     GITLAB_URL,
     with_temporary_folder,
 )
 
 
 def test_subworkflow_install_nopipeline(self):
     """Test installing a subworkflow - no pipeline given"""
@@ -136,7 +137,18 @@
         "bam_sort_stats_samtools"
     ]["installed_by"] == ["subworkflows"]
     assert sorted(
         mod_json["repos"]["https://github.com/nf-core/modules.git"]["subworkflows"]["nf-core"]["bam_stats_samtools"][
             "installed_by"
         ]
     ) == sorted(["subworkflows", "bam_sort_stats_samtools"])
+
+
+def test_subworkflows_install_alternate_remote(self):
+    """Test installing a module from a different remote with the same organization path"""
+    install_obj = SubworkflowInstall(
+        self.pipeline_dir, remote_url=GITLAB_URL, branch=GITLAB_SUBWORKFLOWS_ORG_PATH_BRANCH
+    )
+    # Install a subworkflow from GitLab which is also installed from GitHub with the same org_path
+    with pytest.raises(Exception) as excinfo:
+        install_obj.install("fastqc")
+        assert "Could not find a 'main.nf' or 'nextflow.config' file" in str(excinfo.value)
```

### Comparing `nf-core-2.7.2/tests/subworkflows/list.py` & `nf-core-2.8/tests/subworkflows/list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/subworkflows/remove.py` & `nf-core-2.8/tests/subworkflows/remove.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/subworkflows/subworkflows_test.py` & `nf-core-2.8/tests/subworkflows/subworkflows_test.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/subworkflows/update.py` & `nf-core-2.8/tests/subworkflows/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import yaml
 
 import nf_core.utils
 from nf_core.modules.modules_json import ModulesJson
 from nf_core.modules.modules_repo import NF_CORE_MODULES_NAME, NF_CORE_MODULES_REMOTE
+from nf_core.modules.remove import ModuleRemove
 from nf_core.modules.update import ModuleUpdate
 from nf_core.subworkflows.update import SubworkflowUpdate
 
 from ..utils import OLD_SUBWORKFLOWS_SHA
 
 
 def test_install_and_update(self):
@@ -317,13 +318,17 @@
 
     # Check that tabix/bgziptabix is not there
     assert "tabix/bgziptabix" not in mod_json["repos"][NF_CORE_MODULES_REMOTE]["modules"][NF_CORE_MODULES_NAME]
     assert not Path(self.pipeline_dir, "modules", NF_CORE_MODULES_NAME, "tabix/bgziptabix").is_dir()
     # Check that tabix/tabix is there
     assert "tabix/tabix" in mod_json["repos"][NF_CORE_MODULES_REMOTE]["modules"][NF_CORE_MODULES_NAME]
     assert Path(self.pipeline_dir, "modules", NF_CORE_MODULES_NAME, "tabix/tabix").is_dir()
+    # Check that ensemblevep is not there but instead we have ensemblevep/vep (due to a file re-naming)
+    assert "ensemblvep" not in mod_json["repos"][NF_CORE_MODULES_REMOTE]["modules"][NF_CORE_MODULES_NAME]
+    assert "ensemblvep/vep" in mod_json["repos"][NF_CORE_MODULES_REMOTE]["modules"][NF_CORE_MODULES_NAME]
+    assert Path(self.pipeline_dir, "modules", NF_CORE_MODULES_NAME, "ensemblvep/vep").is_dir()
 
 
 def cmp_component(dir1, dir2):
     """Compare two versions of the same component"""
     files = ["main.nf", "meta.yml"]
     return all(filecmp.cmp(Path(dir1, f), Path(dir2, f), shallow=False) for f in files)
```

### Comparing `nf-core-2.7.2/tests/test_bump_version.py` & `nf-core-2.8/tests/test_bump_version.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_cli.py` & `nf-core-2.8/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,7 +346,24 @@
         cmd = ["lint"]
         with self.assertLogs() as captured_logs:
             result = self.invoke_cli(cmd)
 
         assert result.exit_code == 1
         assert error_txt in captured_logs.output[-1]
         assert captured_logs.records[-1].levelname == "ERROR"
+
+    @mock.patch("nf_core.schema.PipelineSchema.get_schema_path")
+    def test_schema_lint(self, mock_get_schema_path):
+        """Test nf-core schema lint defaults to nextflow_schema.json"""
+        cmd = ["schema", "lint"]
+        result = self.invoke_cli(cmd)
+        assert mock_get_schema_path.called_with("nextflow_schema.json")
+        assert "nextflow_schema.json" in result.output
+
+    @mock.patch("nf_core.schema.PipelineSchema.get_schema_path")
+    def test_schema_lint_filename(self, mock_get_schema_path):
+        """Test nf-core schema lint accepts a filename"""
+        cmd = ["schema", "lint", "some_other_filename"]
+        result = self.invoke_cli(cmd)
+        assert mock_get_schema_path.called_with("some_other_filename")
+        assert "some_other_filename" in result.output
+        assert "nextflow_schema.json" not in result.output
```

### Comparing `nf-core-2.7.2/tests/test_download.py` & `nf-core-2.8/tests/test_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import nf_core.utils
 from nf_core.download import DownloadWorkflow
 
 from .utils import with_temporary_file, with_temporary_folder
 
 
 class DownloadTest(unittest.TestCase):
-
     #
     # Tests for 'get_release_hash'
     #
     def test_get_release_hash_release(self):
         wfs = nf_core.list.Workflows()
         wfs.get_remote_workflows()
         pipeline = "methylseq"
```

### Comparing `nf-core-2.7.2/tests/test_launch.py` & `nf-core-2.8/tests/test_launch.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_licenses.py` & `nf-core-2.8/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_lint.py` & `nf-core-2.8/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_lint_utils.py` & `nf-core-2.8/tests/test_lint_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_list.py` & `nf-core-2.8/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_modules.py` & `nf-core-2.8/tests/test_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 """
 
 import os
 import shutil
 import tempfile
 import unittest
 
-import requests_mock
+import requests_cache
+import responses
 
 import nf_core.create
 import nf_core.modules
 
 from .utils import (
     GITLAB_BRANCH_TEST_BRANCH,
     GITLAB_BRANCH_TEST_OLD_SHA,
     GITLAB_DEFAULT_BRANCH,
     GITLAB_URL,
     OLD_TRIMGALORE_BRANCH,
     OLD_TRIMGALORE_SHA,
-    mock_api_calls,
+    mock_anaconda_api_calls,
+    mock_biocontainers_api_calls,
 )
 
 
 def create_modules_repo_dummy(tmp_dir):
     """Create a dummy copy of the nf-core/modules repo"""
 
     root_dir = os.path.join(tmp_dir, "modules")
@@ -31,19 +33,32 @@
     os.makedirs(os.path.join(root_dir, "tests", "config"))
     with open(os.path.join(root_dir, "tests", "config", "pytest_modules.yml"), "w") as fh:
         fh.writelines(["test:", "\n  - modules/test/**", "\n  - tests/modules/test/**"])
     with open(os.path.join(root_dir, ".nf-core.yml"), "w") as fh:
         fh.writelines(["repository_type: modules", "\n", "org_path: nf-core", "\n"])
 
     # mock biocontainers and anaconda response
-    with requests_mock.Mocker() as mock:
-        mock_api_calls(mock, "bpipe", "0.9.11--hdfd78af_0")
+    with responses.RequestsMock() as rsps:
+        mock_anaconda_api_calls(rsps, "bpipe", "0.9.11--hdfd78af_0")
+        mock_biocontainers_api_calls(rsps, "bpipe", "0.9.11--hdfd78af_0")
         # bpipe is a valid package on bioconda that is very unlikely to ever be added to nf-core/modules
         module_create = nf_core.modules.ModuleCreate(root_dir, "bpipe/test", "@author", "process_single", False, False)
-        module_create.create()
+        with requests_cache.disabled():
+            module_create.create()
+
+    # Remove doi from meta.yml which makes lint fail
+    meta_yml = os.path.join(root_dir, "modules", "nf-core", "bpipe", "test", "meta.yml")
+    with open(meta_yml, "r") as fh:
+        lines = fh.readlines()
+    for line_index in range(len(lines)):
+        if "doi" in lines[line_index]:
+            to_pop = line_index
+    lines.pop(to_pop)
+    with open(meta_yml, "w") as fh:
+        fh.writelines(lines)
 
     return root_dir
 
 
 class TestModules(unittest.TestCase):
     """Class for modules tests"""
 
@@ -51,47 +66,47 @@
         """Create a new PipelineSchema and Launch objects"""
         self.tmp_dir = tempfile.mkdtemp()
         self.component_type = "modules"
 
         # Set up the schema
         root_repo_dir = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
         self.template_dir = os.path.join(root_repo_dir, "nf_core", "pipeline-template")
-        self.pipeline_dir = os.path.join(self.tmp_dir, "mypipeline")
+        self.pipeline_name = "mypipeline"
+        self.pipeline_dir = os.path.join(self.tmp_dir, self.pipeline_name)
         nf_core.create.PipelineCreate(
-            "mypipeline", "it is mine", "me", no_git=True, outdir=self.pipeline_dir, plain=True
+            self.pipeline_name, "it is mine", "me", no_git=True, outdir=self.pipeline_dir, plain=True
         ).init_pipeline()
         # Set up install objects
         self.mods_install = nf_core.modules.ModuleInstall(self.pipeline_dir, prompt=False, force=True)
-        self.mods_install_alt = nf_core.modules.ModuleInstall(self.pipeline_dir, prompt=True, force=True)
         self.mods_install_old = nf_core.modules.ModuleInstall(
             self.pipeline_dir,
             prompt=False,
             force=False,
             sha=OLD_TRIMGALORE_SHA,
             remote_url=GITLAB_URL,
             branch=OLD_TRIMGALORE_BRANCH,
         )
         self.mods_install_trimgalore = nf_core.modules.ModuleInstall(
             self.pipeline_dir,
             prompt=False,
-            force=True,
+            force=False,
             remote_url=GITLAB_URL,
             branch=OLD_TRIMGALORE_BRANCH,
         )
         self.mods_install_gitlab = nf_core.modules.ModuleInstall(
             self.pipeline_dir,
             prompt=False,
-            force=True,
+            force=False,
             remote_url=GITLAB_URL,
             branch=GITLAB_DEFAULT_BRANCH,
         )
         self.mods_install_gitlab_old = nf_core.modules.ModuleInstall(
             self.pipeline_dir,
             prompt=False,
-            force=True,
+            force=False,
             remote_url=GITLAB_URL,
             branch=GITLAB_BRANCH_TEST_BRANCH,
             sha=GITLAB_BRANCH_TEST_OLD_SHA,
         )
 
         # Set up remove objects
         self.mods_remove = nf_core.modules.ModuleRemove(self.pipeline_dir)
@@ -142,25 +157,27 @@
     from .modules.info import (
         test_modules_info_in_modules_repo,
         test_modules_info_local,
         test_modules_info_remote,
         test_modules_info_remote_gitlab,
     )
     from .modules.install import (
+        test_modules_install_alternate_remote,
         test_modules_install_different_branch_fail,
         test_modules_install_different_branch_succeed,
         test_modules_install_emptypipeline,
         test_modules_install_from_gitlab,
         test_modules_install_nomodule,
         test_modules_install_nopipeline,
         test_modules_install_tracking,
         test_modules_install_trimgalore,
         test_modules_install_trimgalore_twice,
     )
     from .modules.lint import (
+        test_modules_lint_check_process_labels,
         test_modules_lint_empty,
         test_modules_lint_gitlab_modules,
         test_modules_lint_multiple_remotes,
         test_modules_lint_new_modules,
         test_modules_lint_no_gitlab,
         test_modules_lint_patched_modules,
         test_modules_lint_trimgalore,
@@ -195,14 +212,15 @@
     from .modules.patch import (
         test_create_patch_change,
         test_create_patch_no_change,
         test_create_patch_try_apply_failed,
         test_create_patch_try_apply_successful,
         test_create_patch_update_fail,
         test_create_patch_update_success,
+        test_remove_patch,
     )
     from .modules.remove import (
         test_modules_remove_multiqc_from_gitlab,
         test_modules_remove_trimgalore,
         test_modules_remove_trimgalore_uninstalled,
     )
     from .modules.update import (
```

### Comparing `nf-core-2.7.2/tests/test_refgenie.py` & `nf-core-2.8/tests/test_refgenie.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 
 import os
 import shlex
 import subprocess
 import tempfile
 import unittest
 
+import yaml
+
 
 class TestRefgenie(unittest.TestCase):
     """Class for refgenie tests"""
 
     def setUp(self):
         """
         Prepare a refgenie config file
         """
         self.tmp_dir = tempfile.mkdtemp()
         self.NXF_HOME = os.path.join(self.tmp_dir, ".nextflow")
         self.NXF_REFGENIE_PATH = os.path.join(self.NXF_HOME, "nf-core", "refgenie_genomes.config")
         self.REFGENIE = os.path.join(self.tmp_dir, "genomes_config.yaml")
+        self.translation_file = os.path.join(self.tmp_dir, "alias_translations.yaml")
         # Set NXF_HOME environment variable
         # avoids adding includeConfig statement to config file outside the current tmpdir
         try:
             self.NXF_HOME_ORIGINAL = os.environ["NXF_HOME"]
         except:
             self.NXF_HOME_ORIGINAL = None
         os.environ["NXF_HOME"] = self.NXF_HOME
@@ -33,14 +36,18 @@
         # Initialize a refgenie config
         os.system(f"refgenie init -c {self.REFGENIE}")
 
         # Add NXF_REFGENIE_PATH to refgenie config
         with open(self.REFGENIE, "a") as fh:
             fh.write(f"nextflow_config: {os.path.join(self.NXF_REFGENIE_PATH)}\n")
 
+        # Add an alias translation to YAML file
+        with open(self.translation_file, "a") as fh:
+            fh.write("ensembl_gtf: gtf\n")
+
     def tearDown(self) -> None:
         # Remove the tempdir again
         os.system(f"rm -rf {self.tmp_dir}")
         # Reset NXF_HOME environment variable
         if self.NXF_HOME_ORIGINAL is None:
             del os.environ["NXF_HOME"]
         else:
@@ -49,7 +56,17 @@
     def test_update_refgenie_genomes_config(self):
         """Test that listing pipelines works"""
         # Populate the config with a genome
         cmd = f"refgenie pull t7/fasta -c {self.REFGENIE}"
         out = subprocess.check_output(shlex.split(cmd), stderr=subprocess.STDOUT)
 
         assert "Updated nf-core genomes config" in str(out)
+
+    def test_asset_alias_translation(self):
+        """Test that asset aliases are translated correctly"""
+        # Populate the config with a genome
+        cmd = f"refgenie pull hg38/ensembl_gtf -c {self.REFGENIE}"
+        subprocess.check_output(shlex.split(cmd), stderr=subprocess.STDOUT)
+        cmd = f"cat {self.NXF_REFGENIE_PATH}"
+        out = subprocess.check_output(shlex.split(cmd), stderr=subprocess.STDOUT)
+        assert "      gtf                  = " in str(out)
+        assert "      ensembl_gtf          = " not in str(out)
```

### Comparing `nf-core-2.7.2/tests/test_schema.py` & `nf-core-2.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_subworkflows.py` & `nf-core-2.8/tests/test_subworkflows.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 """
 
 import os
 import shutil
 import tempfile
 import unittest
 
-import requests_mock
+import responses
 
 import nf_core.create
 import nf_core.modules
 import nf_core.subworkflows
 
-from .utils import GITLAB_SUBWORKFLOWS_BRANCH, GITLAB_URL, OLD_SUBWORKFLOWS_SHA
+from .utils import (
+    GITLAB_SUBWORKFLOWS_BRANCH,
+    GITLAB_SUBWORKFLOWS_ORG_PATH_BRANCH,
+    GITLAB_URL,
+    OLD_SUBWORKFLOWS_SHA,
+)
 
 
 def create_modules_repo_dummy(tmp_dir):
     """Create a dummy copy of the nf-core/modules repo"""
 
     root_dir = os.path.join(tmp_dir, "modules")
     os.makedirs(os.path.join(root_dir, "modules"))
@@ -26,17 +31,17 @@
     os.makedirs(os.path.join(root_dir, "tests", "subworkflows"))
     os.makedirs(os.path.join(root_dir, "tests", "config"))
     with open(os.path.join(root_dir, "tests", "config", "pytest_modules.yml"), "w") as fh:
         fh.writelines(["test:", "\n  - modules/test/**", "\n  - tests/modules/test/**"])
     with open(os.path.join(root_dir, ".nf-core.yml"), "w") as fh:
         fh.writelines(["repository_type: modules", "\n", "org_path: nf-core", "\n"])
 
-    with requests_mock.Mocker() as mock:
-        subworkflow_create = nf_core.subworkflows.SubworkflowCreate(root_dir, "test_subworkflow", "@author", True)
-        subworkflow_create.create()
+    # TODO Add a mock here
+    subworkflow_create = nf_core.subworkflows.SubworkflowCreate(root_dir, "test_subworkflow", "@author", True)
+    subworkflow_create.create()
 
     return root_dir
 
 
 class TestSubworkflows(unittest.TestCase):
     """Class for subworkflows tests"""
 
@@ -44,27 +49,35 @@
         """Create a new PipelineStructure and Launch objects"""
         self.tmp_dir = tempfile.mkdtemp()
         self.component_type = "subworkflows"
 
         # Set up the pipeline structure
         root_repo_dir = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
         self.template_dir = os.path.join(root_repo_dir, "nf_core", "pipeline-template")
-        self.pipeline_dir = os.path.join(self.tmp_dir, "mypipeline")
+        self.pipeline_name = "mypipeline"
+        self.pipeline_dir = os.path.join(self.tmp_dir, self.pipeline_name)
         nf_core.create.PipelineCreate(
-            "mypipeline", "it is mine", "me", no_git=True, outdir=self.pipeline_dir, plain=True
+            self.pipeline_name, "it is mine", "me", no_git=True, outdir=self.pipeline_dir, plain=True
         ).init_pipeline()
 
         # Set up the nf-core/modules repo dummy
         self.nfcore_modules = create_modules_repo_dummy(self.tmp_dir)
 
         # Set up install objects
         self.subworkflow_install = nf_core.subworkflows.SubworkflowInstall(self.pipeline_dir, prompt=False, force=False)
         self.subworkflow_install_gitlab = nf_core.subworkflows.SubworkflowInstall(
             self.pipeline_dir, prompt=False, force=False, remote_url=GITLAB_URL, branch=GITLAB_SUBWORKFLOWS_BRANCH
         )
+        self.subworkflow_install_gitlab_same_org_path = nf_core.subworkflows.SubworkflowInstall(
+            self.pipeline_dir,
+            prompt=False,
+            force=False,
+            remote_url=GITLAB_URL,
+            branch=GITLAB_SUBWORKFLOWS_ORG_PATH_BRANCH,
+        )
         self.subworkflow_install_old = nf_core.subworkflows.SubworkflowInstall(
             self.pipeline_dir,
             prompt=False,
             force=False,
             sha=OLD_SUBWORKFLOWS_SHA,
         )
         self.subworkflow_install_module_change = nf_core.subworkflows.SubworkflowInstall(
@@ -89,22 +102,30 @@
     ################################################
 
     from .subworkflows.create import (
         test_subworkflows_create_fail_exists,
         test_subworkflows_create_nfcore_modules,
         test_subworkflows_create_succeed,
     )
+    from .subworkflows.create_test_yml import (
+        test_subworkflows_create_test_yml_check_inputs,
+        test_subworkflows_create_test_yml_entry_points,
+        test_subworkflows_create_test_yml_get_md5,
+        test_subworkflows_custom_yml_dumper,
+        test_subworkflows_test_file_dict,
+    )
     from .subworkflows.info import (
         test_subworkflows_info_in_modules_repo,
         test_subworkflows_info_local,
         test_subworkflows_info_remote,
         test_subworkflows_info_remote_gitlab,
     )
     from .subworkflows.install import (
         test_subworkflow_install_nopipeline,
+        test_subworkflows_install_alternate_remote,
         test_subworkflows_install_bam_sort_stats_samtools,
         test_subworkflows_install_bam_sort_stats_samtools_twice,
         test_subworkflows_install_different_branch_fail,
         test_subworkflows_install_emptypipeline,
         test_subworkflows_install_from_gitlab,
         test_subworkflows_install_nosubworkflow,
         test_subworkflows_install_tracking,
```

### Comparing `nf-core-2.7.2/tests/test_sync.py` & `nf-core-2.8/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/test_test_utils.py` & `nf-core-2.8/tests/test_test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 def test_tmp_folder_does_not_exist_after():
     tmp_folder = with_temporary_folder(lambda x: x)()
     assert not Path(tmp_folder).exists()
 
 
 def test_set_wd():
-
     with tempfile.TemporaryDirectory() as tmpdirname:
         with set_wd(tmpdirname):
             context_wd = Path().resolve()
         assert context_wd == Path(tmpdirname).resolve()
         assert context_wd != Path().resolve()
```

### Comparing `nf-core-2.7.2/tests/test_utils.py` & `nf-core-2.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nf-core-2.7.2/tests/utils.py` & `nf-core-2.8/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,31 @@
 
 import functools
 import os
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 
-OLD_TRIMGALORE_SHA = "06348dffce2a732fc9e656bdc5c64c3e02d302cb"
+import responses
+
+import nf_core.modules
+
+OLD_TRIMGALORE_SHA = "9b7a3bdefeaad5d42324aa7dd50f87bea1b04386"
 OLD_TRIMGALORE_BRANCH = "mimic-old-trimgalore"
 GITLAB_URL = "https://gitlab.com/nf-core/modules-test.git"
-GITLAB_REPO = "nf-core"
+GITLAB_REPO = "nf-core-test"
 GITLAB_DEFAULT_BRANCH = "main"
 GITLAB_SUBWORKFLOWS_BRANCH = "subworkflows"
+GITLAB_SUBWORKFLOWS_ORG_PATH_BRANCH = "subworkflows-org-path"
 OLD_SUBWORKFLOWS_SHA = "f3c078809a2513f1c95de14f6633fe1f03572fdb"
 # Branch test stuff
 GITLAB_BRANCH_TEST_BRANCH = "branch-tester"
-GITLAB_BRANCH_TEST_OLD_SHA = "bce3f17980b8d1beae5e917cfd3c65c0c69e04b5"
-GITLAB_BRANCH_TEST_NEW_SHA = "2f5f180f6e705bb81d6e7742dc2f24bf4a0c721e"
+GITLAB_BRANCH_ORG_PATH_BRANCH = "org-path"
+GITLAB_BRANCH_TEST_OLD_SHA = "e772abc22c1ff26afdf377845c323172fb3c19ca"
+GITLAB_BRANCH_TEST_NEW_SHA = "7d73e21f30041297ea44367f2b4fd4e045c0b991"
 
 
 def with_temporary_folder(func):
     """
     Call the decorated function under the tempfile.TemporaryDirectory
     context manager. Pass the temporary directory name to the decorated
     function
@@ -64,39 +70,41 @@
     os.chdir(path)
     try:
         yield
     finally:
         os.chdir(start_wd)
 
 
-def mock_api_calls(mock, module, version):
-    """Mock biocontainers and anaconda api calls for module"""
-    biocontainers_api_url = (
-        f"https://api.biocontainers.pro/ga4gh/trs/v2/tools/{module}/versions/{module}-{version.split('--')[0]}"
-    )
+def mock_anaconda_api_calls(rsps: responses.RequestsMock, module, version):
+    """Mock anaconda api calls for module"""
     anaconda_api_url = f"https://api.anaconda.org/package/bioconda/{module}"
     anaconda_mock = {
-        "status_code": 200,
         "latest_version": version.split("--")[0],
         "summary": "",
-        "doc_url": "",
-        "dev_url": "",
+        "doc_url": "http://test",
+        "dev_url": "http://test",
         "files": [{"version": version.split("--")[0]}],
         "license": "",
     }
+    rsps.get(anaconda_api_url, json=anaconda_mock, status=200)
+
+
+def mock_biocontainers_api_calls(rsps: responses.RequestsMock, module, version):
+    """Mock biocontainers api calls for module"""
+    biocontainers_api_url = (
+        f"https://api.biocontainers.pro/ga4gh/trs/v2/tools/{module}/versions/{module}-{version.split('--')[0]}"
+    )
     biocontainers_mock = {
-        "status_code": 200,
         "images": [
             {
                 "image_type": "Singularity",
                 "image_name": f"https://depot.galaxyproject.org/singularity/{module}:{version}",
                 "updated": "2021-09-04T00:00:00Z",
             },
             {
                 "image_type": "Docker",
-                "image_name": f"quay.io/biocontainers/{module}:{version}",
+                "image_name": f"biocontainers/{module}:{version}",
                 "updated": "2021-09-04T00:00:00Z",
             },
         ],
     }
-    mock.register_uri("GET", anaconda_api_url, json=anaconda_mock)
-    mock.register_uri("GET", biocontainers_api_url, json=biocontainers_mock)
+    rsps.get(biocontainers_api_url, json=biocontainers_mock, status=200)
```

