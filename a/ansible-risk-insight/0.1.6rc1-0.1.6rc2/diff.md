# Comparing `tmp/ansible-risk-insight-0.1.6rc1.tar.gz` & `tmp/ansible-risk-insight-0.1.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.6rc1.tar", last modified: Fri Apr 28 05:28:44 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.6rc2.tar", last modified: Fri Apr 28 07:49:26 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.6rc1.tar` & `ansible-risk-insight-0.1.6rc2.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.470151 ansible-risk-insight-0.1.6rc1/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.411484 ansible-risk-insight-0.1.6rc1/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.417048 ansible-risk-insight-0.1.6rc1/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.6rc1/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 05:28:44.469996 ansible-risk-insight-0.1.6rc1/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.427204 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-28 05:28:19.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.430035 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.435013 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.435195 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.437692 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-13 17:26:40.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    75964 2023-04-28 05:12:53.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    43989 2023-04-28 05:12:52.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8092 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.456970 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6282 2023-04-28 04:49:11.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    46832 2023-04-28 04:13:42.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.428168 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.412210 ansible-risk-insight-0.1.6rc1/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.460119 ansible-risk-insight-0.1.6rc1/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.462691 ansible-risk-insight-0.1.6rc1/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.6rc1/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.6rc1/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc1/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc1/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.466153 ansible-risk-insight-0.1.6rc1/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.466653 ansible-risk-insight-0.1.6rc1/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.467031 ansible-risk-insight-0.1.6rc1/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc1/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc1/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.467299 ansible-risk-insight-0.1.6rc1/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc1/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.6rc1/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc1/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-28 05:28:44.470206 ansible-risk-insight-0.1.6rc1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.467603 ansible-risk-insight-0.1.6rc1/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc1/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413326 ansible-risk-insight-0.1.6rc1/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.412883 ansible-risk-insight-0.1.6rc1/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468203 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413020 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413241 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468484 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468749 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468994 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413383 ansible-risk-insight-0.1.6rc1/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413588 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.469205 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.469385 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.469642 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.6rc1/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.109335 ansible-risk-insight-0.1.6rc2/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.047314 ansible-risk-insight-0.1.6rc2/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.054451 ansible-risk-insight-0.1.6rc2/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.6rc2/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 07:49:26.109140 ansible-risk-insight-0.1.6rc2/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.064592 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-28 07:49:19.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.067284 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.072013 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.072186 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.073875 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-13 17:26:40.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    75964 2023-04-28 05:12:53.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    43989 2023-04-28 05:12:52.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8092 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.092936 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6282 2023-04-28 04:49:11.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3050 2023-04-28 06:29:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46832 2023-04-28 04:13:42.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.065569 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-28 07:49:26.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.048139 ansible-risk-insight-0.1.6rc2/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.096663 ansible-risk-insight-0.1.6rc2/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.099954 ansible-risk-insight-0.1.6rc2/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.6rc2/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.6rc2/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc2/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc2/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.103668 ansible-risk-insight-0.1.6rc2/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.104259 ansible-risk-insight-0.1.6rc2/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.104538 ansible-risk-insight-0.1.6rc2/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc2/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc2/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.104962 ansible-risk-insight-0.1.6rc2/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc2/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.6rc2/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc2/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-28 07:49:26.109397 ansible-risk-insight-0.1.6rc2/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.105331 ansible-risk-insight-0.1.6rc2/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc2/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049686 ansible-risk-insight-0.1.6rc2/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049164 ansible-risk-insight-0.1.6rc2/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.106230 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049325 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049586 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.106668 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.106919 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.107426 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049747 ansible-risk-insight-0.1.6rc2/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.050002 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.107667 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.107968 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.108771 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.6rc2/tox.ini
```

### Comparing `ansible-risk-insight-0.1.6rc1/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.6rc2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/.github/workflows/test.yml` & `ansible-risk-insight-0.1.6rc2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/.gitignore` & `ansible-risk-insight-0.1.6rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/CONTRIBUTING.md` & `ansible-risk-insight-0.1.6rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/LICENSE` & `ansible-risk-insight-0.1.6rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/README.md` & `ansible-risk-insight-0.1.6rc2/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.6-rc1"
+__version__ = "0.1.6-rc2"
```

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/model_loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/models.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_assessment_model.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_detector.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,19 +18,36 @@
 
 from ansible_risk_insight.models import (
     AnsibleRunContext,
     RunTargetType,
     Rule,
     Severity,
     RuleTag as Tag,
+    Variable,
     VariableType,
     ArgumentsType,
 )
 
 
+def is_loop_var(value, task):
+    # `item` or alternative loop variable (if any) should not be replaced to avoid breaking loop
+    skip_variables = []
+    if task.spec.loop and isinstance(task.spec.loop, dict):
+        skip_variables.extend(list(task.spec.loop.keys()))
+
+    _v = value.replace(" ", "")
+
+    for var in skip_variables:
+        for _prefix in ["}}", "|", "."]:
+            pattern = "{{" + var + _prefix
+            if pattern in _v:
+                return True
+    return False
+
+
 @dataclass
 class VariableValidationRule(Rule):
     rule_id: str = "P004"
     description: str = "Validate variables and set annotations"
     enabled: bool = True
     name: str = "VariableValidation"
     version: str = "v0.0.1"
@@ -54,15 +71,16 @@
             v = task.variable_use[v_name]
             if v and v[-1].type == VariableType.Unknown:
                 if v_name not in undefined_variables:
                     undefined_variables.append(v_name)
                 if v_name not in unknown_name_vars and v_name not in task_arg_keys:
                     unknown_name_vars.append(v_name)
                 if v_name not in unnecessary_loop:
-                    if v_name.startswith("item."):
+                    v_str = "{{ " + v_name + " }}"
+                    if not is_loop_var(v_str, task):
                         unnecessary_loop.append({"name": v_name, "suggested": v_name.replace("item.", "")})
 
         task.set_annotation("variable.undefined_vars", undefined_variables, rule_id=self.rule_id)
         task.set_annotation("variable.unknown_name_vars", unknown_name_vars, rule_id=self.rule_id)
         task.set_annotation("variable.unnecessary_loop_vars", unnecessary_loop, rule_id=self.rule_id)
 
         return None
```

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/tree.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/data-struct.txt` & `ansible-risk-insight-0.1.6rc2/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.6rc2/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.6rc2/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.6rc2/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.6rc2/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/docs/annotation.md` & `ansible-risk-insight-0.1.6rc2/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/docs/customize_rules.md` & `ansible-risk-insight-0.1.6rc2/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.6rc2/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.6rc2/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.6rc2/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.6rc2/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/example/readme.md` & `ansible-risk-insight-0.1.6rc2/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.6rc2/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/example/sample.py` & `ansible-risk-insight-0.1.6rc2/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/mkdocs.yml` & `ansible-risk-insight-0.1.6rc2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/pyproject.toml` & `ansible-risk-insight-0.1.6rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/test/test_scanner.py` & `ansible-risk-insight-0.1.6rc2/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc1/tox.ini` & `ansible-risk-insight-0.1.6rc2/tox.ini`

 * *Files identical despite different names*

