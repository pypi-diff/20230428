# Comparing `tmp/fractal_server-1.2.2.tar.gz` & `tmp/fractal_server-1.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.2.tar", max compression
+gzip compressed data, was "fractal_server-1.2.3a0.tar", max compression
```

## Comparing `fractal_server-1.2.2.tar` & `fractal_server-1.2.3a0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.2/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.2/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.2/fractal_server/.gitignore
--rw-r--r--   0        0        0       22 2023-04-21 11:00:36.238422 fractal_server-1.2.2/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.2.2/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.2/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.2/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.2/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.2/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2740 2023-04-21 08:35:50.575851 fractal_server-1.2.2/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    21983 2023-04-19 09:17:04.678763 fractal_server-1.2.2/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    11794 2023-04-14 12:55:14.842206 fractal_server-1.2.2/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11398 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     2724 2023-04-14 12:55:14.842206 fractal_server-1.2.2/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.2/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.2/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8282 2023-04-20 08:57:46.572197 fractal_server-1.2.2/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19294 2023-04-17 13:34:24.748408 fractal_server-1.2.2/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5460 2023-04-17 13:34:24.748408 fractal_server-1.2.2/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.2.2/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.2.2/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.2.2/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.2/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3835 2023-04-21 11:00:14.178698 fractal_server-1.2.2/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.2/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-21 08:35:50.575851 fractal_server-1.2.2/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-04-21 11:00:14.178698 fractal_server-1.2.2/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.2/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-04-14 12:55:14.842206 fractal_server-1.2.2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    40272 2023-04-21 08:35:50.575851 fractal_server-1.2.2/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.2/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9749 2023-04-14 12:55:14.846206 fractal_server-1.2.2/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.2/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.2/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.2/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.2/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.2/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.2/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.2/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.2/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.2/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.2/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.2/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.2/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.2/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.2/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.2/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.2/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.2/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.2/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.2/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.2/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-04-20 07:11:45.695470 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-04-20 07:11:45.743469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-04-20 07:11:45.767469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-04-20 07:11:45.767469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-04-20 07:11:45.767469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-04-20 07:11:45.771469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-04-20 07:11:45.771469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2227 2023-04-20 07:11:45.775469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3046 2023-04-20 07:11:45.775469 fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.2/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.2/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.2/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.2/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.2/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.2/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.2/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.2/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.2/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12079 2023-04-17 13:34:24.748408 fractal_server-1.2.2/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.2/fractal_server/logger.py
--rw-r--r--   0        0        0     5805 2023-04-20 08:57:46.572197 fractal_server-1.2.2/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.2/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.2/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.2/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.2/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.2/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.2/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12782 2023-04-14 12:55:14.846206 fractal_server-1.2.2/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-04-14 12:55:14.846206 fractal_server-1.2.2/fractal_server/utils.py
--rw-r--r--   0        0        0     2625 2023-04-21 11:00:36.238422 fractal_server-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4091 1970-01-01 00:00:00.000000 fractal_server-1.2.2/setup.py
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 fractal_server-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.3a0/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.3a0/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.3a0/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-04-28 08:56:46.813130 fractal_server-1.2.3a0/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.2.3a0/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.3a0/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.3a0/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.3a0/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.3a0/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2783 2023-04-28 07:01:22.992049 fractal_server-1.2.3a0/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    22420 2023-04-28 08:39:47.649092 fractal_server-1.2.3a0/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    12019 2023-04-28 07:02:43.542576 fractal_server-1.2.3a0/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11503 2023-04-28 07:00:50.240679 fractal_server-1.2.3a0/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     2724 2023-04-14 12:55:14.842206 fractal_server-1.2.3a0/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.3a0/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3242 2023-04-28 08:08:47.092463 fractal_server-1.2.3a0/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8850 2023-04-28 08:39:14.233193 fractal_server-1.2.3a0/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19294 2023-04-17 13:34:24.748408 fractal_server-1.2.3a0/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5460 2023-04-17 13:34:24.748408 fractal_server-1.2.3a0/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.2.3a0/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.2.3a0/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.2.3a0/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3835 2023-04-21 11:00:14.178698 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-21 08:35:50.575851 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19861 2023-04-21 11:00:14.178698 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-04-14 12:55:14.842206 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    40272 2023-04-21 08:35:50.575851 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9749 2023-04-14 12:55:14.846206 fractal_server-1.2.3a0/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.3a0/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.3a0/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.3a0/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.3a0/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.3a0/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.3a0/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.3a0/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.3a0/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.3a0/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.3a0/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.3a0/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.3a0/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.3a0/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.3a0/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.3a0/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.3a0/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.3a0/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.3a0/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.3a0/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.3a0/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-04-20 07:11:45.695470 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-04-20 07:11:45.743469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-04-20 07:11:45.767469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-04-20 07:11:45.767469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-04-20 07:11:45.767469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-04-20 07:11:45.771469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-04-20 07:11:45.771469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2227 2023-04-20 07:11:45.775469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3046 2023-04-20 07:11:45.775469 fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.3a0/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.3a0/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.3a0/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.3a0/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.3a0/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.3a0/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.3a0/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.3a0/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.3a0/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12079 2023-04-28 06:28:20.387228 fractal_server-1.2.3a0/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.3a0/fractal_server/logger.py
+-rw-r--r--   0        0        0     5805 2023-04-28 06:28:20.387228 fractal_server-1.2.3a0/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.3a0/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.3a0/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.3a0/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.3a0/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.3a0/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.3a0/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.3a0/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.3a0/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.3a0/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12782 2023-04-14 12:55:14.846206 fractal_server-1.2.3a0/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-04-14 12:55:14.846206 fractal_server-1.2.3a0/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-04-28 08:56:46.813130 fractal_server-1.2.3a0/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.3a0/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.3a0/PKG-INFO
```

### Comparing `fractal_server-1.2.2/LICENSE` & `fractal_server-1.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/README.md` & `fractal_server-1.2.3a0/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/__main__.py` & `fractal_server-1.2.3a0/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/alembic.ini` & `fractal_server-1.2.3a0/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/api/__init__.py` & `fractal_server-1.2.3a0/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.3a0/fractal_server/app/api/v1/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         metadata_file = Path(job_read.working_dir) / METADATA_FILENAME
         with metadata_file.open("r") as f:
             metadata = json.load(f)
         job_read.history = metadata["history"]
     except (KeyError, FileNotFoundError):
         pass
 
