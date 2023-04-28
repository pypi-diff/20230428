# Comparing `tmp/ansible-risk-insight-0.1.5rc1.tar.gz` & `tmp/ansible-risk-insight-0.1.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.5rc1.tar", last modified: Thu Apr 27 07:06:57 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.6rc1.tar", last modified: Fri Apr 28 05:28:44 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.5rc1.tar` & `ansible-risk-insight-0.1.6rc1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.966485 ansible-risk-insight-0.1.5rc1/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.924297 ansible-risk-insight-0.1.5rc1/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.929851 ansible-risk-insight-0.1.5rc1/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.5rc1/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.5rc1/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.5rc1/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.5rc1/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.5rc1/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-27 07:06:57.966313 ansible-risk-insight-0.1.5rc1/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.5rc1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.936019 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      662 2023-04-27 07:06:54.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.938122 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.941269 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.941414 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.942607 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-13 17:26:40.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    74282 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    40317 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8092 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.958263 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4968 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    46781 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.936914 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-27 07:06:57.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-27 07:06:57.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-27 07:06:57.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-27 07:06:57.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-27 07:06:57.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-27 07:06:57.000000 ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.5rc1/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.925210 ansible-risk-insight-0.1.5rc1/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.959493 ansible-risk-insight-0.1.5rc1/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.5rc1/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.5rc1/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.5rc1/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.5rc1/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.960418 ansible-risk-insight-0.1.5rc1/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.5rc1/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.5rc1/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.5rc1/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.5rc1/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.963612 ansible-risk-insight-0.1.5rc1/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.5rc1/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.963955 ansible-risk-insight-0.1.5rc1/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.964134 ansible-risk-insight-0.1.5rc1/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.5rc1/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.5rc1/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.964321 ansible-risk-insight-0.1.5rc1/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.5rc1/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.5rc1/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.5rc1/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.5rc1/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-27 07:06:57.966541 ansible-risk-insight-0.1.5rc1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.5rc1/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.964596 ansible-risk-insight-0.1.5rc1/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.5rc1/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.926676 ansible-risk-insight-0.1.5rc1/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.926052 ansible-risk-insight-0.1.5rc1/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.965013 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.926225 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.926541 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.965171 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.965368 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.965551 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.926760 ansible-risk-insight-0.1.5rc1/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.927107 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.965732 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.965898 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-27 07:06:57.966066 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.5rc1/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.5rc1/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.470151 ansible-risk-insight-0.1.6rc1/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.411484 ansible-risk-insight-0.1.6rc1/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.417048 ansible-risk-insight-0.1.6rc1/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.6rc1/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 05:28:44.469996 ansible-risk-insight-0.1.6rc1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.427204 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-28 05:28:19.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.430035 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.435013 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.435195 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.437692 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-13 17:26:40.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    75964 2023-04-28 05:12:53.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    43989 2023-04-28 05:12:52.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8092 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.456970 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6282 2023-04-28 04:49:11.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46832 2023-04-28 04:13:42.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.428168 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-28 05:28:44.000000 ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc1/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.412210 ansible-risk-insight-0.1.6rc1/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.460119 ansible-risk-insight-0.1.6rc1/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc1/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.462691 ansible-risk-insight-0.1.6rc1/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.6rc1/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.6rc1/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc1/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc1/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.466153 ansible-risk-insight-0.1.6rc1/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc1/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.466653 ansible-risk-insight-0.1.6rc1/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.467031 ansible-risk-insight-0.1.6rc1/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc1/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc1/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.467299 ansible-risk-insight-0.1.6rc1/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc1/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.6rc1/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc1/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc1/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-28 05:28:44.470206 ansible-risk-insight-0.1.6rc1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.467603 ansible-risk-insight-0.1.6rc1/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc1/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413326 ansible-risk-insight-0.1.6rc1/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.412883 ansible-risk-insight-0.1.6rc1/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468203 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413020 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413241 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468484 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468749 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.468994 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413383 ansible-risk-insight-0.1.6rc1/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.413588 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.469205 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.469385 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 05:28:44.469642 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc1/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.6rc1/tox.ini
```

### Comparing `ansible-risk-insight-0.1.5rc1/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.6rc1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/.github/workflows/test.yml` & `ansible-risk-insight-0.1.6rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/.gitignore` & `ansible-risk-insight-0.1.6rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/CONTRIBUTING.md` & `ansible-risk-insight-0.1.6rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/LICENSE` & `ansible-risk-insight-0.1.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/README.md` & `ansible-risk-insight-0.1.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.5rc1"
+__version__ = "0.1.6-rc1"
```

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/model_loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1535,14 +1535,15 @@
 
 
 @dataclass
 class AnsibleRunContext(object):
     sequence: RunTargetList = field(default_factory=RunTargetList)
     root_key: str = ""
     parent: Object = None
+    ram_client: any = None
 
     # used by rule check
     current: RunTarget = None
     _i: int = 0
 
     # used if ram generate / other data generation by loop
     last_item: bool = False
@@ -1567,54 +1568,58 @@
         self._i += 1
         return t
 
     def __getitem__(self, i):
         return self.sequence[i]
 
     @staticmethod
-    def from_tree(tree: ObjectList, parent: Object = None, last_item: bool = False):
+    def from_tree(tree: ObjectList, parent: Object = None, last_item: bool = False, ram_client=None):
         if not tree:
             return AnsibleRunContext(parent=parent, last_item=last_item)
         if len(tree.items) == 0:
             return AnsibleRunContext(parent=parent, last_item=last_item)
 
         root_key = tree.items[0].spec.key
         sequence_items = []
         for item in tree.items:
             if not isinstance(item, RunTarget):
                 continue
             sequence_items.append(item)
         tl = RunTargetList(items=sequence_items)
-        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item)
+        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item, ram_client=ram_client)
 
     @staticmethod
-    def from_targets(targets: List[RunTarget], root_key: str = "", parent: Object = None, last_item: bool = False):
+    def from_targets(targets: List[RunTarget], root_key: str = "", parent: Object = None, last_item: bool = False, ram_client=None):
         if not root_key:
             if len(targets) > 0:
                 root_key = targets[0].spec.key
         tl = RunTargetList(items=targets)
-        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item)
+        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item, ram_client=ram_client)
 
     def find(self, target: RunTarget):
         for t in self.sequence:
             if t.key == target.key:
                 return t
         return None
 
     def before(self, target: RunTarget):
         targets = []
         for rt in self.sequence:
             if rt.key == target.key:
                 break
             targets.append(rt)
-        return AnsibleRunContext.from_targets(targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item)
+        return AnsibleRunContext.from_targets(
+            targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item, ram_client=self.ram_client
+        )
 
     def search(self, cond: AnnotationCondition):
         targets = [t for t in self.sequence if t.type == RunTargetType.Task and t.has_annotation_by_condition(cond)]
-        return AnsibleRunContext.from_targets(targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item)
+        return AnsibleRunContext.from_targets(
+            targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item, ram_client=self.ram_client
+        )
 
     def is_end(self, target: RunTarget):
         if len(self) == 0:
             return False
         return target.key == self.sequence[-1].key
 
     def is_last_task(self, target: RunTarget):
@@ -1627,15 +1632,17 @@
 
     def is_begin(self, target: RunTarget):
         if len(self) == 0:
             return False
         return target.key == self.sequence[0].key
 
     def copy(self):
-        return AnsibleRunContext.from_targets(targets=self.sequence.items, root_key=self.root_key, parent=self.parent, last_item=self.last_item)
+        return AnsibleRunContext.from_targets(
+            targets=self.sequence.items, root_key=self.root_key, parent=self.parent, last_item=self.last_item, ram_client=self.ram_client
+        )
 
     @property
     def info(self):
         if not self.root_key:
             return {}
         return get_obj_info_by_key(self.root_key)
 
@@ -2118,14 +2125,63 @@
 
     def __eq__(self, tfm):
         if not isinstance(tfm, TaskFileMetadata):
             return False
         return self.key == tfm.key and self.name == tfm.name and self.type == tfm.type and self.version == tfm.version and self.hash == tfm.hash
 
 
+@dataclass
+class ActionGroupMetadata(object):
+    group_name: str = ""
+    group_modules: list = field(default_factory=list)
+    type: str = ""
+    name: str = ""
+    version: str = ""
+    hash: str = ""
+
+    @staticmethod
+    def from_action_group(group_name: str, group_modules: list, metadata: dict):
+        if not group_name:
+            return None
+
+        if not group_modules:
+            return None
+
+        agm = ActionGroupMetadata()
+        agm.group_name = group_name
+        agm.group_modules = group_modules
+        agm.type = metadata.get("type", "")
+        agm.name = metadata.get("name", "")
+        agm.version = metadata.get("version", "")
+        agm.hash = metadata.get("hash", "")
+        return agm
+
+    @staticmethod
+    def from_dict(d: dict):
+        agm = ActionGroupMetadata()
+        agm.group_name = d.get("group_name", "")
+        agm.group_modules = d.get("group_modules", "")
+        agm.type = d.get("type", "")
+        agm.name = d.get("name", "")
+        agm.version = d.get("version", "")
+        agm.hash = d.get("hash", "")
+        return agm
+
+    def __eq__(self, agm):
+        if not isinstance(agm, ActionGroupMetadata):
+            return False
+        return (
+            self.group_name == agm.group_name
+            and self.name == agm.name
+            and self.type == agm.type
+            and self.version == agm.version
+            and self.hash == agm.hash
+        )
+
+
 # following ansible-lint severity levels
 class Severity:
     VERY_HIGH = "very_high"
     HIGH = "high"
     MEDIUM = "medium"
     LOW = "low"
     VERY_LOW = "very_low"
```

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_assessment_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     Collection,
     Module,
     ModuleMetadata,
     Role,
     RoleMetadata,
     TaskFile,
     TaskFileMetadata,
