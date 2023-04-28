# Comparing `tmp/domino-py-0.1.6.tar.gz` & `tmp/domino-py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.1.6.tar", last modified: Thu Apr 27 21:17:47 2023, max compression
+gzip compressed data, was "domino-py-0.1.7.tar", last modified: Fri Apr 28 13:49:17 2023, max compression
```

## Comparing `domino-py-0.1.6.tar` & `domino-py-0.1.7.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.716592 domino-py-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 21:17:28.000000 domino-py-0.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 21:17:28.000000 domino-py-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-27 21:17:47.716592 domino-py-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-27 21:17:28.000000 domino-py-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.700592 domino-py-0.1.6/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.700592 domino-py-0.1.6/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.700592 domino-py-0.1.6/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/create_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/sidecar_lifecycle.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-airflow/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-airflow/charts/
--rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-airflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-base/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/Chart.lock
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/domino-backend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/domino-frontend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/domino-postgres-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/ingress-api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/ingress-frontend.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-base/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/jobs/domino-migrations.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.712592 domino-py-0.1.6/domino/helm/domino-base/templates/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/piece_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.712592 domino-py-0.1.6/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.712592 domino-py-0.1.6/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/generate_infrasctructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/run_piece_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.716592 domino-py-0.1.6/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/enum_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/types_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.716592 domino-py-0.1.6/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-27 21:17:47.000000 domino-py-0.1.6/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-27 21:17:28.000000 domino-py-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:17:47.716592 domino-py-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-27 21:17:28.000000 domino-py-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.955813 domino-py-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 13:49:03.000000 domino-py-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 13:49:03.000000 domino-py-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 13:49:17.955813 domino-py-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-28 13:49:03.000000 domino-py-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.947813 domino-py-0.1.7/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.947813 domino-py-0.1.7/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.947813 domino-py-0.1.7/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/utils/create_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.947813 domino-py-0.1.7/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.947813 domino-py-0.1.7/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/domino-airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-airflow/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/domino-airflow/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-airflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/domino-base/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/Chart.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/domino-base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/domino-backend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/domino-frontend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/domino-postgres-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/ingress-api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/ingress-frontend.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/domino-base/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/jobs/domino-migrations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/helm/domino-base/templates/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/helm/domino-base/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/piece_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.951813 domino-py-0.1.7/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/generate_infrasctructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/run_piece_dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.955813 domino-py-0.1.7/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/enum_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/types_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 13:49:03.000000 domino-py-0.1.7/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:49:17.955813 domino-py-0.1.7/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 13:49:17.000000 domino-py-0.1.7/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-28 13:49:17.000000 domino-py-0.1.7/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:49:17.000000 domino-py-0.1.7/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 13:49:17.000000 domino-py-0.1.7/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 13:49:17.000000 domino-py-0.1.7/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 13:49:17.000000 domino-py-0.1.7/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-28 13:49:03.000000 domino-py-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:49:17.955813 domino-py-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-28 13:49:03.000000 domino-py-0.1.7/setup.py
```

### Comparing `domino-py-0.1.6/LICENSE.md` & `domino-py-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/MANIFEST.in` & `domino-py-0.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/PKG-INFO` & `domino-py-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

### Comparing `domino-py-0.1.6/README.md` & `domino-py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/base_piece.py` & `domino-py-0.1.7/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/cli/cli.py` & `domino-py-0.1.7/domino/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 def get_github_token_pieces_from_env():
     return os.environ.get("DOMINO_GITHUB_ACCESS_TOKEN_PIECES", None)
 
 def get_github_token_workflows_from_env():
     return os.environ.get("DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS", None)
 
 def get_workflows_repository_from_env():
-    return os.environ.get("DOMINO_WORKFLOWS_REPOSITORY", None)
+    return os.environ.get("DOMINO_GITHUB_WORKFLOWS_REPOSITORY", None)
 
 def get_local_operators_repository_path():
     return ""
 
 def get_registry_token_from_env():
     return os.environ.get('GHCR_PASSWORD', "")
 