+    await db.close()
     return job_read
 
 
 @router.get("/download/{job_id}", response_class=StreamingResponse)
 async def download_job_logs(
     job_id: int,
     user: User = Depends(current_active_user),
@@ -81,12 +82,14 @@
     PREFIX_ZIP = working_dir_path.name
     zip_filename = f"{PREFIX_ZIP}_archive.zip"
     byte_stream = BytesIO()
     with ZipFile(byte_stream, mode="w", compression=ZIP_DEFLATED) as zipfile:
         for fpath in working_dir_path.glob("*"):
             zipfile.write(filename=str(fpath), arcname=str(fpath.name))
 
+    await db.close()
+
     return StreamingResponse(
         iter([byte_stream.getvalue()]),
         media_type="application/x-zip-compressed",
         headers={"Content-Disposition": f"attachment;filename={zip_filename}"},
     )
```

### Comparing `fractal_server-1.2.2/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.3a0/fractal_server/app/api/v1/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     stm = (
         select(Project)
         .join(LinkUserProject)
         .where(LinkUserProject.user_id == user.id)
     )
     res = await db.execute(stm)
     project_list = res.scalars().all()
+    await db.close()
     return project_list
 
 
 @router.post("/", response_model=ProjectRead, status_code=201)
 async def create_project(
     project: ProjectCreate,
     user: User = Depends(current_active_user),
@@ -173,14 +174,15 @@
     db_project = Project.from_orm(project)
     db_project.dataset_list.append(Dataset(name=project.default_dataset_name))
     db_project.user_member_list.append(user)
     try:
         db.add(db_project)
         await db.commit()
         await db.refresh(db_project)
+        await db.close()
     except IntegrityError as e:
         await db.rollback()
         logger = set_logger("create_project")
         logger.error(str(e))
         close_logger(logger)
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
@@ -196,26 +198,29 @@
     response_model=ApplyWorkflowRead,
 )
 async def apply_workflow(
     apply_workflow: ApplyWorkflowCreate,
     background_tasks: BackgroundTasks,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-    db_sync: DBSyncSession = Depends(get_sync_db),
+    db_sync: DBSyncSession = Depends(
+        get_sync_db
+    ),  # FIXME: why both sync and async?  # noqa
 ) -> Optional[ApplyWorkflowRead]:
     output = await _get_dataset_check_owner(
         project_id=apply_workflow.project_id,
         dataset_id=apply_workflow.input_dataset_id,
         user_id=user.id,
         db=db,
     )
     input_dataset = output["dataset"]
     project = output["project"]
 
     workflow = db_sync.get(Workflow, apply_workflow.workflow_id)
+    db_sync.close()
     if not workflow:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"Workflow {apply_workflow.workflow_id} not found",
         )
     if workflow.project_id != project.id:
         raise HTTPException(
@@ -286,20 +291,21 @@
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e)
         )
 
     job = ApplyWorkflow.from_orm(apply_workflow)
     db.add(job)
     await db.commit()
     await db.refresh(job)