+    ActionGroupMetadata,
 )
 from .findings import Findings
 from .utils import (
     escape_url,
     version_to_num,
     diff_files_data,
     is_test_object,
@@ -45,14 +46,15 @@
 from .keyutil import get_obj_info_by_key, make_imported_taskfile_key
 from .model_loader import load_builtin_modules
 
 
 module_index_name = "module_index.json"
 role_index_name = "role_index.json"
 taskfile_index_name = "taskfile_index.json"
+action_group_index_name = "action_group_index.json"
 
 
 @dataclass
 class RAMClient(object):
     root_dir: str = ""
 
     findings_json_list_cache: list = field(default_factory=list)
@@ -67,14 +69,17 @@
 
     builtin_modules_cache: dict = field(default_factory=dict)
 
     module_index: dict = field(default_factory=dict)
     role_index: dict = field(default_factory=dict)
     taskfile_index: dict = field(default_factory=dict)
 
+    # used for grouped module_defaults such as `group/aws`
+    action_group_index: dict = field(default_factory=dict)
+
     max_cache_size: int = 200
 
     def __post_init__(self):
         module_index_path = os.path.join(self.root_dir, "indices", module_index_name)
         if os.path.exists(module_index_path):
             with open(module_index_path, "r") as file:
                 self.module_index = json.load(file)
@@ -85,14 +90,19 @@
                 self.role_index = json.load(file)
 
         taskfile_index_path = os.path.join(self.root_dir, "indices", taskfile_index_name)
         if os.path.exists(taskfile_index_path):
             with open(taskfile_index_path, "r") as file:
                 self.taskfile_index = json.load(file)
 
+        action_group_index_path = os.path.join(self.root_dir, "indices", action_group_index_name)
+        if os.path.exists(action_group_index_path):
+            with open(action_group_index_path, "r") as file:
+                self.action_group_index = json.load(file)
+
     def clear_old_cache(self):
         size = self.max_cache_size
         self._remove_old_item(self.findings_cache, size)
         self._remove_old_item(self.findings_search_cache, size)
         self._remove_old_item(self.module_search_cache, size)
         self._remove_old_item(self.role_search_cache, size)
         self._remove_old_item(self.taskfile_search_cache, size)
@@ -121,14 +131,15 @@
 
         self.clear_old_cache()
 
     def register_indices_to_ram(self, findings: Findings, include_test_contents: bool = False):
         self.register_module_index_to_ram(findings=findings, include_test_contents=include_test_contents)
         self.register_role_index_to_ram(findings=findings, include_test_contents=include_test_contents)
         self.register_taskfile_index_to_ram(findings=findings, include_test_contents=include_test_contents)
+        self.register_action_group_index_to_ram(findings=findings)
 
     def register_module_index_to_ram(self, findings: Findings, include_test_contents: bool = False):
         new_data_found = False
         modules = self.load_module_index()
         for module in findings.root_definitions.get("definitions", {}).get("modules", []):
             if not isinstance(module, Module):
                 continue
@@ -178,22 +189,20 @@
                         current.append(m_meta)
                         new_data_found = True
                     modules.update({short_name: current})
         if new_data_found:
             self.save_module_index(modules)
         return
 
-    def register_role_index_to_ram(self, findings: Findings, include_test_contents: bool = False):
+    def register_role_index_to_ram(self, findings: Findings):
         new_data_found = False
         roles = self.load_role_index()
         for role in findings.root_definitions.get("definitions", {}).get("roles", []):
             if not isinstance(role, Role):
                 continue
-            if include_test_contents and is_test_object(role.defined_in):
-                continue
             r_meta = RoleMetadata.from_role(role, findings.metadata)
             current = roles.get(r_meta.fqcn, [])
             exists = False
             for r_dict in current:
                 r = None
                 if isinstance(r_dict, dict):
                     r = RoleMetadata.from_dict(r_dict)
@@ -238,14 +247,67 @@
                 current.append(tf_meta)
                 new_data_found = True
             taskfiles.update({taskfile.key: current})
         if new_data_found:
             self.save_taskfile_index(taskfiles)
         return
 
+    def register_action_group_index_to_ram(self, findings: Findings, include_test_contents: bool = False):
+        new_data_found = False
+        action_groups = self.load_action_group_index()
+
+        for collection in findings.root_definitions.get("definitions", {}).get("collections", []):
+            if not isinstance(collection, Collection):
+                continue
+            if collection.meta_runtime and isinstance(collection.meta_runtime, dict):
+                for group_name, group_modules in collection.meta_runtime.get("action_groups", {}).items():
+                    short_group_name = f"group/{group_name}"
+                    fq_group_name = f"group/{collection.name}.{group_name}"
+
+                    agm1 = ActionGroupMetadata.from_action_group(short_group_name, group_modules, findings.metadata)
+                    current1 = action_groups.get(short_group_name, [])
+                    exists = False
+                    for ag_dict in current1:
+                        ag = None
+                        if isinstance(ag_dict, dict):
+                            ag = ActionGroupMetadata.from_dict(ag_dict)
+                        elif isinstance(ag_dict, ActionGroupMetadata):
+                            ag = ag_dict
+                        if not ag:
+                            continue
+                        if ag == agm1:
+                            exists = True
+                            break
+                    if not exists:
+                        current1.append(agm1)
+                        new_data_found = True
+                    action_groups.update({short_group_name: current1})
+
+                    agm2 = ActionGroupMetadata.from_action_group(fq_group_name, group_modules, findings.metadata)
+                    current2 = action_groups.get(fq_group_name, [])
+                    exists = False
+                    for ag_dict in current2:
+                        ag = None
+                        if isinstance(ag_dict, dict):
+                            ag = ActionGroupMetadata.from_dict(ag_dict)
+                        elif isinstance(ag_dict, ActionGroupMetadata):
+                            ag = ag_dict
+                        if not ag:
+                            continue
+                        if ag == agm2:
+                            exists = True
+                            break
+                    if not exists:
+                        current2.append(agm2)
+                        new_data_found = True
+                    action_groups.update({fq_group_name: current2})
+        if new_data_found:
+            self.save_action_group_index(action_groups)
+        return
+
     def make_findings_dir_path(self, type, name, version, hash):
         type_root = type + "s"
         dir_name = name
         if type in [LoadType.PROJECT, LoadType.PLAYBOOK, LoadType.TASKFILE]:
             dir_name = escape_url(name)
         ver_str = version if version != "" else "unknown"
         hash_str = hash if hash != "" else "unknown"
@@ -727,14 +789,26 @@
                         search_end = True
                         break
             if search_end:
                 break
         self.task_search_cache[args_str] = matched_tasks
         return matched_tasks
 
+    def search_action_group(self, name, max_match=-1):
+        if max_match == 0:
+            return []
+
+        found_groups = []
+        if name in self.action_group_index and self.action_group_index[name]:
+            found_groups = self.action_group_index[name]
+
+        if max_match > 0 and len(found_groups) > max_match:
+            found_groups = found_groups[:max_match]
+        return found_groups
+
     def get_object_by_key(self, obj_key: str):
         obj_info = get_obj_info_by_key(obj_key)
         obj_type = obj_info.get("type", "")
         parent_name = obj_info.get("parent_name", "")
         type_str = obj_type + "s"
 
         search_patterns = os.path.join(self.root_dir, "collections", "findings", parent_name, "*", "*", "root", f"{type_str}.json")
@@ -888,14 +962,20 @@
 
     def save_taskfile_index(self, taskfiles):
         return self.save_index(taskfiles, taskfile_index_name)
 
     def load_taskfile_index(self):
         return self.load_index(taskfile_index_name)
 
+    def save_action_group_index(self, action_groups):
+        return self.save_index(action_groups, action_group_index_name)
+
+    def load_action_group_index(self):
+        return self.load_index(action_group_index_name)
+
     def save_error(self, error: str, out_dir: str):
         if out_dir == "":
             raise ValueError("output dir must be a non-empty value")
 
         if not os.path.exists(out_dir):
             os.makedirs(out_dir, exist_ok=True)
```

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/risk_detector.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ansible_risk_insight.models import (
     AnsibleRunContext,
     RunTargetType,
     Rule,
     Severity,
     RuleTag as Tag,
     ExecutableType,
+    ActionGroupMetadata,
 )
 
 
 @dataclass
 class ModuleArgumentKeyValidationRule(Rule):
     rule_id: str = "P002"
     description: str = "Validate module argument keys and set annotations"
@@ -55,14 +56,39 @@
                 elif len(parts) > 2:
                     module_short = ".".join(module_fqcn.split(".")[2:])
             default_args = {}
             if module_short and module_short in task.module_defaults:
                 default_args = task.module_defaults[module_short]
             elif module_fqcn and module_fqcn in task.module_defaults:
                 default_args = task.module_defaults[module_fqcn]
+            elif ctx.ram_client:
+                for group_name in task.module_defaults:
+                    tmp_args = task.module_defaults[group_name]
+                    found = False
+                    if not group_name.startswith("group/"):
+                        continue
+                    groups = ctx.ram_client.search_action_group(group_name)
+                    if not groups:
+                        continue
+                    for group_dict in groups:
+                        if not group_dict:
+                            continue
+                        if not isinstance(group_dict, dict):
+                            continue
+                        group = ActionGroupMetadata.from_dict(group_dict)
+                        if module_short and module_short in group.group_modules:
+                            found = True
+                            default_args = tmp_args
+                            break
+                        elif module_fqcn and module_fqcn in group.group_modules:
+                            found = True
+                            default_args = tmp_args
+                            break
+                    if found:
+                        break
 
             used_keys = []
             if isinstance(mo, dict):
                 used_keys = list(mo.keys())
             available_keys = []
             required_keys = []
             alias_reverse_map = {}
@@ -114,12 +140,13 @@
                 )
 
             task.set_annotation("module.wrong_arg_keys", wrong_keys, rule_id=self.rule_id)
             task.set_annotation("module.available_arg_keys", available_keys, rule_id=self.rule_id)
             task.set_annotation("module.required_arg_keys", required_keys, rule_id=self.rule_id)
             task.set_annotation("module.missing_required_arg_keys", missing_required_keys, rule_id=self.rule_id)
             task.set_annotation("module.available_args", available_args, rule_id=self.rule_id)
+            task.set_annotation("module.default_args", default_args, rule_id=self.rule_id)
             task.set_annotation("module.used_alias_and_real_keys", used_alias_and_real_keys, rule_id=self.rule_id)
 
         # TODO: find duplicate keys
 
         return None
```

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,21 +582,21 @@
                 for t_obj_list in self.trees:
                     lines.append(t_obj_list.to_one_line_json())
                 open(tree_rel_file, "w").write("\n".join(lines))
                 if not self.silent:
                     logger.info("  tree file saved")
         return
 
-    def resolve_variables(self):
+    def resolve_variables(self, ram_client=None):
         taskcalls_in_trees = resolve(self.trees, self.additional)
         self.taskcalls_in_trees = taskcalls_in_trees
 
         for i, tree in enumerate(self.trees):
             last_item = i + 1 == len(self.trees)
-            ctx = AnsibleRunContext.from_tree(tree=tree, parent=self.target_object, last_item=last_item)
+            ctx = AnsibleRunContext.from_tree(tree=tree, parent=self.target_object, last_item=last_item, ram_client=ram_client)
             self.contexts.append(ctx)
 
         if self.do_save:
             root_def_dir = self.__path_mappings["root_definitions"]
             tasks_in_t_path = os.path.join(root_def_dir, "tasks_in_trees.json")
             tasks_in_t_lines = []
             for d in taskcalls_in_trees:
@@ -1000,24 +1000,24 @@
         self.record_begin(time_records, "tree_construction")
         scandata.construct_trees(_ram_client)
         self.record_end(time_records, "tree_construction")
         if not self.silent:
             logger.debug("construct_trees() done")
 
         self.record_begin(time_records, "variable_resolution")
-        scandata.resolve_variables()
+        scandata.resolve_variables(_ram_client)
         self.record_end(time_records, "variable_resolution")
         if not self.silent:
             logger.debug("resolve_variables() done")
 
         self.record_begin(time_records, "module_annotators")
         scandata.annotate()
+        self.record_end(time_records, "module_annotators")
         if not self.silent:
             logger.debug("annotate() done")
-        self.record_end(time_records, "module_annotators")
 
         self.record_begin(time_records, "apply_rules")
         scandata.apply_rules()
         self.record_end(time_records, "apply_rules")
         if not self.silent:
             logger.debug("apply_rules() done")
```

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/tree.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.6rc1/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/data-struct.txt` & `ansible-risk-insight-0.1.6rc1/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.6rc1/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.6rc1/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.6rc1/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.6rc1/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/docs/annotation.md` & `ansible-risk-insight-0.1.6rc1/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/docs/customize_rules.md` & `ansible-risk-insight-0.1.6rc1/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.6rc1/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.6rc1/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.6rc1/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.6rc1/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/example/readme.md` & `ansible-risk-insight-0.1.6rc1/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.6rc1/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/example/sample.py` & `ansible-risk-insight-0.1.6rc1/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/mkdocs.yml` & `ansible-risk-insight-0.1.6rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/pyproject.toml` & `ansible-risk-insight-0.1.6rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/test/test_scanner.py` & `ansible-risk-insight-0.1.6rc1/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.6rc1/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.5rc1/tox.ini` & `ansible-risk-insight-0.1.6rc1/tox.ini`

 * *Files identical despite different names*