@@ -114,26 +114,26 @@
 )
 def cli_prepare_platform(
     cluster_name,
     workflows_repository,
     github_workflows_ssh_private_key,
     github_pieces_token,
     github_workflows_token,
-    dev_mode,
+    deploy_mode,
     local_pieces_repository_path,
     local_domino_path
 ):
     """Prepare local folder for running a Domino platform."""
     platform.prepare_platform(
         cluster_name=cluster_name, 
         workflows_repository=workflows_repository,
         github_workflows_ssh_private_key=github_workflows_ssh_private_key, 
         github_pieces_token=github_pieces_token,
         github_workflows_token=github_workflows_token,
-        dev_mode=dev_mode,
+        deploy_mode=deploy_mode,
         local_pieces_repository_path=ast.literal_eval(local_pieces_repository_path),
         local_domino_path=local_domino_path
     )
 
 
 @click.command()
 @click.option(
```

### Comparing `domino-py-0.1.6/domino/cli/utils/config-domino-local.toml` & `domino-py-0.1.7/domino/cli/utils/config-domino-local.toml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/cli/utils/create_cluster.sh` & `domino-py-0.1.7/domino/cli/utils/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/cli/utils/pieces_repository.py` & `domino-py-0.1.7/domino/cli/utils/pieces_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 CONFIG_REQUIRED_FIELDS = {}
 
 
 def validate_github_token(token: str) -> bool:
     """
-    Validate GITHUB_ACCESS_TOKEN
+    Validate DOMINO_GITHUB_ACCESS_TOKEN
     By now it is only accepting the ghp token.
 
     Args:
         token (str): Github access token (ghp)
 
     Returns:
         bool: True if token is valid, False otherwise.
@@ -45,19 +45,19 @@
     pattern = re.compile(regex)
     if pattern.match(token):
         return True
     return False
 
 
 REQUIRED_ENV_VARS_VALIDATORS = {
-    "GITHUB_ACCESS_TOKEN_OPERATORS": {
+    "DOMINO_GITHUB_ACCESS_TOKEN_PIECES": {
         "depends": lambda arg: arg.get('OPERATORS_REPOSITORY_SOURCE') == 'github',
         "validator_func": validate_github_token
     },
-    "GITHUB_ACCESS_TOKEN_WORKFLOWS": {
+    "DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS": {
         "depends": lambda arg: arg.get('OPERATORS_REPOSITORY_SOURCE') == 'github',
         "validator_func": validate_github_token
     }
 }
 
 
 def set_config_as_env(key: str, value: Union[str, int, float]) -> None:
```

### Comparing `domino-py-0.1.6/domino/cli/utils/platform.py` & `domino-py-0.1.7/domino/cli/utils/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,31 +52,31 @@
 
 def prepare_platform(
     cluster_name: str, 
     workflows_repository: str, 
     github_workflows_ssh_private_key: str, 
     github_pieces_token: str, 
     github_workflows_token: str,
-    dev_mode: str,
+    deploy_mode: str,
     local_pieces_repository_path: list,
     local_domino_path: str
 ) -> None:
     # Create local configuration file updated with user-provided arguments
     config_file_path = Path(__file__).resolve().parent / "config-domino-local.toml"
     with open(str(config_file_path), "rb") as f:
         config_dict = tomli.load(f)
     
     running_path = str(Path().cwd().resolve())
     config_dict["path"]["DOMINO_LOCAL_RUNNING_PATH"] = running_path
     config_dict["kind"]["DOMINO_KIND_CLUSTER_NAME"] = cluster_name
-    config_dict['kind']['dev_mode'] = dev_mode
+    config_dict['kind']['DOMINO_DEPLOY_MODE'] = deploy_mode
 
     config_dict['local_pieces_repositories'] = {}
     config_dict['local_domino_repository'] = {"DOMINO_LOCAL_DOMINO_REPOSITORY": ""}
-    if dev_mode == 'local':
+    if deploy_mode == 'local-k8s-dev':
         config_dict['local_domino_repository']['DOMINO_LOCAL_DOMINO_REPOSITORY'] = local_domino_path
         for local_pieces_repository in local_pieces_repository_path:
             # Read repo config.toml to get repo name to map it to cluster path
             repo_config_file_path = Path(local_pieces_repository).resolve() / "config.toml"
             with open(str(repo_config_file_path), "rb") as f:
                 repo_toml = tomli.load(f)
             
@@ -116,15 +116,15 @@
         nodeRegistration=dict(
             kubeletExtraArgs={
                 "node-labels": "ingress-ready=true"
             }
         )
     )
     extra_mounts_local_repositories = []
-    if platform_config['kind']['dev_mode'] == 'local':
+    if platform_config['kind']['DOMINO_DEPLOY_MODE'] == 'local-k8s-dev':
         for repo_name, repo_path in platform_config['local_pieces_repositories'].items():
             extra_mounts_local_repositories.append(
                 dict(
                     hostPath=repo_path,
                     containerPath=f"/pieces_repositories/{repo_name}",
                     readOnly=True,
                     propagation='HostToContainer'
@@ -268,15 +268,15 @@
     )
     airflow_ssh_config_parsed = AsLiteral(yaml.dump(airflow_ssh_config))
 
     workers_extra_volumes = []
     workers_extra_volumes_mounts = []
     workers = {}
     scheduler = {}
-    if platform_config['kind']["dev_mode"] == 'local' and platform_config['local_domino_repository'].get('DOMINO_LOCAL_DOMINO_REPOSITORY'):
+    if platform_config['kind']["DOMINO_DEPLOY_MODE"] == 'local-k8s-dev' and platform_config['local_domino_repository'].get('DOMINO_LOCAL_DOMINO_REPOSITORY'):
         workers_extra_volumes = [
             {
                 "name": "domino-dev-extra",
                 "persistentVolumeClaim": {
                     "claimName": "domino-dev-volume-claim"
                 }
             }
@@ -301,16 +301,16 @@
         }
 
     airflow_values_override_config = {
         "airflow": {
             "enabled": True,
             "env": [
                 {
-                    "name": "DOMINO_DEV_MODE",
-                    "value": platform_config['kind']["dev_mode"]
+                    "name": "DOMINO_DEPLOY_MODE",
+                    "value": platform_config['kind']["DOMINO_DEPLOY_MODE"]
                 },
             ],
             "images": {
                 "useDefaultImageForMigration": False,
                 "airflow": {
                     "repository": "ghcr.io/tauffer-consulting/domino-airflow-base", # TODO change to prod # TODO change to domino image name when we have it
                     "tag": "latest",
@@ -350,15 +350,15 @@
             "helm", "upgrade",
             "-i", "-f", str(fp.name),
             "domino-airflow",
             domino_airlflow_helm_path,
         ])
 
     # For each path create a pv and pvc
-    if platform_config['kind']['dev_mode'] == 'local':
+    if platform_config['kind']['DOMINO_DEPLOY_MODE'] == 'local-k8s-dev':
         config.load_kube_config()
         k8s_client = client.CoreV1Api()
         v1 = client.RbacAuthorizationV1Api()
 
         # Create service account role binding with admin access for airflow worker
         role_binding_name_worker = "full-access-user-clusterrolebinding-worker"
         sa_name = "domino-airflow-worker"
```

### Comparing `domino-py-0.1.6/domino/client/airflow_client.py` & `domino-py-0.1.7/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/client/domino_backend_client.py` & `domino-py-0.1.7/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/client/fs_client.py` & `domino-py-0.1.7/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/client/github_rest_client.py` & `domino-py-0.1.7/domino/client/github_rest_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from github import Github
 import os
 
 
 class GithubRestClient(Github):
-    def __init__(self, token: str = None):
-        if not token:
-            token = os.getenv("GITHUB_ACCESS_TOKEN")
+    def __init__(self, token: str):
         super().__init__(token)
 
     def get_releases(self, repo_name: str):
         """
         Get all releases from a repository.
         """
         repo = super().get_repo(repo_name)
```

### Comparing `domino-py-0.1.6/domino/client/local_files_client.py` & `domino-py-0.1.7/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/client/s3_client.py` & `domino-py-0.1.7/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/custom_operators/bash_operator.py` & `domino-py-0.1.7/domino/custom_operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/custom_operators/k8s_operator.py` & `domino-py-0.1.7/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/custom_operators/python_operator.py` & `domino-py-0.1.7/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/custom_operators/sidecar/logger.py` & `domino-py-0.1.7/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/custom_operators/sidecar/mount.py` & `domino-py-0.1.7/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/exceptions/exceptions.py` & `domino-py-0.1.7/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz` & `domino-py-0.1.7/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/helm/domino-airflow/values.yaml` & `domino-py-0.1.7/domino/helm/domino-airflow/values.yaml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/helm/domino-base/templates/domino-backend-deployment.yml` & `domino-py-0.1.7/domino/helm/domino-base/templates/domino-backend-deployment.yml`

 * *Files 6% similar despite different names*

```diff
@@ -28,37 +28,37 @@
           ports:
             - containerPort: 8000
           imagePullPolicy: IfNotPresent
           env: 
             # TODO use load balancer instead of service ip for airflow webserver ?
             - name: AIRFLOW_WEBSERVER_HOST
               value: http://{{ .Release.Name }}-airflow-webserver:8080
-            - name: FLOWUI_DEPLOY_MODE
-              value: dev # TODO change to prod
-            - name: DB_HOST
+            - name: DOMINO_DEPLOY_MODE
+              value: local-k8s-dev # TODO change to prod
+            - name: DOMINO_DB_HOST
               value: {{ .Release.Name }}-postgres-service
-            - name: DB_NAME
+            - name: DOMINO_DB_NAME
               value: {{ .Values.database.name }}
-            - name: DB_USER
+            - name: DOMINO_DB_USER
               value: {{ .Values.database.user }}
-            - name: DB_PASSWORD
+            - name: DOMINO_DB_PASSWORD
               value: {{ .Values.database.password }}
-            - name: DB_PORT
+            - name: DOMINO_DB_PORT
               value: "5432"
-            - name: "GITHUB_ACCESS_TOKEN_PIECES"
+            - name: "DOMINO_GITHUB_ACCESS_TOKEN_PIECES"
               valueFrom:
                 secretKeyRef:
                   key:  github_access_token_pieces
                   name: {{ .Release.Name }}-secrets
-            - name: "GITHUB_ACCESS_TOKEN_WORKFLOWS"
+            - name: "DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS"
               valueFrom:
                 secretKeyRef:
                   key:  github_access_token_workflows
                   name: {{ .Release.Name }}-secrets
-            - name: FLOWUI_WORKFLOWS_REPOSITORY
+            - name: DOMINO_GITHUB_WORKFLOWS_REPOSITORY
               value: {{ .Values.backend.workflowsRepository }}
           {{- if .Values.backend.extraVolumeMounts }}
           volumeMounts:             
 {{ toYaml .Values.backend.extraVolumeMounts | indent 12 }}
           {{- end }}
           # volumeMounts:
           #   - name: my-pods-persistent-storage
```

### Comparing `domino-py-0.1.6/domino/helm/domino-base/templates/domino-frontend-deployment.yml` & `domino-py-0.1.7/domino/helm/domino-base/templates/domino-frontend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/helm/domino-base/templates/domino-postgres-deployment.yml` & `domino-py-0.1.7/domino/helm/domino-base/templates/domino-postgres-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/helm/domino-base/templates/jobs/domino-migrations.yml` & `domino-py-0.1.7/domino/helm/domino-base/templates/jobs/domino-migrations.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,18 @@
       restartPolicy: OnFailure
       containers:
       - name: database-migrations
         image: {{ .Values.backend.image }}
         command: ["/bin/bash"]
         args: ["run_migrations.sh"]   # will sleep for 20 seconds, run migrations and create first user
         env:
-          - name: DB_HOST
+          - name: DOMINO_DB_HOST
             value: {{ .Release.Name }}-postgres-service
-          - name: DB_NAME
+          - name: DOMINO_DB_NAME
             value: {{ .Values.database.name }}
-          - name: DB_USER
+          - name: DOMINO_DB_USER
             value: {{ .Values.database.user }}
-          - name: DB_PASSWORD
+          - name: DOMINO_DB_PASSWORD
             value: {{ .Values.database.password }}
-          - name: DB_PORT
+          - name: DOMINO_DB_PORT
             value: "5432"
```

### Comparing `domino-py-0.1.6/domino/logger.py` & `domino-py-0.1.7/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/schemas/piece_metadata.py` & `domino-py-0.1.7/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/schemas/shared_storage.py` & `domino-py-0.1.7/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.1.7/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/create_docker_compose_file.py` & `domino-py-0.1.7/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/docker_compose_constants.py` & `domino-py-0.1.7/domino/scripts/docker_compose_constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,23 +300,23 @@
     "image": "taufferconsulting/flowui-backend:latest",
     "container_name": "flowui-backend",
     "command": 'bash -c "alembic upgrade heads && uvicorn main:app --reload --workers 1 --host 0.0.0.0 --port 8000"',
     "ports": [
         "8000:8000"
     ],
     "environment": [
-        "DB_USER=postgres",
-        "DB_PASSWORD=postgres",
-        "DB_HOST=flowui-postgres",
-        "DB_PORT=5432",
-        "DB_NAME=postgres",
-        "CODE_REPOSITORY_SOURCE=${CODE_REPOSITORY_SOURCE}",
-        "GITHUB_ACCESS_TOKEN=${GITHUB_ACCESS_TOKEN}",
-        "GITHUB_REPOSITORY_NAME=${GITHUB_REPOSITORY_NAME}",
-        "FLOWUI_DEPLOY_MODE=${FLOWUI_DEPLOY_MODE}"
+        "DOMINO_DB_USER=postgres",
+        "DOMINO_DB_PASSWORD=postgres",
+        "DOMINO_DB_HOST=flowui-postgres",
+        "DOMINO_DB_PORT=5432",
+        "DOMINO_DB_NAME=postgres",
+        "DOMINO_GITHUB_ACCESS_TOKEN_PIECES=${DOMINO_GITHUB_ACCESS_TOKEN_PIECES}",
+        "DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS=${DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS}",
+        "DOMINO_GITHUB_WORKFLOWS_REPOSITORY=${DOMINO_GITHUB_WORKFLOWS_REPOSITORY}",
+        "DOMINO_DEPLOY_MODE=${DOMINO_DEPLOY_MODE}"
     ],
     "networks": [
         "flowui-postgres-network"
     ],
     "volumes": airflow_common_volumes,
     "depends_on": {
         "flowui-postgres": {
@@ -333,23 +333,23 @@
     },
     "container_name": "flowui-backend-dev",
     "command": 'bash -c "alembic upgrade heads && uvicorn main:app --reload --workers 1 --host 0.0.0.0 --port 8000"',
     "ports": [
         "8000:8000"
     ],
     "environment": [
-        "DB_USER=postgres",
-        "DB_PASSWORD=postgres",
-        "DB_HOST=flowui-postgres",
-        "DB_PORT=5432",
-        "DB_NAME=postgres",
-        "CODE_REPOSITORY_SOURCE=${CODE_REPOSITORY_SOURCE}",
-        "GITHUB_ACCESS_TOKEN=${GITHUB_ACCESS_TOKEN}",
-        "GITHUB_REPOSITORY_NAME=${GITHUB_REPOSITORY_NAME}",
-        "FLOWUI_DEPLOY_MODE=${FLOWUI_DEPLOY_MODE}"
+        "DOMINO_DB_USER=postgres",
+        "DOMINO_DB_PASSWORD=postgres",
+        "DOMINO_DB_HOST=flowui-postgres",
+        "DOMINO_DB_PORT=5432",
+        "DOMINO_DB_NAME=postgres",
+        "DOMINO_GITHUB_ACCESS_TOKEN_PIECES=${DOMINO_GITHUB_ACCESS_TOKEN_PIECES}",
+        "DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS=${DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS}",
+        "DOMINO_GITHUB_WORKFLOWS_REPOSITORY=${DOMINO_GITHUB_WORKFLOWS_REPOSITORY}",
+        "DOMINO_DEPLOY_MODE=${DOMINO_DEPLOY_MODE}"
     ],
     "networks": [
         "flowui-postgres-network"
     ],
     "volumes": airflow_common_volumes_dev + [f"{flowui_path_host}/backend:/backend"],
     "depends_on": {
         "flowui-postgres": {
```

### Comparing `domino-py-0.1.6/domino/scripts/docker_compose_scripts.py` & `domino-py-0.1.7/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/generate_infrasctructure.py` & `domino-py-0.1.7/domino/scripts/generate_infrasctructure.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/load_piece.py` & `domino-py-0.1.7/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/run_piece_bash.py` & `domino-py-0.1.7/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/run_piece_dry.py` & `domino-py-0.1.7/domino/scripts/run_piece_dry.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/scripts/run_piece_k8s.py` & `domino-py-0.1.7/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino/task.py` & `domino-py-0.1.7/domino/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self, 
         dag: DAG, 
         task_id: str,
         piece: dict,
         piece_input_kwargs: dict,
         workflow_shared_storage: dict = None,
         container_resources: dict = None,
-        deploy_mode: str = 'k8s',
+        deploy_mode: str = 'local-k8s-dev',
     ) -> None:
         # Task configuration and attributes
         self.task_id = task_id
         self.logger = get_configured_logger(f"{self.__class__.__name__ }-{self.task_id}")
         self.logger.info('### Configuring task object ###')
         self.dag = dag
         self.dag_id = self.dag.dag_id
@@ -104,15 +104,15 @@
 
         # References: 
         # - https://airflow.apache.org/docs/apache-airflow/1.10.14/_api/airflow/contrib/operators/kubernetes_pod_operator/index.html
         # - https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html
         # - https://www.astronomer.io/guides/templating/
         # - good example: https://github.com/apache/airflow/blob/main/tests/system/providers/cncf/kubernetes/example_kubernetes.py
         # - commands HAVE to go in a list object: https://stackoverflow.com/a/55149915/11483674
-        elif self.deploy_mode == "k8s":
+        elif self.deploy_mode in ["local-k8s", "local-k8s-dev", "prod"]:
             container_env_vars = {
                 "DOMINO_K8S_PIECE": self.piece["name"],
                 "DOMINO_K8S_INSTANTIATE_PIECE_KWARGS": str({
                     "deploy_mode": self.deploy_mode,
                     "task_id": self.task_id,
                     "dag_id": self.dag_id,
                 }),
@@ -140,16 +140,16 @@
             #self.container_resources = ContainerResourcesModel(**self.container_resources)
             container_resources_obj = k8s.V1ResourceRequirements(**basic_container_resources)
 
             # Volumes
             all_volumes = []
             all_volume_mounts = []
 
-            ######################## For local DOMINO_DEV_MODE Operators dev ###########################################
-            if os.environ.get('DOMINO_DEV_MODE') == 'local':
+            ######################## For local DOMINO_DEPLOY_MODE Operators dev ###########################################
+            if os.environ.get('DOMINO_DEPLOY_MODE') == 'local-k8s-dev':
                 source_image = self.piece.get('source_image')
                 repository_raw_project_name = str(source_image).split('/')[1].split(':')[0]
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
 
                 persistent_volume_name = 'pv-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
```

### Comparing `domino-py-0.1.6/domino/utils/validators.py` & `domino-py-0.1.7/domino/utils/validators.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/domino_py.egg-info/PKG-INFO` & `domino-py-0.1.7/domino_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

### Comparing `domino-py-0.1.6/domino_py.egg-info/SOURCES.txt` & `domino-py-0.1.7/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.6/setup.py` & `domino-py-0.1.7/setup.py`

 * *Files identical despite different names*