+    await db.close()
 
     background_tasks.add_task(
         submit_workflow,
-        workflow=workflow,
-        input_dataset=input_dataset,
-        output_dataset=output_dataset,
+        workflow_id=workflow.id,
+        input_dataset_id=input_dataset.id,
+        output_dataset_id=output_dataset.id,
         job_id=job.id,
         worker_init=apply_workflow.worker_init,
         slurm_user=user.slurm_user,
         user_cache_dir=user.cache_dir,
     )
 
     return job
@@ -316,14 +322,15 @@
 ) -> Optional[ProjectRead]:
     """
     Return info on an existing project
     """
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
+    await db.close()
     return project
 
 
 @router.delete("/{project_id}", status_code=204)
 async def delete_project(
     project_id: int,
     user: User = Depends(current_active_user),
@@ -333,14 +340,15 @@
     Delete project
     """
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     await db.delete(project)
     await db.commit()
+    await db.close()
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.post(
     "/{project_id}/",
     response_model=DatasetRead,
     status_code=status.HTTP_201_CREATED,
@@ -357,14 +365,16 @@
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     db_dataset = Dataset(project_id=project_id, **dataset.dict())
     db.add(db_dataset)
     await db.commit()
     await db.refresh(db_dataset)
+    await db.close()
+
     return db_dataset
 
 
 @router.get("/{project_id}/workflows/", response_model=list[WorkflowRead])
 async def get_workflow_list(
     project_id: int,
     user: User = Depends(current_active_user),
@@ -375,14 +385,15 @@
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     stm = select(Workflow).where(Workflow.project_id == project_id)
     res = await db.execute(stm)
     workflow_list = res.scalars().all()
+    await db.close()
     return workflow_list
 
 
 @router.get("/{project_id}/jobs/", response_model=list[ApplyWorkflowRead])
 async def get_job_list(
     project_id: int,
     user: User = Depends(current_active_user),
@@ -393,14 +404,15 @@
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     stm = select(ApplyWorkflow).where(ApplyWorkflow.project_id == project_id)
     res = await db.execute(stm)
     job_list = res.scalars().all()
+
     return job_list
 
 
 @router.patch("/{project_id}", response_model=ProjectRead)
 async def edit_project(
     project_id: int,
     project_update: ProjectUpdate,
@@ -411,14 +423,15 @@
         project_id=project_id, user_id=user.id, db=db
     )
     for key, value in project_update.dict(exclude_unset=True).items():
         setattr(project, key, value)
 
     await db.commit()
     await db.refresh(project)
+    await db.close()
     return project
 
 
 # Dataset endpoints ("/{project_id}/{dataset_id}")
 
 
 @router.get("/{project_id}/{dataset_id}", response_model=DatasetRead)
@@ -431,14 +444,15 @@
     """
     Get info on a dataset associated to the current project
     """
     output = await _get_dataset_check_owner(
         project_id=project_id, dataset_id=dataset_id, user_id=user.id, db=db
     )
     dataset = output["dataset"]
+    await db.close()
     return dataset
 
 
 @router.patch("/{project_id}/{dataset_id}", response_model=DatasetRead)
 async def patch_dataset(
     project_id: int,
     dataset_id: int,
@@ -458,14 +472,15 @@
     db_dataset = output["dataset"]
 
     for key, value in dataset_update.dict(exclude_unset=True).items():
         setattr(db_dataset, key, value)
 
     await db.commit()
     await db.refresh(db_dataset)
+    await db.close()
     return db_dataset
 
 
 @router.delete("/{project_id}/{dataset_id}", status_code=204)
 async def delete_dataset(
     project_id: int,
     dataset_id: int,
@@ -484,14 +499,15 @@
         .where(Project.id == project_id)
         .where(Dataset.id == dataset_id)
     )
     res = await db.execute(stm)
     dataset = res.scalar()
     await db.delete(dataset)
     await db.commit()
+    await db.close()
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.post(
     "/{project_id}/{dataset_id}",
     response_model=ResourceRead,
     status_code=status.HTTP_201_CREATED,
@@ -517,14 +533,15 @@
             detail=f"Dataset {dataset_id} is not part of project {project_id}",
         )
 
     db_resource = Resource(dataset_id=dataset.id, **resource.dict())
     db.add(db_resource)
     await db.commit()
     await db.refresh(db_resource)
+    await db.close()
     return db_resource
 
 
 @router.get(
     "/{project_id}/{dataset_id}/resources/",
     response_model=list[ResourceRead],
 )
@@ -539,14 +556,15 @@
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     stm = select(Resource).where(Resource.dataset_id == dataset_id)
     res = await db.execute(stm)
     resource_list = res.scalars().all()
+    await db.close()
     return resource_list
 
 
 # Resource endpoints ("/{project_id}/{dataset_id}/{resource_id}")
 
 
 @router.delete("/{project_id}/{dataset_id}/{resource_id}", status_code=204)
@@ -569,14 +587,15 @@
     ):
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail="Resource does not exist or does not belong to project",
         )
     await db.delete(resource)
     await db.commit()
+    await db.close()
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.patch(
     "/{project_id}/{dataset_id}/{resource_id}", response_model=ResourceRead
 )
 async def edit_resource(
@@ -610,14 +629,15 @@
             ),
         )
 
     for key, value in resource_update.dict(exclude_unset=True).items():
         setattr(orig_resource, key, value)
     await db.commit()
     await db.refresh(orig_resource)
+    await db.close()
     return orig_resource
 
 
 @router.post(
     "/{project_id}/import-workflow/",
     response_model=WorkflowRead,
     status_code=status.HTTP_201_CREATED,
@@ -711,8 +731,9 @@
             )
             # Insert task
             await db_workflow.insert_task(
                 **new_wf_task.dict(exclude={"workflow_id"}),
                 db=db,
             )
 
+    await db.close()
     return db_workflow
```

### Comparing `fractal_server-1.2.2/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.3a0/fractal_server/app/api/v1/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     """
     Insert tasks into database
     """
     task_db_list = [Task.from_orm(t) for t in task_list]
     db.add_all(task_db_list)
     await db.commit()
     await asyncio.gather(*[db.refresh(t) for t in task_db_list])
+    await db.close()
     return task_db_list
 
 
 @router.post(
     "/collect/pip/",
     response_model=StateRead,
     responses={
@@ -204,25 +205,27 @@
     except FileExistsError:
         venv_path = create_package_dir_pip(
             task_pkg=task_pkg, user=pkg_user, create=False
         )
         try:
             task_collect_status = get_collection_data(venv_path)
         except FileNotFoundError as e:
+            await db.close()
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=(
                     "Cannot collect package. Possible reason: another "
                     "collection of the same package is in progress. "
                     f"Original error: {e}"
                 ),
             )
         task_collect_status.info = "Already installed"
         state = State(data=task_collect_status.sanitised_dict())
         response.status_code == status.HTTP_200_OK
+        await db.close()
         return state
     settings = Inject(get_settings)
 
     full_venv_path = venv_path.relative_to(settings.FRACTAL_TASKS_DIR)
     collection_status = TaskCollectStatus(
         status="pending", venv_path=full_venv_path, package=task_pkg.package
     )
@@ -249,14 +252,15 @@
     close_logger(logger)
     info = (
         "Collecting tasks in the background. "
         f"GET /task/collect/{state.id} to query collection status"
     )
     state.data["info"] = info
     response.status_code = status.HTTP_201_CREATED
+    await db.close()
     return state
 
 
 @router.get("/collect/{state_id}", response_model=StateRead)
 async def check_collection_status(
     state_id: int,
     user: User = Depends(current_active_user),
@@ -266,26 +270,28 @@
     """
     Check status of background task collection
     """
     logger = set_logger(logger_name="check_collection_status")
     logger.debug(f"Querying state for state.id={state_id}")
     state = await db.get(State, state_id)
     if not state:
+        await db.close()
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"No task collection info with id={state_id}",
         )
     data = TaskCollectStatus(**state.data)
 
     # In some cases (i.e. a successful or ongoing task collection), data.log is
     # not set; if so, we collect the current logs
     if verbose and not data.log:
         data.log = get_collection_log(data.venv_path)
         state.data = data.sanitised_dict()
     close_logger(logger)
+    await db.close()
     return state
 
 
 @router.get("/", response_model=list[TaskRead])
 async def get_list_task(
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
@@ -293,27 +299,29 @@
     """
     Get list of available tasks
     """
     stm = select(Task)
     res = await db.execute(stm)
     task_list = res.scalars().unique().fetchall()
     await asyncio.gather(*[db.refresh(t) for t in task_list])
+    await db.close()
     return task_list
 
 
 @router.get("/{task_id}", response_model=TaskRead)
 def get_task(
     task_id: int,
     user: User = Depends(current_active_user),
     db_sync: DBSyncSession = Depends(get_sync_db),
 ) -> TaskRead:
     """
     Get info on a specific task
     """
     task = db_sync.get(Task, task_id)
+    db_sync.close()
     return task
 
 
 @router.patch("/{task_id}", response_model=TaskRead)
 async def patch_task(
     task_id: int,
     task_update: TaskUpdate,
@@ -342,14 +350,15 @@
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=f"Invalid {type(value)=} for {key=}",
             )
 
     await db.commit()
     await db.refresh(db_task)
+    await db.close()
     return db_task
 
 
 @router.post("/", response_model=TaskRead, status_code=status.HTTP_201_CREATED)
 async def create_task(
     task: TaskCreate,
     user: User = Depends(current_active_user),
@@ -365,8 +374,9 @@
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=f"Task with source={task.source} already in use",
         )
     db_task = Task.from_orm(task)
     db.add(db_task)
     await db.commit()
     await db.refresh(db_task)
+    await db.close()
     return db_task
```

### Comparing `fractal_server-1.2.2/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.3a0/fractal_server/app/api/v1/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
         name=workflow.name, project_id=workflow.project_id, db=db
     )
 
     db_workflow = Workflow.from_orm(workflow)
     db.add(db_workflow)
     await db.commit()
     await db.refresh(db_workflow)
+    await db.close()
     return db_workflow
 
 
 # Workflow endpoints ("/{workflow_id}")
 
 
 @router.delete("/{workflow_id}", status_code=status.HTTP_204_NO_CONTENT)
@@ -243,14 +244,15 @@
             for ind_wftask in range(num_tasks):
                 new_order = value.index(workflow.task_list[ind_wftask].id)
                 workflow.task_list[ind_wftask].order = new_order
         else:
             setattr(workflow, key, value)
     await db.commit()
     await db.refresh(workflow)
+    await db.close()
 
     return workflow
 
 
 @router.get("/{workflow_id}", response_model=WorkflowRead)
 async def get_workflow(
     workflow_id: int,
@@ -288,14 +290,15 @@
     )
     async with db:
         workflow_task = await workflow.insert_task(
             **new_task.dict(),
             db=db,
         )
 
+    await db.close()
     return workflow_task
 
 
 # WorkflowTask endpoints ("/{workflow_id}/../{workflow_task_id}"
 
 
 @router.patch(
@@ -333,14 +336,15 @@
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=f"patch_workflow_task endpoint cannot set {key=}",
             )
 
     await db.commit()
     await db.refresh(db_workflow_task)
+    await db.close()
 
     return db_workflow_task
 
 
 @router.delete(
     "/{workflow_id}/rm-task/{workflow_task_id}",
     status_code=status.HTTP_204_NO_CONTENT,
@@ -383,8 +387,9 @@
 ) -> Optional[WorkflowExport]:
     """
     Export an existing workflow, after stripping all IDs
     """
     workflow = await _get_workflow_check_owner(
         workflow_id=workflow_id, user_id=user.id, db=db
     )
+    await db.close()
     return workflow
```

### Comparing `fractal_server-1.2.2/fractal_server/app/db/__init__.py` & `fractal_server-1.2.3a0/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/models/job.py` & `fractal_server-1.2.3a0/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/models/project.py` & `fractal_server-1.2.3a0/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/models/security.py` & `fractal_server-1.2.3a0/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/models/state.py` & `fractal_server-1.2.3a0/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/models/task.py` & `fractal_server-1.2.3a0/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/models/workflow.py` & `fractal_server-1.2.3a0/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,57 +64,66 @@
             ),
         )
     return process_workflow
 
 
 async def submit_workflow(
     *,
-    workflow: Workflow,
-    input_dataset: Dataset,
-    output_dataset: Dataset,
+    workflow_id: int,
+    input_dataset_id: int,
+    output_dataset_id: int,
     job_id: int,
     worker_init: Optional[str] = None,
     slurm_user: Optional[str] = None,
     user_cache_dir: Optional[str] = None,
 ) -> None:
     """
     Prepares a workflow and applies it to a dataset
 
     This function wraps the process_workflow one, which is different for each
     backend (e.g. local or slurm backend).
 
     Args:
-        workflow:
-            Workflow being applied
-        input_dataset:
-            Input dataset
-        output_dataset:
-            the destination dataset of the workflow. If not provided,
+        workflow_id:
+            ID of the workflow being applied
+        input_dataset_id
+            Input dataset ID
+        output_dataset_id:
+            ID of the destination dataset of the workflow. If not provided,
             overwriting of the input dataset is implied and an error is raised
-            if the dataset is in read only mode. If a string is passed and the
-            dataset does not exist, a new dataset with that name is created and
-            within it a new resource with the same name.
+            if the dataset is in read only mode.
         job_id:
             Id of the job record which stores the state for the current
             workflow application.
         worker_init:
             Custom executor parameters that get parsed before the execution of
             each task.
         user_cache_dir:
             Cache directory (namely a path where the user can write); for the
             slurm backend, this is used as a base directory for
             `job.working_dir_user`.
         slurm_user:
             The username to impersonate for the workflow execution, for the
             slurm backend.
     """
+
     db_sync = next(DB.get_sync_db())
-    job: ApplyWorkflow = db_sync.get(ApplyWorkflow, job_id)  # type: ignore
+
+    job: ApplyWorkflow = db_sync.get(ApplyWorkflow, job_id)
     if not job:
         raise ValueError("Cannot fetch job from database")
+    input_dataset: Dataset = db_sync.get(Dataset, input_dataset_id)
+    if not input_dataset:
+        raise ValueError("Cannot fetch input_dataset from database")
+    output_dataset: Dataset = db_sync.get(Dataset, output_dataset_id)
+    if not output_dataset:
+        raise ValueError("Cannot fetch output_dataset from database")
+    workflow: Workflow = db_sync.get(Workflow, workflow_id)
+    if not workflow:
+        raise ValueError("Cannot fetch workflow from database")
 
     # Select backend
     settings = Inject(get_settings)
     FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
     process_workflow = get_process_workflow()
 
     # Prepare some of process_workflow arguments
@@ -174,15 +183,21 @@
     logger.debug(f"input_paths: {input_paths}")
     logger.debug(f"output_path: {output_path}")
     logger.debug(f"job.id: {job.id}")
     logger.debug(f"job.working_dir: {str(WORKFLOW_DIR)}")
     logger.debug(f"job.workflow_dir_user: {str(WORKFLOW_DIR_USER)}")
     logger.debug(f'START workflow "{workflow.name}"')
 
+    # Note: from the docs, "The Session.close() method does not prevent the
+    # Session from being used again"
+    # (https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session.close)
+    db_sync.close()
+
     try:
+
         output_dataset.meta = await process_workflow(
             workflow=workflow,
             input_paths=input_paths,
             output_path=output_path,
             input_metadata=input_dataset.meta,
             slurm_user=slurm_user,
             user_cache_dir=user_cache_dir,
@@ -236,7 +251,8 @@
         job.status = JobStatusType.FAILED
         job.log = f"UNKNOWN ERROR\nOriginal error: {str(e)}"
         db_sync.merge(job)
 
     finally:
         close_job_logger(logger)
         db_sync.commit()
+        db_sync.close()
```

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_common.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/runner/common.py` & `fractal_server-1.2.3a0/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/app/security/__init__.py` & `fractal_server-1.2.3a0/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.3a0/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.3a0/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/README.md` & `fractal_server-1.2.3a0/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.3a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/project.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/state.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/task.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/user.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.3a0/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.3a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.3a0/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/config.py` & `fractal_server-1.2.3a0/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/logger.py` & `fractal_server-1.2.3a0/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/main.py` & `fractal_server-1.2.3a0/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/migrations/env.py` & `fractal_server-1.2.3a0/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.3a0/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.3a0/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.3a0/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.3a0/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/syringe.py` & `fractal_server-1.2.3a0/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/tasks/collection.py` & `fractal_server-1.2.3a0/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/fractal_server/utils.py` & `fractal_server-1.2.3a0/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.2/pyproject.toml` & `fractal_server-1.2.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.2"
+version = "1.2.3a0"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -71,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.2"
+current_version = "1.2.3a0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.2/setup.py` & `fractal_server-1.2.3a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.2',
+    'version': '1.2.3a0',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.2/PKG-INFO` & `fractal_server-1.2.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.2
+Version: 1.2.3a0
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

