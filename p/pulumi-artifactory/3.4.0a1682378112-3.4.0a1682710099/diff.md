# Comparing `tmp/pulumi_artifactory-3.4.0a1682378112.tar.gz` & `tmp/pulumi_artifactory-3.4.0a1682710099.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_artifactory-3.4.0a1682378112.tar", last modified: Mon Apr 24 23:25:19 2023, max compression
+gzip compressed data, was "pulumi_artifactory-3.4.0a1682710099.tar", last modified: Fri Apr 28 19:33:28 2023, max compression
```

## Comparing `pulumi_artifactory-3.4.0a1682378112.tar` & `pulumi_artifactory-3.4.0a1682710099.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:25:19.624644 pulumi_artifactory-3.4.0a1682378112/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-24 23:25:19.624644 pulumi_artifactory-3.4.0a1682378112/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:25:19.620644 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/
--rw-r--r--   0 runner    (1001) docker     (123)    45570 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    26856 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    54037 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/anonymous_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/artifact_property_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/artifact_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/artifactory_release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/build_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:25:19.624644 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/distribution_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/docker_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/general_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_terraformbackend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    29823 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/ldap_group_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/ldap_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_repository_multi_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_repository_single_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_terraform_backend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/managed_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/oauth_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/permission_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/property_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/pull_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/push_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_repository_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/repository_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/saml_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/scoped_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/single_replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25359 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/unmanaged_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    27006 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44685 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_terraform_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:25:19.624644 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:25:19.624644 pulumi_artifactory-3.4.0a1682378112/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-24 23:25:19.000000 pulumi_artifactory-3.4.0a1682378112/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:28.866222 pulumi_artifactory-3.4.0a1682710099/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 19:33:28.866222 pulumi_artifactory-3.4.0a1682710099/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:28.862223 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (123)    45570 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26856 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54037 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/anonymous_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/artifact_property_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/artifact_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/artifactory_release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/build_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:28.866222 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/distribution_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/docker_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/general_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_terraformbackend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29850 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/ldap_group_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/ldap_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_repository_multi_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_repository_single_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_terraform_backend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24136 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/managed_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/oauth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18740 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/permission_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/pull_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/push_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_repository_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24828 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/repository_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/saml_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35645 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/scoped_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/single_replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/unmanaged_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27110 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44685 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_terraform_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:28.866222 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:33:28.866222 pulumi_artifactory-3.4.0a1682710099/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-28 19:33:28.000000 pulumi_artifactory-3.4.0a1682710099/setup.py
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/PKG-INFO` & `pulumi_artifactory-3.4.0a1682710099/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_artifactory
-Version: 3.4.0a1682378112
+Version: 3.4.0a1682710099
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/README.md` & `pulumi_artifactory-3.4.0a1682710099/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/__init__.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/_inputs.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/_utilities.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/access_token.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/anonymous_user.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/api_key.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/artifact_property_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/artifact_property_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/artifact_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/artifact_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/artifactory_release_bundle_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/artifactory_release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/backup.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/build_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/build_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/certificate.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/config/vars.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/distribution_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/distribution_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/docker_v1_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/docker_v2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/docker_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/docker_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_cargo_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_cocoapods_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_docker_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_docker_v1_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_docker_v2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_gitltfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_opkg_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_terraform_module_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_terraform_provider_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/federated_vagrant_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/general_security.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/general_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_cargo_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_cocoapods_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_docker_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_docker_v1_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_docker_v2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_gitlfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_opkg_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_terraform_module_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_terraform_provider_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_federated_vagrant_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_file.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_fileinfo.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_fileinfo.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_group.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_cargo_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_cocoapods_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_docker_v1_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_docker_v2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_gitlfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_opkg_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_pub_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_terraform_module_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_terraform_provider_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_terraformbackend_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_terraformbackend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_local_vagrant_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_permission_target.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_cargo_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_cocoapods_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_docker_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_gitlfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_opkg_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_p2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_pub_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_terraform_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_remote_vcs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_user.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_docker_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_gitlfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_p2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_pub_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/get_virtual_terraform_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/get_virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/group.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,66 +10,77 @@
 from . import _utilities
 
 __all__ = ['GroupArgs', 'Group']
 
 @pulumi.input_type
 class GroupArgs:
     def __init__(__self__, *,
+                 name: pulumi.Input[str],
                  admin_privileges: Optional[pulumi.Input[bool]] = None,
                  auto_join: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  detach_all_users: Optional[pulumi.Input[bool]] = None,
                  external_id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  policy_manager: Optional[pulumi.Input[bool]] = None,
                  realm: Optional[pulumi.Input[str]] = None,
                  realm_attributes: Optional[pulumi.Input[str]] = None,
                  reports_manager: Optional[pulumi.Input[bool]] = None,
                  users_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  watch_manager: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Group resource.
+        :param pulumi.Input[str] name: Name of the group
         :param pulumi.Input[bool] admin_privileges: Any users added to this group will automatically be assigned with admin privileges in the system.
         :param pulumi.Input[bool] auto_join: When this parameter is set, any new users defined in the system are automatically assigned to this group.
         :param pulumi.Input[str] description: A description for the group
         :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group
         :param pulumi.Input[str] external_id: New external group ID used to configure the corresponding group in Azure AD.
-        :param pulumi.Input[str] name: Name of the group
         :param pulumi.Input[bool] policy_manager: When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         :param pulumi.Input[str] realm: The realm for the group.
         :param pulumi.Input[str] realm_attributes: The realm attributes for the group.
         :param pulumi.Input[bool] reports_manager: When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
         :param pulumi.Input[bool] watch_manager: When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
+        pulumi.set(__self__, "name", name)
         if admin_privileges is not None:
             pulumi.set(__self__, "admin_privileges", admin_privileges)
         if auto_join is not None:
             pulumi.set(__self__, "auto_join", auto_join)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if detach_all_users is not None:
             pulumi.set(__self__, "detach_all_users", detach_all_users)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if policy_manager is not None:
             pulumi.set(__self__, "policy_manager", policy_manager)
         if realm is not None:
             pulumi.set(__self__, "realm", realm)
         if realm_attributes is not None:
             pulumi.set(__self__, "realm_attributes", realm_attributes)
         if reports_manager is not None:
             pulumi.set(__self__, "reports_manager", reports_manager)
         if users_names is not None:
             pulumi.set(__self__, "users_names", users_names)
         if watch_manager is not None:
             pulumi.set(__self__, "watch_manager", watch_manager)
 
     @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Name of the group
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="adminPrivileges")
     def admin_privileges(self) -> Optional[pulumi.Input[bool]]:
         """
         Any users added to this group will automatically be assigned with admin privileges in the system.
         """
         return pulumi.get(self, "admin_privileges")
 
@@ -122,26 +133,14 @@
         return pulumi.get(self, "external_id")
 
     @external_id.setter
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the group
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
     @pulumi.getter(name="policyManager")
     def policy_manager(self) -> Optional[pulumi.Input[bool]]:
         """
         When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         """
         return pulumi.get(self, "policy_manager")
 
@@ -444,15 +443,15 @@
         :param pulumi.Input[bool] reports_manager: When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
         :param pulumi.Input[bool] watch_manager: When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[GroupArgs] = None,
+                 args: GroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
         Groups can be imported using their name, e.g.
 
         ```sh
@@ -496,14 +495,16 @@
             __props__ = GroupArgs.__new__(GroupArgs)
 
             __props__.__dict__["admin_privileges"] = admin_privileges
             __props__.__dict__["auto_join"] = auto_join
             __props__.__dict__["description"] = description
             __props__.__dict__["detach_all_users"] = detach_all_users
             __props__.__dict__["external_id"] = external_id
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["policy_manager"] = policy_manager
             __props__.__dict__["realm"] = realm
             __props__.__dict__["realm_attributes"] = realm_attributes
             __props__.__dict__["reports_manager"] = reports_manager
             __props__.__dict__["users_names"] = users_names
             __props__.__dict__["watch_manager"] = watch_manager
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/keypair.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/ldap_group_setting.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/ldap_group_setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,43 +15,42 @@
 class LdapGroupSettingArgs:
     def __init__(__self__, *,
                  description_attribute: pulumi.Input[str],
                  filter: pulumi.Input[str],
                  group_member_attribute: pulumi.Input[str],
                  group_name_attribute: pulumi.Input[str],
                  ldap_setting_key: pulumi.Input[str],
+                 name: pulumi.Input[str],
                  strategy: pulumi.Input[str],
                  group_base_dn: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  sub_tree: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a LdapGroupSetting resource.
         :param pulumi.Input[str] description_attribute: An attribute on the group entry which denoting the group description. Used when importing groups.
         :param pulumi.Input[str] filter: The LDAP filter used to search for group entries. Used for importing groups.
         :param pulumi.Input[str] group_member_attribute: A multi-value attribute on the group entry containing user DNs or IDs of the group members (e.g., uniqueMember,member).
         :param pulumi.Input[str] group_name_attribute: Attribute on the group entry denoting the group name. Used when importing groups.
         :param pulumi.Input[str] ldap_setting_key: The LDAP setting key you want to use for group retrieval. The value for this field corresponds to 'enabledLdap' field of the ldap group setting XML block of system configuration.
+        :param pulumi.Input[str] name: Ldap group setting name.
         :param pulumi.Input[str] strategy: The JFrog Platform Deployment (JPD) supports three ways of mapping groups to LDAP schemas:
                - STATIC: Group objects are aware of their members, however, the users are not aware of the groups they belong to. Each group object such as groupOfNames or groupOfUniqueNames holds its respective member attributes, typically member or uniqueMember, which is a user DN.
                - DYNAMIC: User objects are aware of what groups they belong to, but the group objects are not aware of their members. Each user object contains a custom attribute, such as group, that holds the group DNs or group names of which the user is a member.
                - HIERARCHICAL: The user's DN is indicative of the groups the user belongs to by using group names as part of user DN hierarchy. Each user DN contains a list of ou's or custom attributes that make up the group association. For example, uid=user1,ou=developers,ou=uk,dc=jfrog,dc=org indicates that user1 belongs to two groups: uk and developers.
         :param pulumi.Input[str] group_base_dn: A search base for group entry DNs, relative to the DN on the LDAP server’s URL (and not relative to the LDAP Setting’s “Search Base”). Used when importing groups.
-        :param pulumi.Input[str] name: Ldap group setting name.
         :param pulumi.Input[bool] sub_tree: When set, enables deep search through the sub-tree of the LDAP URL + Search Base. True by default.
         """
         pulumi.set(__self__, "description_attribute", description_attribute)
         pulumi.set(__self__, "filter", filter)
         pulumi.set(__self__, "group_member_attribute", group_member_attribute)
         pulumi.set(__self__, "group_name_attribute", group_name_attribute)
         pulumi.set(__self__, "ldap_setting_key", ldap_setting_key)
+        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "strategy", strategy)
         if group_base_dn is not None:
             pulumi.set(__self__, "group_base_dn", group_base_dn)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if sub_tree is not None:
             pulumi.set(__self__, "sub_tree", sub_tree)
 
     @property
     @pulumi.getter(name="descriptionAttribute")
     def description_attribute(self) -> pulumi.Input[str]:
         """
@@ -109,14 +108,26 @@
 
     @ldap_setting_key.setter
     def ldap_setting_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "ldap_setting_key", value)
 
     @property
     @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Ldap group setting name.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def strategy(self) -> pulumi.Input[str]:
         """
         The JFrog Platform Deployment (JPD) supports three ways of mapping groups to LDAP schemas:
         - STATIC: Group objects are aware of their members, however, the users are not aware of the groups they belong to. Each group object such as groupOfNames or groupOfUniqueNames holds its respective member attributes, typically member or uniqueMember, which is a user DN.
         - DYNAMIC: User objects are aware of what groups they belong to, but the group objects are not aware of their members. Each user object contains a custom attribute, such as group, that holds the group DNs or group names of which the user is a member.
         - HIERARCHICAL: The user's DN is indicative of the groups the user belongs to by using group names as part of user DN hierarchy. Each user DN contains a list of ou's or custom attributes that make up the group association. For example, uid=user1,ou=developers,ou=uk,dc=jfrog,dc=org indicates that user1 belongs to two groups: uk and developers.
         """
@@ -135,26 +146,14 @@
         return pulumi.get(self, "group_base_dn")
 
     @group_base_dn.setter
     def group_base_dn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_base_dn", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Ldap group setting name.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
     @pulumi.getter(name="subTree")
     def sub_tree(self) -> Optional[pulumi.Input[bool]]:
         """
         When set, enables deep search through the sub-tree of the LDAP URL + Search Base. True by default.
         """
         return pulumi.get(self, "sub_tree")
 
@@ -354,14 +353,15 @@
         ldap_group_name = artifactory.LdapGroupSetting("ldapGroupName",
             description_attribute="description",
             filter="(objectClass=groupOfNames)",
             group_base_dn="",
             group_member_attribute="uniqueMember",
             group_name_attribute="cn",
             ldap_setting_key="ldap_name",
+            name="ldap_group_name",
             strategy="STATIC",
             sub_tree=True)
         ```
         Note: `Name` argument has to match to the resource name.\\
         Reference Link: [JFrog LDAP](https://www.jfrog.com/confluence/display/JFROG/LDAP)
 
         ## Import
@@ -411,14 +411,15 @@
         ldap_group_name = artifactory.LdapGroupSetting("ldapGroupName",
             description_attribute="description",
             filter="(objectClass=groupOfNames)",
             group_base_dn="",
             group_member_attribute="uniqueMember",
             group_name_attribute="cn",
             ldap_setting_key="ldap_name",
+            name="ldap_group_name",
             strategy="STATIC",
             sub_tree=True)
         ```
         Note: `Name` argument has to match to the resource name.\\
         Reference Link: [JFrog LDAP](https://www.jfrog.com/confluence/display/JFROG/LDAP)
 
         ## Import
@@ -474,14 +475,16 @@
             __props__.__dict__["group_member_attribute"] = group_member_attribute
             if group_name_attribute is None and not opts.urn:
                 raise TypeError("Missing required property 'group_name_attribute'")
             __props__.__dict__["group_name_attribute"] = group_name_attribute
             if ldap_setting_key is None and not opts.urn:
                 raise TypeError("Missing required property 'ldap_setting_key'")
             __props__.__dict__["ldap_setting_key"] = ldap_setting_key
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if strategy is None and not opts.urn:
                 raise TypeError("Missing required property 'strategy'")
             __props__.__dict__["strategy"] = strategy
             __props__.__dict__["sub_tree"] = sub_tree
         super(LdapGroupSetting, __self__).__init__(
             'artifactory:index/ldapGroupSetting:LdapGroupSetting',
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/ldap_setting.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/ldap_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_cargo_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_cocoapods_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_gitltfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_opkg_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_pub_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_repository_multi_replication.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_repository_multi_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_repository_single_replication.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_repository_single_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_terraform_backend_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_terraform_backend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_terraform_module_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_terraform_provider_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/local_vagrant_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/managed_user.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/managed_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,44 +11,43 @@
 
 __all__ = ['ManagedUserArgs', 'ManagedUser']
 
 @pulumi.input_type
 class ManagedUserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
+                 name: pulumi.Input[str],
                  password: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ManagedUser resource.
         :param pulumi.Input[str] email: Email for user.
+        :param pulumi.Input[str] name: Username for user.
         :param pulumi.Input[str] password: Password for the user.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
-        :param pulumi.Input[str] name: Username for user.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
         """
@@ -58,14 +57,26 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Username for user.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def password(self) -> pulumi.Input[str]:
         """
         Password for the user.
         """
         return pulumi.get(self, "password")
 
     @password.setter
@@ -117,26 +128,14 @@
         return pulumi.get(self, "internal_password_disabled")
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Username for user.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
         When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         return pulumi.get(self, "profile_updatable")
 
@@ -305,14 +304,15 @@
         # Create a new Artifactory user called terraform
         test_user = artifactory.ManagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
+            name="terraform",
             password="my super secret password")
         ```
 
         ## Import
 
         Users can be imported using their name, e.g.
 
@@ -347,14 +347,15 @@
         # Create a new Artifactory user called terraform
         test_user = artifactory.ManagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
+            name="terraform",
             password="my super secret password")
         ```
 
         ## Import
 
         Users can be imported using their name, e.g.
 
@@ -397,14 +398,16 @@
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if password is None and not opts.urn:
                 raise TypeError("Missing required property 'password'")
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/oauth_settings.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/oauth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/outputs.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/permission_target.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/permission_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,57 +12,56 @@
 from ._inputs import *
 
 __all__ = ['PermissionTargetArgs', 'PermissionTarget']
 
 @pulumi.input_type
 class PermissionTargetArgs:
     def __init__(__self__, *,
+                 name: pulumi.Input[str],
                  build: Optional[pulumi.Input['PermissionTargetBuildArgs']] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  release_bundle: Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']] = None,
                  repo: Optional[pulumi.Input['PermissionTargetRepoArgs']] = None):
         """
         The set of arguments for constructing a PermissionTarget resource.
-        :param pulumi.Input['PermissionTargetBuildArgs'] build: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input[str] name: Name of permission.
+        :param pulumi.Input['PermissionTargetBuildArgs'] build: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input['PermissionTargetReleaseBundleArgs'] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input['PermissionTargetRepoArgs'] repo: Repository permission configuration.
         """
+        pulumi.set(__self__, "name", name)
         if build is not None:
             pulumi.set(__self__, "build", build)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if release_bundle is not None:
             pulumi.set(__self__, "release_bundle", release_bundle)
         if repo is not None:
             pulumi.set(__self__, "repo", repo)
 
     @property
     @pulumi.getter
-    def build(self) -> Optional[pulumi.Input['PermissionTargetBuildArgs']]:
+    def name(self) -> pulumi.Input[str]:
         """
-        As for repo but for artifactory-build-info permissions.
+        Name of permission.
         """
-        return pulumi.get(self, "build")
+        return pulumi.get(self, "name")
 
-    @build.setter
-    def build(self, value: Optional[pulumi.Input['PermissionTargetBuildArgs']]):
-        pulumi.set(self, "build", value)
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def build(self) -> Optional[pulumi.Input['PermissionTargetBuildArgs']]:
         """
-        Name of permission.
+        As for repo but for artifactory-build-info permissions.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "build")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @build.setter
+    def build(self, value: Optional[pulumi.Input['PermissionTargetBuildArgs']]):
+        pulumi.set(self, "build", value)
 
     @property
     @pulumi.getter(name="releaseBundle")
     def release_bundle(self) -> Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']]:
         """
         As for repo for for release-bundles permissions.
         """
@@ -187,14 +186,15 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
+            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -257,15 +257,15 @@
         :param pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']] repo: Repository permission configuration.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[PermissionTargetArgs] = None,
+                 args: PermissionTargetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Artifactory permission target resource. This can be used to create and manage Artifactory permission targets.
 
         ## Example Usage
 
         ```python
@@ -283,14 +283,15 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
+            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -371,14 +372,16 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PermissionTargetArgs.__new__(PermissionTargetArgs)
 
             __props__.__dict__["build"] = build
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["release_bundle"] = release_bundle
             __props__.__dict__["repo"] = repo
         super(PermissionTarget, __self__).__init__(
             'artifactory:index/permissionTarget:PermissionTarget',
             resource_name,
             __props__,
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/permission_targets.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/permission_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,57 +12,56 @@
 from ._inputs import *
 
 __all__ = ['PermissionTargetsArgs', 'PermissionTargets']
 
 @pulumi.input_type
 class PermissionTargetsArgs:
     def __init__(__self__, *,
+                 name: pulumi.Input[str],
                  build: Optional[pulumi.Input['PermissionTargetsBuildArgs']] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  release_bundle: Optional[pulumi.Input['PermissionTargetsReleaseBundleArgs']] = None,
                  repo: Optional[pulumi.Input['PermissionTargetsRepoArgs']] = None):
         """
         The set of arguments for constructing a PermissionTargets resource.
-        :param pulumi.Input['PermissionTargetsBuildArgs'] build: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input[str] name: Name of permission.
+        :param pulumi.Input['PermissionTargetsBuildArgs'] build: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input['PermissionTargetsReleaseBundleArgs'] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input['PermissionTargetsRepoArgs'] repo: Repository permission configuration.
         """
+        pulumi.set(__self__, "name", name)
         if build is not None:
             pulumi.set(__self__, "build", build)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if release_bundle is not None:
             pulumi.set(__self__, "release_bundle", release_bundle)
         if repo is not None:
             pulumi.set(__self__, "repo", repo)
 
     @property
     @pulumi.getter
-    def build(self) -> Optional[pulumi.Input['PermissionTargetsBuildArgs']]:
+    def name(self) -> pulumi.Input[str]:
         """
-        As for repo but for artifactory-build-info permissions.
+        Name of permission.
         """
-        return pulumi.get(self, "build")
+        return pulumi.get(self, "name")
 
-    @build.setter
-    def build(self, value: Optional[pulumi.Input['PermissionTargetsBuildArgs']]):
-        pulumi.set(self, "build", value)
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def build(self) -> Optional[pulumi.Input['PermissionTargetsBuildArgs']]:
         """
-        Name of permission.
+        As for repo but for artifactory-build-info permissions.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "build")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @build.setter
+    def build(self, value: Optional[pulumi.Input['PermissionTargetsBuildArgs']]):
+        pulumi.set(self, "build", value)
 
     @property
     @pulumi.getter(name="releaseBundle")
     def release_bundle(self) -> Optional[pulumi.Input['PermissionTargetsReleaseBundleArgs']]:
         """
         As for repo for for release-bundles permissions.
         """
@@ -187,14 +186,15 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
+            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -257,15 +257,15 @@
         :param pulumi.Input[pulumi.InputType['PermissionTargetsReleaseBundleArgs']] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input[pulumi.InputType['PermissionTargetsRepoArgs']] repo: Repository permission configuration.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[PermissionTargetsArgs] = None,
+                 args: PermissionTargetsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Artifactory permission target resource. This can be used to create and manage Artifactory permission targets.
 
         ## Example Usage
 
         ```python
@@ -283,14 +283,15 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
+            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -371,14 +372,16 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PermissionTargetsArgs.__new__(PermissionTargetsArgs)
 
             __props__.__dict__["build"] = build
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["release_bundle"] = release_bundle
             __props__.__dict__["repo"] = repo
         super(PermissionTargets, __self__).__init__(
             'artifactory:index/permissionTargets:PermissionTargets',
             resource_name,
             __props__,
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/property_set.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/property_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,52 +12,51 @@
 from ._inputs import *
 
 __all__ = ['PropertySetArgs', 'PropertySet']
 
 @pulumi.input_type
 class PropertySetArgs:
     def __init__(__self__, *,
+                 name: pulumi.Input[str],
                  properties: pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]],
-                 name: Optional[pulumi.Input[str]] = None,
                  visible: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a PropertySet resource.
-        :param pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]] properties: A list of properties that will be part of the property set.
         :param pulumi.Input[str] name: Predefined property name.
+        :param pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]] properties: A list of properties that will be part of the property set.
         :param pulumi.Input[bool] visible: Defines if the list visible and assignable to the repository or artifact. Default value is `true`.
         """
+        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "properties", properties)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if visible is not None:
             pulumi.set(__self__, "visible", visible)
 
     @property
     @pulumi.getter
-    def properties(self) -> pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]]:
+    def name(self) -> pulumi.Input[str]:
         """
-        A list of properties that will be part of the property set.
+        Predefined property name.
         """
-        return pulumi.get(self, "properties")
+        return pulumi.get(self, "name")
 
-    @properties.setter
-    def properties(self, value: pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]]):
-        pulumi.set(self, "properties", value)
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def properties(self) -> pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]]:
         """
-        Predefined property name.
+        A list of properties that will be part of the property set.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "properties")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @properties.setter
+    def properties(self, value: pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]]):
+        pulumi.set(self, "properties", value)
 
     @property
     @pulumi.getter
     def visible(self) -> Optional[pulumi.Input[bool]]:
         """
         Defines if the list visible and assignable to the repository or artifact. Default value is `true`.
         """
@@ -143,14 +142,15 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         foo = artifactory.PropertySet("foo",
+            name="property-set1",
             properties=[
                 artifactory.PropertySetPropertyArgs(
                     closed_predefined_values=True,
                     multiple_choice=True,
                     name="set1property1",
                     predefined_values=[
                         artifactory.PropertySetPropertyPredefinedValueArgs(
@@ -212,14 +212,15 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         foo = artifactory.PropertySet("foo",
+            name="property-set1",
             properties=[
                 artifactory.PropertySetPropertyArgs(
                     closed_predefined_values=True,
                     multiple_choice=True,
                     name="set1property1",
                     predefined_values=[
                         artifactory.PropertySetPropertyPredefinedValueArgs(
@@ -282,14 +283,16 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PropertySetArgs.__new__(PropertySetArgs)
 
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if properties is None and not opts.urn:
                 raise TypeError("Missing required property 'properties'")
             __props__.__dict__["properties"] = properties
             __props__.__dict__["visible"] = visible
         super(PropertySet, __self__).__init__(
             'artifactory:index/propertySet:PropertySet',
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/provider.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/proxy.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/pull_replication.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/pull_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/push_replication.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/push_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/release_bundle_webhook.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_cargo_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_cocoapods_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_docker_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_gitlfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_go_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_maven_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_opkg_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_p2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_pub_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_repository_replication.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_repository_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_terraform_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/remote_vcs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/replication_config.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/repository_layout.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/repository_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,43 +13,42 @@
 
 @pulumi.input_type
 class RepositoryLayoutArgs:
     def __init__(__self__, *,
                  artifact_path_pattern: pulumi.Input[str],
                  file_integration_revision_regexp: pulumi.Input[str],
                  folder_integration_revision_regexp: pulumi.Input[str],
+                 name: pulumi.Input[str],
                  descriptor_path_pattern: Optional[pulumi.Input[str]] = None,
-                 distinctive_descriptor_path_pattern: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 distinctive_descriptor_path_pattern: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a RepositoryLayout resource.
         :param pulumi.Input[str] artifact_path_pattern: Please refer to: [Path
                Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-ModulesandPathPatternsusedbyRepositoryLayouts)
                in the Artifactory Wiki documentation.
         :param pulumi.Input[str] file_integration_revision_regexp: A regular expression matching the integration revision string appearing in a file name as part of the artifact's path.
                For example, 'SNAPSHOT|(?:(?:[0-9]{8}.[0-9]{6})-(?:[0-9]+))', in Maven. Note! Take care not to introduce any regexp
                capturing groups within this expression. If not applicable use '.*'
         :param pulumi.Input[str] folder_integration_revision_regexp: A regular expression matching the integration revision string appearing in a folder name as part of the artifact's path.
                For example, 'SNAPSHOT', in Maven. Note! Take care not to introduce any regexp capturing groups within this expression.
                If not applicable use '.*'
+        :param pulumi.Input[str] name: Layout name
         :param pulumi.Input[str] descriptor_path_pattern: Please refer to: [Descriptor Path
                Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-DescriptorPathPatterns) in
                the Artifactory Wiki documentation.
         :param pulumi.Input[bool] distinctive_descriptor_path_pattern: When set, 'descriptor_path_pattern' will be used. Default to 'false'.
-        :param pulumi.Input[str] name: Layout name
         """
         pulumi.set(__self__, "artifact_path_pattern", artifact_path_pattern)
         pulumi.set(__self__, "file_integration_revision_regexp", file_integration_revision_regexp)
         pulumi.set(__self__, "folder_integration_revision_regexp", folder_integration_revision_regexp)
+        pulumi.set(__self__, "name", name)
         if descriptor_path_pattern is not None:
             pulumi.set(__self__, "descriptor_path_pattern", descriptor_path_pattern)
         if distinctive_descriptor_path_pattern is not None:
             pulumi.set(__self__, "distinctive_descriptor_path_pattern", distinctive_descriptor_path_pattern)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="artifactPathPattern")
     def artifact_path_pattern(self) -> pulumi.Input[str]:
         """
         Please refer to: [Path
         Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-ModulesandPathPatternsusedbyRepositoryLayouts)
@@ -86,14 +85,26 @@
         return pulumi.get(self, "folder_integration_revision_regexp")
 
     @folder_integration_revision_regexp.setter
     def folder_integration_revision_regexp(self, value: pulumi.Input[str]):
         pulumi.set(self, "folder_integration_revision_regexp", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Layout name
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="descriptorPathPattern")
     def descriptor_path_pattern(self) -> Optional[pulumi.Input[str]]:
         """
         Please refer to: [Descriptor Path
         Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-DescriptorPathPatterns) in
         the Artifactory Wiki documentation.
         """
@@ -111,26 +122,14 @@
         """
         return pulumi.get(self, "distinctive_descriptor_path_pattern")
 
     @distinctive_descriptor_path_pattern.setter
     def distinctive_descriptor_path_pattern(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "distinctive_descriptor_path_pattern", value)
 
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Layout name
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
 
 @pulumi.input_type
 class _RepositoryLayoutState:
     def __init__(__self__, *,
                  artifact_path_pattern: Optional[pulumi.Input[str]] = None,
                  descriptor_path_pattern: Optional[pulumi.Input[str]] = None,
                  distinctive_descriptor_path_pattern: Optional[pulumi.Input[bool]] = None,
@@ -324,14 +323,16 @@
             __props__.__dict__["distinctive_descriptor_path_pattern"] = distinctive_descriptor_path_pattern
             if file_integration_revision_regexp is None and not opts.urn:
                 raise TypeError("Missing required property 'file_integration_revision_regexp'")
             __props__.__dict__["file_integration_revision_regexp"] = file_integration_revision_regexp
             if folder_integration_revision_regexp is None and not opts.urn:
                 raise TypeError("Missing required property 'folder_integration_revision_regexp'")
             __props__.__dict__["folder_integration_revision_regexp"] = folder_integration_revision_regexp
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
         super(RepositoryLayout, __self__).__init__(
             'artifactory:index/repositoryLayout:RepositoryLayout',
             resource_name,
             __props__,
             opts)
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/saml_settings.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/saml_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/scoped_token.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_alpine_repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,570 +5,830 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ScopedTokenArgs', 'ScopedToken']
+__all__ = ['VirtualAlpineRepositoryArgs', 'VirtualAlpineRepository']
 
 @pulumi.input_type
-class ScopedTokenArgs:
+class VirtualAlpineRepositoryArgs:
     def __init__(__self__, *,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 key: pulumi.Input[str],
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a ScopedToken resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
-        """
-        if audiences is not None:
-            pulumi.set(__self__, "audiences", audiences)
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
+        """
+        The set of arguments for constructing a VirtualAlpineRepository resource.
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
+        """
+        pulumi.set(__self__, "key", key)
+        if artifactory_requests_can_retrieve_remote_artifacts is not None:
+            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
+        if default_deployment_repo is not None:
+            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if expires_in is not None:
-            pulumi.set(__self__, "expires_in", expires_in)
-        if refreshable is not None:
-            pulumi.set(__self__, "refreshable", refreshable)
-        if scopes is not None:
-            pulumi.set(__self__, "scopes", scopes)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+        if excludes_pattern is not None:
+            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
+        if includes_pattern is not None:
+            pulumi.set(__self__, "includes_pattern", includes_pattern)
+        if notes is not None:
+            pulumi.set(__self__, "notes", notes)
+        if primary_keypair_ref is not None:
+            pulumi.set(__self__, "primary_keypair_ref", primary_keypair_ref)
+        if project_environments is not None:
+            pulumi.set(__self__, "project_environments", project_environments)
+        if project_key is not None:
+            pulumi.set(__self__, "project_key", project_key)
+        if repo_layout_ref is not None:
+            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
+        if repositories is not None:
+            pulumi.set(__self__, "repositories", repositories)
+        if retrieval_cache_period_seconds is not None:
+            pulumi.set(__self__, "retrieval_cache_period_seconds", retrieval_cache_period_seconds)
 
     @property
     @pulumi.getter
-    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def key(self) -> pulumi.Input[str]:
         """
-        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+        contain spaces or special characters.
         """
-        return pulumi.get(self, "audiences")
+        return pulumi.get(self, "key")
 
-    @audiences.setter
-    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "audiences", value)
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
+    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+        another Artifactory instance.
+        """
+        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
+
+    @artifactory_requests_can_retrieve_remote_artifacts.setter
+    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
+
+    @property
+    @pulumi.getter(name="defaultDeploymentRepo")
+    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default repository to deploy artifacts.
+        """
+        return pulumi.get(self, "default_deployment_repo")
+
+    @default_deployment_repo.setter
+    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_deployment_repo", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        Public description.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="expiresIn")
-    def expires_in(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="excludesPattern")
+    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+        artifacts are excluded.
         """
-        return pulumi.get(self, "expires_in")
+        return pulumi.get(self, "excludes_pattern")
 
-    @expires_in.setter
-    def expires_in(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expires_in", value)
+    @excludes_pattern.setter
+    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "excludes_pattern", value)
 
     @property
-    @pulumi.getter
-    def refreshable(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="includesPattern")
+    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Is this token refreshable? Defaults to `false`
+        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         """
-        return pulumi.get(self, "refreshable")
+        return pulumi.get(self, "includes_pattern")
 
-    @refreshable.setter
-    def refreshable(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "refreshable", value)
+    @includes_pattern.setter
+    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "includes_pattern", value)
 
     @property
     @pulumi.getter
-    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def notes(self) -> Optional[pulumi.Input[str]]:
+        """
+        Internal description.
+        """
+        return pulumi.get(self, "notes")
+
+    @notes.setter
+    def notes(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "notes", value)
+
+    @property
+    @pulumi.getter(name="primaryKeypairRef")
+    def primary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        Primary keypair used to sign artifacts. Default value is empty.
         """
-        return pulumi.get(self, "scopes")
+        return pulumi.get(self, "primary_keypair_ref")
 
-    @scopes.setter
-    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "scopes", value)
+    @primary_keypair_ref.setter
+    def primary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "primary_keypair_ref", value)
+
+    @property
+    @pulumi.getter(name="projectEnvironments")
+    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        """
+        return pulumi.get(self, "project_environments")
+
+    @project_environments.setter
+    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "project_environments", value)
+
+    @property
+    @pulumi.getter(name="projectKey")
+    def project_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        """
+        return pulumi.get(self, "project_key")
+
+    @project_key.setter
+    def project_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_key", value)
+
+    @property
+    @pulumi.getter(name="repoLayoutRef")
+    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
+        """
+        Repository layout key for the local repository
+        """
+        return pulumi.get(self, "repo_layout_ref")
+
+    @repo_layout_ref.setter
+    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo_layout_ref", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The effective list of actual repositories included in this virtual repository.
+        """
+        return pulumi.get(self, "repositories")
+
+    @repositories.setter
+    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "repositories", value)
+
+    @property
+    @pulumi.getter(name="retrievalCachePeriodSeconds")
+    def retrieval_cache_period_seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "retrieval_cache_period_seconds")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @retrieval_cache_period_seconds.setter
+    def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
 @pulumi.input_type
-class _ScopedTokenState:
+class _VirtualAlpineRepositoryState:
     def __init__(__self__, *,
-                 access_token: Optional[pulumi.Input[str]] = None,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 expiry: Optional[pulumi.Input[int]] = None,
-                 issued_at: Optional[pulumi.Input[int]] = None,
-                 issuer: Optional[pulumi.Input[str]] = None,
-                 refresh_token: Optional[pulumi.Input[str]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 subject: Optional[pulumi.Input[str]] = None,
-                 token_type: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering ScopedToken resources.
-        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[int] expiry: Returns the token expiry
-        :param pulumi.Input[int] issued_at: Returns the token issued at date/time
-        :param pulumi.Input[str] issuer: Returns the token issuer
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] subject: Returns the token type
-        :param pulumi.Input[str] token_type: Returns the token type
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
-        """
-        if access_token is not None:
-            pulumi.set(__self__, "access_token", access_token)
-        if audiences is not None:
-            pulumi.set(__self__, "audiences", audiences)
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 package_type: Optional[pulumi.Input[str]] = None,
+                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
+        """
+        Input properties used for looking up and filtering VirtualAlpineRepository resources.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
+        """
+        if artifactory_requests_can_retrieve_remote_artifacts is not None:
+            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
+        if default_deployment_repo is not None:
+            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if expires_in is not None:
-            pulumi.set(__self__, "expires_in", expires_in)
-        if expiry is not None:
-            pulumi.set(__self__, "expiry", expiry)
-        if issued_at is not None:
-            pulumi.set(__self__, "issued_at", issued_at)
-        if issuer is not None:
-            pulumi.set(__self__, "issuer", issuer)
-        if refresh_token is not None:
-            pulumi.set(__self__, "refresh_token", refresh_token)
-        if refreshable is not None:
-            pulumi.set(__self__, "refreshable", refreshable)
-        if scopes is not None:
-            pulumi.set(__self__, "scopes", scopes)
-        if subject is not None:
-            pulumi.set(__self__, "subject", subject)
-        if token_type is not None:
-            pulumi.set(__self__, "token_type", token_type)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
-
-    @property
-    @pulumi.getter(name="accessToken")
-    def access_token(self) -> Optional[pulumi.Input[str]]:
-        """
-        Returns the access token to authenticate to Artifactory
-        """
-        return pulumi.get(self, "access_token")
-
-    @access_token.setter
-    def access_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "access_token", value)
-
-    @property
-    @pulumi.getter
-    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        """
-        return pulumi.get(self, "audiences")
-
-    @audiences.setter
-    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "audiences", value)
+        if excludes_pattern is not None:
+            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
+        if includes_pattern is not None:
+            pulumi.set(__self__, "includes_pattern", includes_pattern)
+        if key is not None:
+            pulumi.set(__self__, "key", key)
+        if notes is not None:
+            pulumi.set(__self__, "notes", notes)
+        if package_type is not None:
+            pulumi.set(__self__, "package_type", package_type)
+        if primary_keypair_ref is not None:
+            pulumi.set(__self__, "primary_keypair_ref", primary_keypair_ref)
+        if project_environments is not None:
+            pulumi.set(__self__, "project_environments", project_environments)
+        if project_key is not None:
+            pulumi.set(__self__, "project_key", project_key)
+        if repo_layout_ref is not None:
+            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
+        if repositories is not None:
+            pulumi.set(__self__, "repositories", repositories)
+        if retrieval_cache_period_seconds is not None:
+            pulumi.set(__self__, "retrieval_cache_period_seconds", retrieval_cache_period_seconds)
+
+    @property
+    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
+    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+        another Artifactory instance.
+        """
+        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
+
+    @artifactory_requests_can_retrieve_remote_artifacts.setter
+    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
+
+    @property
+    @pulumi.getter(name="defaultDeploymentRepo")
+    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
+        """
+        Default repository to deploy artifacts.
+        """
+        return pulumi.get(self, "default_deployment_repo")
+
+    @default_deployment_repo.setter
+    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_deployment_repo", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        Public description.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="expiresIn")
-    def expires_in(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="excludesPattern")
+    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+        artifacts are excluded.
         """
-        return pulumi.get(self, "expires_in")
+        return pulumi.get(self, "excludes_pattern")
 
-    @expires_in.setter
-    def expires_in(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expires_in", value)
+    @excludes_pattern.setter
+    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "excludes_pattern", value)
 
     @property
-    @pulumi.getter
-    def expiry(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="includesPattern")
+    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token expiry
+        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         """
-        return pulumi.get(self, "expiry")
+        return pulumi.get(self, "includes_pattern")
 
-    @expiry.setter
-    def expiry(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "expiry", value)
+    @includes_pattern.setter
+    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "includes_pattern", value)
 
     @property
-    @pulumi.getter(name="issuedAt")
-    def issued_at(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def key(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token issued at date/time
+        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+        contain spaces or special characters.
         """
-        return pulumi.get(self, "issued_at")
+        return pulumi.get(self, "key")
 
-    @issued_at.setter
-    def issued_at(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "issued_at", value)
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
-    def issuer(self) -> Optional[pulumi.Input[str]]:
+    def notes(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token issuer
+        Internal description.
         """
-        return pulumi.get(self, "issuer")
+        return pulumi.get(self, "notes")
 
-    @issuer.setter
-    def issuer(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "issuer", value)
+    @notes.setter
+    def notes(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "notes", value)
 
     @property
-    @pulumi.getter(name="refreshToken")
-    def refresh_token(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "refresh_token")
+    @pulumi.getter(name="packageType")
+    def package_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "package_type")
 
-    @refresh_token.setter
-    def refresh_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "refresh_token", value)
+    @package_type.setter
+    def package_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "package_type", value)
 
     @property
-    @pulumi.getter
-    def refreshable(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="primaryKeypairRef")
+    def primary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        (Optional) Is this token refreshable? Defaults to `false`
+        Primary keypair used to sign artifacts. Default value is empty.
         """
-        return pulumi.get(self, "refreshable")
+        return pulumi.get(self, "primary_keypair_ref")
 
-    @refreshable.setter
-    def refreshable(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "refreshable", value)
+    @primary_keypair_ref.setter
+    def primary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "primary_keypair_ref", value)
 
     @property
-    @pulumi.getter
-    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="projectEnvironments")
+    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         """
-        return pulumi.get(self, "scopes")
+        return pulumi.get(self, "project_environments")
 
-    @scopes.setter
-    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "scopes", value)
+    @project_environments.setter
+    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "project_environments", value)
 
     @property
-    @pulumi.getter
-    def subject(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="projectKey")
+    def project_key(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token type
+        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         """
-        return pulumi.get(self, "subject")
+        return pulumi.get(self, "project_key")
 
-    @subject.setter
-    def subject(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "subject", value)
+    @project_key.setter
+    def project_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_key", value)
 
     @property
-    @pulumi.getter(name="tokenType")
-    def token_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="repoLayoutRef")
+    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        Returns the token type
+        Repository layout key for the local repository
         """
-        return pulumi.get(self, "token_type")
+        return pulumi.get(self, "repo_layout_ref")
 
-    @token_type.setter
-    def token_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "token_type", value)
+    @repo_layout_ref.setter
+    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "repo_layout_ref", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The effective list of actual repositories included in this virtual repository.
+        """
+        return pulumi.get(self, "repositories")
+
+    @repositories.setter
+    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "repositories", value)
+
+    @property
+    @pulumi.getter(name="retrievalCachePeriodSeconds")
+    def retrieval_cache_period_seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "retrieval_cache_period_seconds")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @retrieval_cache_period_seconds.setter
+    def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
-class ScopedToken(pulumi.CustomResource):
+class VirtualAlpineRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
+        Creates a virtual Alpine repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-VirtualRepositorySettingupaVirtualRepository).
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        foo_alpine = artifactory.VirtualAlpineRepository("foo-alpine",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="foo-alpine",
+            notes="Internal description",
+            repositories=[])
+        ```
+
         ## Import
 
-        Artifactory **does not** retain scoped tokens and cannot be imported into state.
+        Virtual repositories can be imported using their name, e.g.
+
+        ```sh
+         $ pulumi import artifactory:index/virtualAlpineRepository:VirtualAlpineRepository foo-alpine foo-alpine
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ScopedTokenArgs] = None,
+                 args: VirtualAlpineRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Creates a virtual Alpine repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-VirtualRepositorySettingupaVirtualRepository).
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        foo_alpine = artifactory.VirtualAlpineRepository("foo-alpine",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="foo-alpine",
+            notes="Internal description",
+            repositories=[])
+        ```
+
         ## Import
 
-        Artifactory **does not** retain scoped tokens and cannot be imported into state.
+        Virtual repositories can be imported using their name, e.g.
+
+        ```sh
+         $ pulumi import artifactory:index/virtualAlpineRepository:VirtualAlpineRepository foo-alpine foo-alpine
+        ```
 
         :param str resource_name: The name of the resource.
-        :param ScopedTokenArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualAlpineRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ScopedTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualAlpineRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 expires_in: Optional[pulumi.Input[int]] = None,
-                 refreshable: Optional[pulumi.Input[bool]] = None,
-                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 excludes_pattern: Optional[pulumi.Input[str]] = None,
+                 includes_pattern: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 notes: Optional[pulumi.Input[str]] = None,
+                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
+                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 project_key: Optional[pulumi.Input[str]] = None,
+                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ScopedTokenArgs.__new__(ScopedTokenArgs)
+            __props__ = VirtualAlpineRepositoryArgs.__new__(VirtualAlpineRepositoryArgs)
 
-            __props__.__dict__["audiences"] = audiences
+            __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
+            __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
-            __props__.__dict__["expires_in"] = expires_in
-            __props__.__dict__["refreshable"] = refreshable
-            __props__.__dict__["scopes"] = scopes
-            __props__.__dict__["username"] = username
-            __props__.__dict__["access_token"] = None
-            __props__.__dict__["expiry"] = None
-            __props__.__dict__["issued_at"] = None
-            __props__.__dict__["issuer"] = None
-            __props__.__dict__["refresh_token"] = None
-            __props__.__dict__["subject"] = None
-            __props__.__dict__["token_type"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "refreshToken"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(ScopedToken, __self__).__init__(
-            'artifactory:index/scopedToken:ScopedToken',
+            __props__.__dict__["excludes_pattern"] = excludes_pattern
+            __props__.__dict__["includes_pattern"] = includes_pattern
+            if key is None and not opts.urn:
+                raise TypeError("Missing required property 'key'")
+            __props__.__dict__["key"] = key
+            __props__.__dict__["notes"] = notes
+            __props__.__dict__["primary_keypair_ref"] = primary_keypair_ref
+            __props__.__dict__["project_environments"] = project_environments
+            __props__.__dict__["project_key"] = project_key
+            __props__.__dict__["repo_layout_ref"] = repo_layout_ref
+            __props__.__dict__["repositories"] = repositories
+            __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
+            __props__.__dict__["package_type"] = None
+        super(VirtualAlpineRepository, __self__).__init__(
+            'artifactory:index/virtualAlpineRepository:VirtualAlpineRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            access_token: Optional[pulumi.Input[str]] = None,
-            audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
+            default_deployment_repo: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            expires_in: Optional[pulumi.Input[int]] = None,
-            expiry: Optional[pulumi.Input[int]] = None,
-            issued_at: Optional[pulumi.Input[int]] = None,
-            issuer: Optional[pulumi.Input[str]] = None,
-            refresh_token: Optional[pulumi.Input[str]] = None,
-            refreshable: Optional[pulumi.Input[bool]] = None,
-            scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            subject: Optional[pulumi.Input[str]] = None,
-            token_type: Optional[pulumi.Input[str]] = None,
-            username: Optional[pulumi.Input[str]] = None) -> 'ScopedToken':
+            excludes_pattern: Optional[pulumi.Input[str]] = None,
+            includes_pattern: Optional[pulumi.Input[str]] = None,
+            key: Optional[pulumi.Input[str]] = None,
+            notes: Optional[pulumi.Input[str]] = None,
+            package_type: Optional[pulumi.Input[str]] = None,
+            primary_keypair_ref: Optional[pulumi.Input[str]] = None,
+            project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            project_key: Optional[pulumi.Input[str]] = None,
+            repo_layout_ref: Optional[pulumi.Input[str]] = None,
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualAlpineRepository':
         """
-        Get an existing ScopedToken resource's state with the given name, id, and optional extra
+        Get an existing VirtualAlpineRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
-        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
-        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
-        :param pulumi.Input[int] expiry: Returns the token expiry
-        :param pulumi.Input[int] issued_at: Returns the token issued at date/time
-        :param pulumi.Input[str] issuer: Returns the token issuer
-        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
-        :param pulumi.Input[str] subject: Returns the token type
-        :param pulumi.Input[str] token_type: Returns the token type
-        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+               another Artifactory instance.
+        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
+        :param pulumi.Input[str] description: Public description.
+        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+               artifacts are excluded.
+        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+               contain spaces or special characters.
+        :param pulumi.Input[str] notes: Internal description.
+        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ScopedTokenState.__new__(_ScopedTokenState)
+        __props__ = _VirtualAlpineRepositoryState.__new__(_VirtualAlpineRepositoryState)
 
-        __props__.__dict__["access_token"] = access_token
-        __props__.__dict__["audiences"] = audiences
+        __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
+        __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
-        __props__.__dict__["expires_in"] = expires_in
-        __props__.__dict__["expiry"] = expiry
-        __props__.__dict__["issued_at"] = issued_at
-        __props__.__dict__["issuer"] = issuer
-        __props__.__dict__["refresh_token"] = refresh_token
-        __props__.__dict__["refreshable"] = refreshable
-        __props__.__dict__["scopes"] = scopes
-        __props__.__dict__["subject"] = subject
-        __props__.__dict__["token_type"] = token_type
-        __props__.__dict__["username"] = username
-        return ScopedToken(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["excludes_pattern"] = excludes_pattern
+        __props__.__dict__["includes_pattern"] = includes_pattern
+        __props__.__dict__["key"] = key
+        __props__.__dict__["notes"] = notes
+        __props__.__dict__["package_type"] = package_type
+        __props__.__dict__["primary_keypair_ref"] = primary_keypair_ref
+        __props__.__dict__["project_environments"] = project_environments
+        __props__.__dict__["project_key"] = project_key
+        __props__.__dict__["repo_layout_ref"] = repo_layout_ref
+        __props__.__dict__["repositories"] = repositories
+        __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
+        return VirtualAlpineRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="accessToken")
-    def access_token(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
+    def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
-        Returns the access token to authenticate to Artifactory
+        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
+        another Artifactory instance.
         """
-        return pulumi.get(self, "access_token")
+        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
 
     @property
-    @pulumi.getter
-    def audiences(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="defaultDeploymentRepo")
+    def default_deployment_repo(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        Default repository to deploy artifacts.
         """
-        return pulumi.get(self, "audiences")
+        return pulumi.get(self, "default_deployment_repo")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        Public description.
         """
         return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="expiresIn")
-    def expires_in(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="excludesPattern")
+    def excludes_pattern(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
+        artifacts are excluded.
         """
-        return pulumi.get(self, "expires_in")
+        return pulumi.get(self, "excludes_pattern")
 
     @property
-    @pulumi.getter
-    def expiry(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="includesPattern")
+    def includes_pattern(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token expiry
+        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
+        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         """
-        return pulumi.get(self, "expiry")
+        return pulumi.get(self, "includes_pattern")
 
     @property
-    @pulumi.getter(name="issuedAt")
-    def issued_at(self) -> pulumi.Output[int]:
+    @pulumi.getter
+    def key(self) -> pulumi.Output[str]:
         """
-        Returns the token issued at date/time
+        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
+        contain spaces or special characters.
         """
-        return pulumi.get(self, "issued_at")
+        return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
-    def issuer(self) -> pulumi.Output[str]:
+    def notes(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token issuer
+        Internal description.
         """
-        return pulumi.get(self, "issuer")
+        return pulumi.get(self, "notes")
 
     @property
-    @pulumi.getter(name="refreshToken")
-    def refresh_token(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "refresh_token")
+    @pulumi.getter(name="packageType")
+    def package_type(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "package_type")
 
     @property
-    @pulumi.getter
-    def refreshable(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="primaryKeypairRef")
+    def primary_keypair_ref(self) -> pulumi.Output[Optional[str]]:
         """
-        (Optional) Is this token refreshable? Defaults to `false`
+        Primary keypair used to sign artifacts. Default value is empty.
         """
-        return pulumi.get(self, "refreshable")
+        return pulumi.get(self, "primary_keypair_ref")
 
     @property
-    @pulumi.getter
-    def scopes(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="projectEnvironments")
+    def project_environments(self) -> pulumi.Output[Sequence[str]]:
         """
-        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
+        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
+        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
+        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         """
-        return pulumi.get(self, "scopes")
+        return pulumi.get(self, "project_environments")
 
     @property
-    @pulumi.getter
-    def subject(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="projectKey")
+    def project_key(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token type
+        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
+        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         """
-        return pulumi.get(self, "subject")
+        return pulumi.get(self, "project_key")
 
     @property
-    @pulumi.getter(name="tokenType")
-    def token_type(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="repoLayoutRef")
+    def repo_layout_ref(self) -> pulumi.Output[Optional[str]]:
         """
-        Returns the token type
+        Repository layout key for the local repository
         """
-        return pulumi.get(self, "token_type")
+        return pulumi.get(self, "repo_layout_ref")
 
     @property
     @pulumi.getter
-    def username(self) -> pulumi.Output[Optional[str]]:
+    def repositories(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        The effective list of actual repositories included in this virtual repository.
+        """
+        return pulumi.get(self, "repositories")
+
+    @property
+    @pulumi.getter(name="retrievalCachePeriodSeconds")
+    def retrieval_cache_period_seconds(self) -> pulumi.Output[Optional[int]]:
         """
-        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "retrieval_cache_period_seconds")
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/single_replication_config.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/single_replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/unmanaged_user.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/unmanaged_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,43 +11,42 @@
 
 __all__ = ['UnmanagedUserArgs', 'UnmanagedUser']
 
 @pulumi.input_type
 class UnmanagedUserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
+                 name: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a UnmanagedUser resource.
         :param pulumi.Input[str] email: Email for user.
+        :param pulumi.Input[str] name: Username for user.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
-        :param pulumi.Input[str] name: Username for user.
         :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "name", name)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
@@ -59,14 +58,26 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Username for user.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
@@ -107,26 +118,14 @@
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Username for user.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
         Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         """
         return pulumi.get(self, "password")
 
     @password.setter
@@ -306,14 +305,15 @@
         # Create a new Artifactory user called terraform
         test_user = artifactory.UnmanagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
+            name="terraform",
             password="my super secret password")
         ```
         ## Managing groups relationship
 
         See our recommendation on how to manage user-group relationship.
 
         ## Import
@@ -351,14 +351,15 @@
         # Create a new Artifactory user called terraform
         test_user = artifactory.UnmanagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
+            name="terraform",
             password="my super secret password")
         ```
         ## Managing groups relationship
 
         See our recommendation on how to manage user-group relationship.
 
         ## Import
@@ -404,14 +405,16 @@
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(UnmanagedUser, __self__).__init__(
             'artifactory:index/unmanagedUser:UnmanagedUser',
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/user.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,43 +11,42 @@
 
 __all__ = ['UserArgs', 'User']
 
 @pulumi.input_type
 class UserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
+                 name: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a User resource.
         :param pulumi.Input[str] email: Email for user.
+        :param pulumi.Input[str] name: Username for user.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
-        :param pulumi.Input[str] name: Username for user.
         :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "name", name)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
@@ -59,14 +58,26 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Username for user.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
@@ -107,26 +118,14 @@
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Username for user.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
         Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         """
         return pulumi.get(self, "password")
 
     @password.setter
@@ -312,14 +311,15 @@
         # Create a new Artifactory user called terraform
         test_user = artifactory.User("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
+            name="terraform",
             password="my super secret password")
         ```
         ## Managing groups relationship
 
         See our recommendation on how to manage user-group relationship.
 
         ## Import
@@ -363,14 +363,15 @@
         # Create a new Artifactory user called terraform
         test_user = artifactory.User("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
+            name="terraform",
             password="my super secret password")
         ```
         ## Managing groups relationship
 
         See our recommendation on how to manage user-group relationship.
 
         ## Import
@@ -416,14 +417,16 @@
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
+            if name is None and not opts.urn:
+                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(User, __self__).__init__(
             'artifactory:index/user:User',
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_alpine_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_conan_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualAlpineRepositoryArgs', 'VirtualAlpineRepository']
+__all__ = ['VirtualConanRepositoryArgs', 'VirtualConanRepository']
 
 @pulumi.input_type
-class VirtualAlpineRepositoryArgs:
+class VirtualConanRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
-                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
         """
-        The set of arguments for constructing a VirtualAlpineRepository resource.
+        The set of arguments for constructing a VirtualConanRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
                used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
@@ -60,16 +58,14 @@
             pulumi.set(__self__, "description", description)
         if excludes_pattern is not None:
             pulumi.set(__self__, "excludes_pattern", excludes_pattern)
         if includes_pattern is not None:
             pulumi.set(__self__, "includes_pattern", includes_pattern)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
-        if primary_keypair_ref is not None:
-            pulumi.set(__self__, "primary_keypair_ref", primary_keypair_ref)
         if project_environments is not None:
             pulumi.set(__self__, "project_environments", project_environments)
         if project_key is not None:
             pulumi.set(__self__, "project_key", project_key)
         if repo_layout_ref is not None:
             pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
         if repositories is not None:
@@ -162,26 +158,14 @@
         return pulumi.get(self, "notes")
 
     @notes.setter
     def notes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notes", value)
 
     @property
-    @pulumi.getter(name="primaryKeypairRef")
-    def primary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
-        """
-        Primary keypair used to sign artifacts. Default value is empty.
-        """
-        return pulumi.get(self, "primary_keypair_ref")
-
-    @primary_keypair_ref.setter
-    def primary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "primary_keypair_ref", value)
-
-    @property
     @pulumi.getter(name="projectEnvironments")
     def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
         Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
         attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
         be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
@@ -239,44 +223,42 @@
 
     @retrieval_cache_period_seconds.setter
     def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
 @pulumi.input_type
-class _VirtualAlpineRepositoryState:
+class _VirtualConanRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
-                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
         """
-        Input properties used for looking up and filtering VirtualAlpineRepository resources.
+        Input properties used for looking up and filtering VirtualConanRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
                used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
@@ -295,16 +277,14 @@
             pulumi.set(__self__, "includes_pattern", includes_pattern)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
         if package_type is not None:
             pulumi.set(__self__, "package_type", package_type)
-        if primary_keypair_ref is not None:
-            pulumi.set(__self__, "primary_keypair_ref", primary_keypair_ref)
         if project_environments is not None:
             pulumi.set(__self__, "project_environments", project_environments)
         if project_key is not None:
             pulumi.set(__self__, "project_key", project_key)
         if repo_layout_ref is not None:
             pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
         if repositories is not None:
@@ -406,26 +386,14 @@
         return pulumi.get(self, "package_type")
 
     @package_type.setter
     def package_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "package_type", value)
 
     @property
-    @pulumi.getter(name="primaryKeypairRef")
-    def primary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
-        """
-        Primary keypair used to sign artifacts. Default value is empty.
-        """
-        return pulumi.get(self, "primary_keypair_ref")
-
-    @primary_keypair_ref.setter
-    def primary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "primary_keypair_ref", value)
-
-    @property
     @pulumi.getter(name="projectEnvironments")
     def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
         Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
         attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
         be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
@@ -482,58 +450,58 @@
         return pulumi.get(self, "retrieval_cache_period_seconds")
 
     @retrieval_cache_period_seconds.setter
     def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
-class VirtualAlpineRepository(pulumi.CustomResource):
+class VirtualConanRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
-                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Creates a virtual Alpine repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-VirtualRepositorySettingupaVirtualRepository).
+        Creates a virtual Conan repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conan+Repositories#ConanRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_alpine = artifactory.VirtualAlpineRepository("foo-alpine",
+        foo_conan = artifactory.VirtualConanRepository("foo-conan",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-alpine",
+            key="foo-conan",
             notes="Internal description",
+            repo_layout_ref="conan-default",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualAlpineRepository:VirtualAlpineRepository foo-alpine foo-alpine
+         $ pulumi import artifactory:index/virtualConanRepository:VirtualConanRepository foo-conan foo-conan
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -541,65 +509,65 @@
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
                used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualAlpineRepositoryArgs,
+                 args: VirtualConanRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Alpine repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-VirtualRepositorySettingupaVirtualRepository).
+        Creates a virtual Conan repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conan+Repositories#ConanRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_alpine = artifactory.VirtualAlpineRepository("foo-alpine",
+        foo_conan = artifactory.VirtualConanRepository("foo-conan",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-alpine",
+            key="foo-conan",
             notes="Internal description",
+            repo_layout_ref="conan-default",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualAlpineRepository:VirtualAlpineRepository foo-alpine foo-alpine
+         $ pulumi import artifactory:index/virtualConanRepository:VirtualConanRepository foo-conan foo-conan
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualAlpineRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualConanRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualAlpineRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualConanRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -607,47 +575,45 @@
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
-                 primary_keypair_ref: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualAlpineRepositoryArgs.__new__(VirtualAlpineRepositoryArgs)
+            __props__ = VirtualConanRepositoryArgs.__new__(VirtualConanRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
-            __props__.__dict__["primary_keypair_ref"] = primary_keypair_ref
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
             __props__.__dict__["package_type"] = None
-        super(VirtualAlpineRepository, __self__).__init__(
-            'artifactory:index/virtualAlpineRepository:VirtualAlpineRepository',
+        super(VirtualConanRepository, __self__).__init__(
+            'artifactory:index/virtualConanRepository:VirtualConanRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -656,22 +622,21 @@
             default_deployment_repo: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             excludes_pattern: Optional[pulumi.Input[str]] = None,
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
-            primary_keypair_ref: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
             repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualAlpineRepository':
+            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualConanRepository':
         """
-        Get an existing VirtualAlpineRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualConanRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -680,44 +645,42 @@
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
                used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: Primary keypair used to sign artifacts. Default value is empty.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualAlpineRepositoryState.__new__(_VirtualAlpineRepositoryState)
+        __props__ = _VirtualConanRepositoryState.__new__(_VirtualConanRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
-        __props__.__dict__["primary_keypair_ref"] = primary_keypair_ref
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
         __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
-        return VirtualAlpineRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualConanRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
@@ -777,22 +740,14 @@
 
     @property
     @pulumi.getter(name="packageType")
     def package_type(self) -> pulumi.Output[str]:
         return pulumi.get(self, "package_type")
 
     @property
-    @pulumi.getter(name="primaryKeypairRef")
-    def primary_keypair_ref(self) -> pulumi.Output[Optional[str]]:
-        """
-        Primary keypair used to sign artifacts. Default value is empty.
-        """
-        return pulumi.get(self, "primary_keypair_ref")
-
-    @property
     @pulumi.getter(name="projectEnvironments")
     def project_environments(self) -> pulumi.Output[Sequence[str]]:
         """
         Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
         Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
         attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
         be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_bower_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_chef_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_composer_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_conan_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_conda_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualConanRepositoryArgs', 'VirtualConanRepository']
+__all__ = ['VirtualCondaRepositoryArgs', 'VirtualCondaRepository']
 
 @pulumi.input_type
-class VirtualConanRepositoryArgs:
+class VirtualCondaRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
         """
-        The set of arguments for constructing a VirtualConanRepository resource.
+        The set of arguments for constructing a VirtualCondaRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -223,15 +223,15 @@
 
     @retrieval_cache_period_seconds.setter
     def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
 @pulumi.input_type
-class _VirtualConanRepositoryState:
+class _VirtualCondaRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
@@ -239,15 +239,15 @@
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
         """
-        Input properties used for looking up and filtering VirtualConanRepository resources.
+        Input properties used for looking up and filtering VirtualCondaRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -450,15 +450,15 @@
         return pulumi.get(self, "retrieval_cache_period_seconds")
 
     @retrieval_cache_period_seconds.setter
     def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
-class VirtualConanRepository(pulumi.CustomResource):
+class VirtualCondaRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -469,39 +469,38 @@
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Creates a virtual Conan repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conan+Repositories#ConanRepositories-VirtualRepositories).
+        Creates a virtual Conda repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conda+Repositories#CondaRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_conan = artifactory.VirtualConanRepository("foo-conan",
+        foo_conda = artifactory.VirtualCondaRepository("foo-conda",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-conan",
+            key="foo-conda",
             notes="Internal description",
-            repo_layout_ref="conan-default",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualConanRepository:VirtualConanRepository foo-conan foo-conan
+         $ pulumi import artifactory:index/virtualCondaRepository:VirtualCondaRepository foo-conda foo-conda
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -523,51 +522,50 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualConanRepositoryArgs,
+                 args: VirtualCondaRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Conan repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conan+Repositories#ConanRepositories-VirtualRepositories).
+        Creates a virtual Conda repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conda+Repositories#CondaRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_conan = artifactory.VirtualConanRepository("foo-conan",
+        foo_conda = artifactory.VirtualCondaRepository("foo-conda",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-conan",
+            key="foo-conda",
             notes="Internal description",
-            repo_layout_ref="conan-default",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualConanRepository:VirtualConanRepository foo-conan foo-conan
+         $ pulumi import artifactory:index/virtualCondaRepository:VirtualCondaRepository foo-conda foo-conda
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualConanRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualCondaRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualConanRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualCondaRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -587,15 +585,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualConanRepositoryArgs.__new__(VirtualConanRepositoryArgs)
+            __props__ = VirtualCondaRepositoryArgs.__new__(VirtualCondaRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -604,16 +602,16 @@
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
             __props__.__dict__["package_type"] = None
-        super(VirtualConanRepository, __self__).__init__(
-            'artifactory:index/virtualConanRepository:VirtualConanRepository',
+        super(VirtualCondaRepository, __self__).__init__(
+            'artifactory:index/virtualCondaRepository:VirtualCondaRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -626,17 +624,17 @@
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
             repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualConanRepository':
+            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualCondaRepository':
         """
-        Get an existing VirtualConanRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualCondaRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -657,30 +655,30 @@
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualConanRepositoryState.__new__(_VirtualConanRepositoryState)
+        __props__ = _VirtualCondaRepositoryState.__new__(_VirtualCondaRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
         __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
-        return VirtualConanRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualCondaRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_conda_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_cran_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualCondaRepositoryArgs', 'VirtualCondaRepository']
+__all__ = ['VirtualCranRepositoryArgs', 'VirtualCranRepository']
 
 @pulumi.input_type
-class VirtualCondaRepositoryArgs:
+class VirtualCranRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
         """
-        The set of arguments for constructing a VirtualCondaRepository resource.
+        The set of arguments for constructing a VirtualCranRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -223,15 +223,15 @@
 
     @retrieval_cache_period_seconds.setter
     def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
 @pulumi.input_type
-class _VirtualCondaRepositoryState:
+class _VirtualCranRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
@@ -239,15 +239,15 @@
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
         """
-        Input properties used for looking up and filtering VirtualCondaRepository resources.
+        Input properties used for looking up and filtering VirtualCranRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -450,15 +450,15 @@
         return pulumi.get(self, "retrieval_cache_period_seconds")
 
     @retrieval_cache_period_seconds.setter
     def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retrieval_cache_period_seconds", value)
 
 
-class VirtualCondaRepository(pulumi.CustomResource):
+class VirtualCranRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -469,38 +469,38 @@
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Creates a virtual Conda repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conda+Repositories#CondaRepositories-VirtualRepositories).
+        Creates a virtual Cran repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/CRAN+Repositories#CRANRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_conda = artifactory.VirtualCondaRepository("foo-conda",
+        foo_cran = artifactory.VirtualCranRepository("foo-cran",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-conda",
+            key="foo-cran",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualCondaRepository:VirtualCondaRepository foo-conda foo-conda
+         $ pulumi import artifactory:index/virtualCranRepository:VirtualCranRepository foo-cran foo-cran
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -522,50 +522,50 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualCondaRepositoryArgs,
+                 args: VirtualCranRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Conda repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Conda+Repositories#CondaRepositories-VirtualRepositories).
+        Creates a virtual Cran repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/CRAN+Repositories#CRANRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_conda = artifactory.VirtualCondaRepository("foo-conda",
+        foo_cran = artifactory.VirtualCranRepository("foo-cran",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-conda",
+            key="foo-cran",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualCondaRepository:VirtualCondaRepository foo-conda foo-conda
+         $ pulumi import artifactory:index/virtualCranRepository:VirtualCranRepository foo-cran foo-cran
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualCondaRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualCranRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualCondaRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualCranRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -585,15 +585,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualCondaRepositoryArgs.__new__(VirtualCondaRepositoryArgs)
+            __props__ = VirtualCranRepositoryArgs.__new__(VirtualCranRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -602,16 +602,16 @@
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
             __props__.__dict__["package_type"] = None
-        super(VirtualCondaRepository, __self__).__init__(
-            'artifactory:index/virtualCondaRepository:VirtualCondaRepository',
+        super(VirtualCranRepository, __self__).__init__(
+            'artifactory:index/virtualCranRepository:VirtualCranRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -624,17 +624,17 @@
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
             repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualCondaRepository':
+            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualCranRepository':
         """
-        Get an existing VirtualCondaRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualCranRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -655,30 +655,30 @@
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualCondaRepositoryState.__new__(_VirtualCondaRepositoryState)
+        __props__ = _VirtualCranRepositoryState.__new__(_VirtualCranRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
         __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
-        return VirtualCondaRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualCranRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_cran_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_gitlfs_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualCranRepositoryArgs', 'VirtualCranRepository']
+__all__ = ['VirtualGitlfsRepositoryArgs', 'VirtualGitlfsRepository']
 
 @pulumi.input_type
-class VirtualCranRepositoryArgs:
+class VirtualGitlfsRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualCranRepository resource.
+        The set of arguments for constructing a VirtualGitlfsRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -43,15 +42,14 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         pulumi.set(__self__, "key", key)
         if artifactory_requests_can_retrieve_remote_artifacts is not None:
             pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
         if default_deployment_repo is not None:
             pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
@@ -66,16 +64,14 @@
             pulumi.set(__self__, "project_environments", project_environments)
         if project_key is not None:
             pulumi.set(__self__, "project_key", project_key)
         if repo_layout_ref is not None:
             pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
         if repositories is not None:
             pulumi.set(__self__, "repositories", repositories)
-        if retrieval_cache_period_seconds is not None:
-            pulumi.set(__self__, "retrieval_cache_period_seconds", retrieval_cache_period_seconds)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
         A mandatory identifier for the repository that must be unique. It cannot begin with a number or
         contain spaces or special characters.
@@ -209,45 +205,32 @@
         """
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
-    @property
-    @pulumi.getter(name="retrievalCachePeriodSeconds")
-    def retrieval_cache_period_seconds(self) -> Optional[pulumi.Input[int]]:
-        """
-        This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
-        """
-        return pulumi.get(self, "retrieval_cache_period_seconds")
-
-    @retrieval_cache_period_seconds.setter
-    def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "retrieval_cache_period_seconds", value)
-
 
 @pulumi.input_type
-class _VirtualCranRepositoryState:
+class _VirtualGitlfsRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None):
+                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualCranRepository resources.
+        Input properties used for looking up and filtering VirtualGitlfsRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -259,15 +242,14 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         if artifactory_requests_can_retrieve_remote_artifacts is not None:
             pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
         if default_deployment_repo is not None:
             pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -285,16 +267,14 @@
             pulumi.set(__self__, "project_environments", project_environments)
         if project_key is not None:
             pulumi.set(__self__, "project_key", project_key)
         if repo_layout_ref is not None:
             pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
         if repositories is not None:
             pulumi.set(__self__, "repositories", repositories)
-        if retrieval_cache_period_seconds is not None:
-            pulumi.set(__self__, "retrieval_cache_period_seconds", retrieval_cache_period_seconds)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
@@ -437,28 +417,16 @@
         """
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
-    @property
-    @pulumi.getter(name="retrievalCachePeriodSeconds")
-    def retrieval_cache_period_seconds(self) -> Optional[pulumi.Input[int]]:
-        """
-        This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
-        """
-        return pulumi.get(self, "retrieval_cache_period_seconds")
-
-    @retrieval_cache_period_seconds.setter
-    def retrieval_cache_period_seconds(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "retrieval_cache_period_seconds", value)
-
 
-class VirtualCranRepository(pulumi.CustomResource):
+class VirtualGitlfsRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -466,41 +434,40 @@
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Creates a virtual Cran repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/CRAN+Repositories#CRANRepositories-VirtualRepositories).
+        Creates a virtual Git LFS repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Git+LFS+Repositories#GitLFSRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_cran = artifactory.VirtualCranRepository("foo-cran",
+        foo_gitlfs = artifactory.VirtualGitlfsRepository("foo-gitlfs",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-cran",
+            key="foo-gitlfs",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualCranRepository:VirtualCranRepository foo-cran foo-cran
+         $ pulumi import artifactory:index/virtualGitlfsRepository:VirtualGitlfsRepository foo-gitlfs foo-gitlfs
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -516,56 +483,55 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualCranRepositoryArgs,
+                 args: VirtualGitlfsRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Cran repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/CRAN+Repositories#CRANRepositories-VirtualRepositories).
+        Creates a virtual Git LFS repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Git+LFS+Repositories#GitLFSRepositories-VirtualRepositories).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_cran = artifactory.VirtualCranRepository("foo-cran",
+        foo_gitlfs = artifactory.VirtualGitlfsRepository("foo-gitlfs",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-cran",
+            key="foo-gitlfs",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualCranRepository:VirtualCranRepository foo-cran foo-cran
+         $ pulumi import artifactory:index/virtualGitlfsRepository:VirtualGitlfsRepository foo-gitlfs foo-gitlfs
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualCranRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualGitlfsRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualCranRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualGitlfsRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -577,41 +543,39 @@
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualCranRepositoryArgs.__new__(VirtualCranRepositoryArgs)
+            __props__ = VirtualGitlfsRepositoryArgs.__new__(VirtualGitlfsRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
-            __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
             __props__.__dict__["package_type"] = None
-        super(VirtualCranRepository, __self__).__init__(
-            'artifactory:index/virtualCranRepository:VirtualCranRepository',
+        super(VirtualGitlfsRepository, __self__).__init__(
+            'artifactory:index/virtualGitlfsRepository:VirtualGitlfsRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -623,18 +587,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            retrieval_cache_period_seconds: Optional[pulumi.Input[int]] = None) -> 'VirtualCranRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualGitlfsRepository':
         """
-        Get an existing VirtualCranRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualGitlfsRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -651,34 +614,32 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[int] retrieval_cache_period_seconds: This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualCranRepositoryState.__new__(_VirtualCranRepositoryState)
+        __props__ = _VirtualGitlfsRepositoryState.__new__(_VirtualGitlfsRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        __props__.__dict__["retrieval_cache_period_seconds"] = retrieval_cache_period_seconds
-        return VirtualCranRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualGitlfsRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
@@ -773,15 +734,7 @@
     @pulumi.getter
     def repositories(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The effective list of actual repositories included in this virtual repository.
         """
         return pulumi.get(self, "repositories")
 
-    @property
-    @pulumi.getter(name="retrievalCachePeriodSeconds")
-    def retrieval_cache_period_seconds(self) -> pulumi.Output[Optional[int]]:
-        """
-        This value refers to the number of seconds to cache metadata files before checking for newer versions on aggregated repositories. A value of 0 indicates no caching.
-        """
-        return pulumi.get(self, "retrieval_cache_period_seconds")
-
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_debian_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_docker_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_gems_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_generic_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_gitlfs_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_pub_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualGitlfsRepositoryArgs', 'VirtualGitlfsRepository']
+__all__ = ['VirtualPubRepositoryArgs', 'VirtualPubRepository']
 
 @pulumi.input_type
-class VirtualGitlfsRepositoryArgs:
+class VirtualPubRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualGitlfsRepository resource.
+        The set of arguments for constructing a VirtualPubRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -207,30 +207,30 @@
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _VirtualGitlfsRepositoryState:
+class _VirtualPubRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualGitlfsRepository resources.
+        Input properties used for looking up and filtering VirtualPubRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -418,15 +418,15 @@
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
-class VirtualGitlfsRepository(pulumi.CustomResource):
+class VirtualPubRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -436,38 +436,38 @@
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Creates a virtual Git LFS repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Git+LFS+Repositories#GitLFSRepositories-VirtualRepositories).
+        Creates a virtual Pub repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Pub+Repositories#PubRepositories-SettingupaVirtualRepository).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_gitlfs = artifactory.VirtualGitlfsRepository("foo-gitlfs",
+        foo_pub = artifactory.VirtualPubRepository("foo-pub",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-gitlfs",
+            key="foo-pub",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualGitlfsRepository:VirtualGitlfsRepository foo-gitlfs foo-gitlfs
+         $ pulumi import artifactory:index/virtualPubRepository:VirtualPubRepository foo-pub foo-pub
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -488,50 +488,50 @@
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualGitlfsRepositoryArgs,
+                 args: VirtualPubRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Git LFS repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Git+LFS+Repositories#GitLFSRepositories-VirtualRepositories).
+        Creates a virtual Pub repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Pub+Repositories#PubRepositories-SettingupaVirtualRepository).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_gitlfs = artifactory.VirtualGitlfsRepository("foo-gitlfs",
+        foo_pub = artifactory.VirtualPubRepository("foo-pub",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-gitlfs",
+            key="foo-pub",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualGitlfsRepository:VirtualGitlfsRepository foo-gitlfs foo-gitlfs
+         $ pulumi import artifactory:index/virtualPubRepository:VirtualPubRepository foo-pub foo-pub
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualGitlfsRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualPubRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualGitlfsRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualPubRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -550,15 +550,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualGitlfsRepositoryArgs.__new__(VirtualGitlfsRepositoryArgs)
+            __props__ = VirtualPubRepositoryArgs.__new__(VirtualPubRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -566,16 +566,16 @@
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["package_type"] = None
-        super(VirtualGitlfsRepository, __self__).__init__(
-            'artifactory:index/virtualGitlfsRepository:VirtualGitlfsRepository',
+        super(VirtualPubRepository, __self__).__init__(
+            'artifactory:index/virtualPubRepository:VirtualPubRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -587,17 +587,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualGitlfsRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualPubRepository':
         """
-        Get an existing VirtualGitlfsRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualPubRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -617,29 +617,29 @@
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualGitlfsRepositoryState.__new__(_VirtualGitlfsRepositoryState)
+        __props__ = _VirtualPubRepositoryState.__new__(_VirtualPubRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        return VirtualGitlfsRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualPubRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_gradle_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_helm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_ivy_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_npm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_nuget_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_p2_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_pub_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_puppet_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualPubRepositoryArgs', 'VirtualPubRepository']
+__all__ = ['VirtualPuppetRepositoryArgs', 'VirtualPuppetRepository']
 
 @pulumi.input_type
-class VirtualPubRepositoryArgs:
+class VirtualPuppetRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualPubRepository resource.
+        The set of arguments for constructing a VirtualPuppetRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -207,30 +207,30 @@
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _VirtualPubRepositoryState:
+class _VirtualPuppetRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualPubRepository resources.
+        Input properties used for looking up and filtering VirtualPuppetRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -418,15 +418,15 @@
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
-class VirtualPubRepository(pulumi.CustomResource):
+class VirtualPuppetRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -436,38 +436,38 @@
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Creates a virtual Pub repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Pub+Repositories#PubRepositories-SettingupaVirtualRepository).
+        Creates a virtual Puppet repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_pub = artifactory.VirtualPubRepository("foo-pub",
+        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-pub",
+            key="foo-puppet",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualPubRepository:VirtualPubRepository foo-pub foo-pub
+         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -488,50 +488,50 @@
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualPubRepositoryArgs,
+                 args: VirtualPuppetRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Pub repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Pub+Repositories#PubRepositories-SettingupaVirtualRepository).
+        Creates a virtual Puppet repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        foo_pub = artifactory.VirtualPubRepository("foo-pub",
+        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
             description="A test virtual repo",
             excludes_pattern="com/google/**",
             includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-pub",
+            key="foo-puppet",
             notes="Internal description",
             repositories=[])
         ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualPubRepository:VirtualPubRepository foo-pub foo-pub
+         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualPubRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualPuppetRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualPubRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualPuppetRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -550,15 +550,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualPubRepositoryArgs.__new__(VirtualPubRepositoryArgs)
+            __props__ = VirtualPuppetRepositoryArgs.__new__(VirtualPuppetRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -566,16 +566,16 @@
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["package_type"] = None
-        super(VirtualPubRepository, __self__).__init__(
-            'artifactory:index/virtualPubRepository:VirtualPubRepository',
+        super(VirtualPuppetRepository, __self__).__init__(
+            'artifactory:index/virtualPuppetRepository:VirtualPuppetRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -587,17 +587,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualPubRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualPuppetRepository':
         """
-        Get an existing VirtualPubRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualPuppetRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -617,29 +617,29 @@
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualPubRepositoryState.__new__(_VirtualPubRepositoryState)
+        __props__ = _VirtualPuppetRepositoryState.__new__(_VirtualPuppetRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        return VirtualPubRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualPuppetRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_puppet_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_swift_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualPuppetRepositoryArgs', 'VirtualPuppetRepository']
+__all__ = ['VirtualSwiftRepositoryArgs', 'VirtualSwiftRepository']
 
 @pulumi.input_type
-class VirtualPuppetRepositoryArgs:
+class VirtualSwiftRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualPuppetRepository resource.
+        The set of arguments for constructing a VirtualSwiftRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -207,30 +207,30 @@
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _VirtualPuppetRepositoryState:
+class _VirtualSwiftRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualPuppetRepository resources.
+        Input properties used for looking up and filtering VirtualSwiftRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -418,15 +418,15 @@
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
-class VirtualPuppetRepository(pulumi.CustomResource):
+class VirtualSwiftRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -436,38 +436,23 @@
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Creates a virtual Puppet repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-puppet",
-            notes="Internal description",
-            repositories=[])
-        ```
+        Creates a virtual Swift repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
+         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -488,50 +473,35 @@
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualPuppetRepositoryArgs,
+                 args: VirtualSwiftRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Puppet repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Puppet+Repositories#PuppetRepositories-VirtualPuppetRepository).
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        foo_puppet = artifactory.VirtualPuppetRepository("foo-puppet",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="foo-puppet",
-            notes="Internal description",
-            repositories=[])
-        ```
+        Creates a virtual Swift repository.
+        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualPuppetRepository:VirtualPuppetRepository foo-puppet foo-puppet
+         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualPuppetRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualSwiftRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualPuppetRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualSwiftRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -550,15 +520,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualPuppetRepositoryArgs.__new__(VirtualPuppetRepositoryArgs)
+            __props__ = VirtualSwiftRepositoryArgs.__new__(VirtualSwiftRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -566,16 +536,16 @@
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["package_type"] = None
-        super(VirtualPuppetRepository, __self__).__init__(
-            'artifactory:index/virtualPuppetRepository:VirtualPuppetRepository',
+        super(VirtualSwiftRepository, __self__).__init__(
+            'artifactory:index/virtualSwiftRepository:VirtualSwiftRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -587,17 +557,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualPuppetRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualSwiftRepository':
         """
-        Get an existing VirtualPuppetRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualSwiftRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -617,29 +587,29 @@
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualPuppetRepositoryState.__new__(_VirtualPuppetRepositoryState)
+        __props__ = _VirtualSwiftRepositoryState.__new__(_VirtualSwiftRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        return VirtualPuppetRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualSwiftRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_pypi_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_rpm_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_sbt_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_swift_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/virtual_terraform_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualSwiftRepositoryArgs', 'VirtualSwiftRepository']
+__all__ = ['VirtualTerraformRepositoryArgs', 'VirtualTerraformRepository']
 
 @pulumi.input_type
-class VirtualSwiftRepositoryArgs:
+class VirtualTerraformRepositoryArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        The set of arguments for constructing a VirtualSwiftRepository resource.
+        The set of arguments for constructing a VirtualTerraformRepository resource.
         :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
                contain spaces or special characters.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
@@ -207,30 +207,30 @@
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
 @pulumi.input_type
-class _VirtualSwiftRepositoryState:
+class _VirtualTerraformRepositoryState:
     def __init__(__self__, *,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  excludes_pattern: Optional[pulumi.Input[str]] = None,
                  includes_pattern: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  package_type: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering VirtualSwiftRepository resources.
+        Input properties used for looking up and filtering VirtualTerraformRepository resources.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
         :param pulumi.Input[str] description: Public description.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
@@ -418,15 +418,15 @@
         return pulumi.get(self, "repositories")
 
     @repositories.setter
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
 
-class VirtualSwiftRepository(pulumi.CustomResource):
+class VirtualTerraformRepository(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
                  default_deployment_repo: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
@@ -436,23 +436,35 @@
                  notes: Optional[pulumi.Input[str]] = None,
                  project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_key: Optional[pulumi.Input[str]] = None,
                  repo_layout_ref: Optional[pulumi.Input[str]] = None,
                  repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Creates a virtual Swift repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="terraform-remote",
+            notes="Internal description",
+            repositories=[])
+        ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
+         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
         :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
@@ -473,35 +485,47 @@
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualSwiftRepositoryArgs,
+                 args: VirtualTerraformRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a virtual Swift repository.
-        Official documentation can be found [here](https://www.jfrog.com/confluence/display/JFROG/Swift+Repositories#SwiftRepositories-VirtualRepositories).
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
+            description="A test virtual repo",
+            excludes_pattern="com/google/**",
+            includes_pattern="com/jfrog/**,cloud/jfrog/**",
+            key="terraform-remote",
+            notes="Internal description",
+            repositories=[])
+        ```
 
         ## Import
 
         Virtual repositories can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/virtualSwiftRepository:VirtualSwiftRepository foo-swift foo-swift
+         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
         ```
 
         :param str resource_name: The name of the resource.
-        :param VirtualSwiftRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param VirtualTerraformRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualSwiftRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VirtualTerraformRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -520,15 +544,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualSwiftRepositoryArgs.__new__(VirtualSwiftRepositoryArgs)
+            __props__ = VirtualTerraformRepositoryArgs.__new__(VirtualTerraformRepositoryArgs)
 
             __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
             __props__.__dict__["default_deployment_repo"] = default_deployment_repo
             __props__.__dict__["description"] = description
             __props__.__dict__["excludes_pattern"] = excludes_pattern
             __props__.__dict__["includes_pattern"] = includes_pattern
             if key is None and not opts.urn:
@@ -536,16 +560,16 @@
             __props__.__dict__["key"] = key
             __props__.__dict__["notes"] = notes
             __props__.__dict__["project_environments"] = project_environments
             __props__.__dict__["project_key"] = project_key
             __props__.__dict__["repo_layout_ref"] = repo_layout_ref
             __props__.__dict__["repositories"] = repositories
             __props__.__dict__["package_type"] = None
-        super(VirtualSwiftRepository, __self__).__init__(
-            'artifactory:index/virtualSwiftRepository:VirtualSwiftRepository',
+        super(VirtualTerraformRepository, __self__).__init__(
+            'artifactory:index/virtualTerraformRepository:VirtualTerraformRepository',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -557,17 +581,17 @@
             includes_pattern: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             package_type: Optional[pulumi.Input[str]] = None,
             project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             project_key: Optional[pulumi.Input[str]] = None,
             repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualSwiftRepository':
+            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualTerraformRepository':
         """
-        Get an existing VirtualSwiftRepository resource's state with the given name, id, and optional extra
+        Get an existing VirtualTerraformRepository resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
                another Artifactory instance.
@@ -587,29 +611,29 @@
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualSwiftRepositoryState.__new__(_VirtualSwiftRepositoryState)
+        __props__ = _VirtualTerraformRepositoryState.__new__(_VirtualTerraformRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
         __props__.__dict__["description"] = description
         __props__.__dict__["excludes_pattern"] = excludes_pattern
         __props__.__dict__["includes_pattern"] = includes_pattern
         __props__.__dict__["key"] = key
         __props__.__dict__["notes"] = notes
         __props__.__dict__["package_type"] = package_type
         __props__.__dict__["project_environments"] = project_environments
         __props__.__dict__["project_key"] = project_key
         __props__.__dict__["repo_layout_ref"] = repo_layout_ref
         __props__.__dict__["repositories"] = repositories
-        return VirtualSwiftRepository(resource_name, opts=opts, __props__=__props__)
+        return VirtualTerraformRepository(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
     def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
         another Artifactory instance.
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory/virtual_terraform_repository.py` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory/scoped_token.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,730 +5,645 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['VirtualTerraformRepositoryArgs', 'VirtualTerraformRepository']
+__all__ = ['ScopedTokenArgs', 'ScopedToken']
 
 @pulumi.input_type
-class VirtualTerraformRepositoryArgs:
+class ScopedTokenArgs:
     def __init__(__self__, *,
-                 key: pulumi.Input[str],
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        The set of arguments for constructing a VirtualTerraformRepository resource.
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        """
-        pulumi.set(__self__, "key", key)
-        if artifactory_requests_can_retrieve_remote_artifacts is not None:
-            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
-        if default_deployment_repo is not None:
-            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a ScopedToken resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
+        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        """
+        if audiences is not None:
+            pulumi.set(__self__, "audiences", audiences)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if excludes_pattern is not None:
-            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
-        if includes_pattern is not None:
-            pulumi.set(__self__, "includes_pattern", includes_pattern)
-        if notes is not None:
-            pulumi.set(__self__, "notes", notes)
-        if project_environments is not None:
-            pulumi.set(__self__, "project_environments", project_environments)
-        if project_key is not None:
-            pulumi.set(__self__, "project_key", project_key)
-        if repo_layout_ref is not None:
-            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
-        if repositories is not None:
-            pulumi.set(__self__, "repositories", repositories)
+        if expires_in is not None:
+            pulumi.set(__self__, "expires_in", expires_in)
+        if include_reference_token is not None:
+            pulumi.set(__self__, "include_reference_token", include_reference_token)
+        if refreshable is not None:
+            pulumi.set(__self__, "refreshable", refreshable)
+        if scopes is not None:
+            pulumi.set(__self__, "scopes", scopes)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def key(self) -> pulumi.Input[str]:
-        """
-        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-        contain spaces or special characters.
-        """
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key", value)
-
-    @property
-    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
-    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-        another Artifactory instance.
-        """
-        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
-
-    @artifactory_requests_can_retrieve_remote_artifacts.setter
-    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
-
-    @property
-    @pulumi.getter(name="defaultDeploymentRepo")
-    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
+    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Default repository to deploy artifacts.
+        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
         """
-        return pulumi.get(self, "default_deployment_repo")
+        return pulumi.get(self, "audiences")
 
-    @default_deployment_repo.setter
-    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_deployment_repo", value)
+    @audiences.setter
+    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "audiences", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Public description.
+        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="excludesPattern")
-    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="expiresIn")
+    def expires_in(self) -> Optional[pulumi.Input[int]]:
         """
-        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-        artifacts are excluded.
+        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
         """
-        return pulumi.get(self, "excludes_pattern")
+        return pulumi.get(self, "expires_in")
 
-    @excludes_pattern.setter
-    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "excludes_pattern", value)
+    @expires_in.setter
+    def expires_in(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "expires_in", value)
 
     @property
-    @pulumi.getter(name="includesPattern")
-    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="includeReferenceToken")
+    def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
         """
-        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        (Optional) Should a reference token also be created? Defaults to `false`
         """
-        return pulumi.get(self, "includes_pattern")
+        return pulumi.get(self, "include_reference_token")
 
-    @includes_pattern.setter
-    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "includes_pattern", value)
+    @include_reference_token.setter
+    def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "include_reference_token", value)
 
     @property
     @pulumi.getter
-    def notes(self) -> Optional[pulumi.Input[str]]:
+    def refreshable(self) -> Optional[pulumi.Input[bool]]:
         """
-        Internal description.
+        (Optional) Is this token refreshable? Defaults to `false`
         """
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "refreshable")
 
-    @notes.setter
-    def notes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "notes", value)
+    @refreshable.setter
+    def refreshable(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "refreshable", value)
 
     @property
-    @pulumi.getter(name="projectEnvironments")
-    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        """
-        return pulumi.get(self, "project_environments")
-
-    @project_environments.setter
-    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "project_environments", value)
-
-    @property
-    @pulumi.getter(name="projectKey")
-    def project_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        """
-        return pulumi.get(self, "project_key")
-
-    @project_key.setter
-    def project_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_key", value)
-
-    @property
-    @pulumi.getter(name="repoLayoutRef")
-    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Repository layout key for the local repository
+        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
         """
-        return pulumi.get(self, "repo_layout_ref")
+        return pulumi.get(self, "scopes")
 
-    @repo_layout_ref.setter
-    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "repo_layout_ref", value)
+    @scopes.setter
+    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "scopes", value)
 
     @property
     @pulumi.getter
-    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The effective list of actual repositories included in this virtual repository.
+        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
         """
-        return pulumi.get(self, "repositories")
+        return pulumi.get(self, "username")
 
-    @repositories.setter
-    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "repositories", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
-class _VirtualTerraformRepositoryState:
+class _ScopedTokenState:
     def __init__(__self__, *,
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 access_token: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 package_type: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        Input properties used for looking up and filtering VirtualTerraformRepository resources.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        """
-        if artifactory_requests_can_retrieve_remote_artifacts is not None:
-            pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
-        if default_deployment_repo is not None:
-            pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 expiry: Optional[pulumi.Input[int]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 issued_at: Optional[pulumi.Input[int]] = None,
+                 issuer: Optional[pulumi.Input[str]] = None,
+                 reference_token: Optional[pulumi.Input[str]] = None,
+                 refresh_token: Optional[pulumi.Input[str]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 subject: Optional[pulumi.Input[str]] = None,
+                 token_type: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering ScopedToken resources.
+        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        :param pulumi.Input[int] expiry: Returns the token expiry
+        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
+        :param pulumi.Input[int] issued_at: Returns the token issued at date/time
+        :param pulumi.Input[str] issuer: Returns the token issuer
+        :param pulumi.Input[str] reference_token: Returns the reference token to authenticate to Artifactory
+        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        :param pulumi.Input[str] subject: Returns the token type
+        :param pulumi.Input[str] token_type: Returns the token type
+        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
+        """
+        if access_token is not None:
+            pulumi.set(__self__, "access_token", access_token)
+        if audiences is not None:
+            pulumi.set(__self__, "audiences", audiences)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if excludes_pattern is not None:
-            pulumi.set(__self__, "excludes_pattern", excludes_pattern)
-        if includes_pattern is not None:
-            pulumi.set(__self__, "includes_pattern", includes_pattern)
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if notes is not None:
-            pulumi.set(__self__, "notes", notes)
-        if package_type is not None:
-            pulumi.set(__self__, "package_type", package_type)
-        if project_environments is not None:
-            pulumi.set(__self__, "project_environments", project_environments)
-        if project_key is not None:
-            pulumi.set(__self__, "project_key", project_key)
-        if repo_layout_ref is not None:
-            pulumi.set(__self__, "repo_layout_ref", repo_layout_ref)
-        if repositories is not None:
-            pulumi.set(__self__, "repositories", repositories)
-
-    @property
-    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
-    def artifactory_requests_can_retrieve_remote_artifacts(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-        another Artifactory instance.
-        """
-        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
-
-    @artifactory_requests_can_retrieve_remote_artifacts.setter
-    def artifactory_requests_can_retrieve_remote_artifacts(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "artifactory_requests_can_retrieve_remote_artifacts", value)
-
-    @property
-    @pulumi.getter(name="defaultDeploymentRepo")
-    def default_deployment_repo(self) -> Optional[pulumi.Input[str]]:
-        """
-        Default repository to deploy artifacts.
-        """
-        return pulumi.get(self, "default_deployment_repo")
-
-    @default_deployment_repo.setter
-    def default_deployment_repo(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_deployment_repo", value)
+        if expires_in is not None:
+            pulumi.set(__self__, "expires_in", expires_in)
+        if expiry is not None:
+            pulumi.set(__self__, "expiry", expiry)
+        if include_reference_token is not None:
+            pulumi.set(__self__, "include_reference_token", include_reference_token)
+        if issued_at is not None:
+            pulumi.set(__self__, "issued_at", issued_at)
+        if issuer is not None:
+            pulumi.set(__self__, "issuer", issuer)
+        if reference_token is not None:
+            pulumi.set(__self__, "reference_token", reference_token)
+        if refresh_token is not None:
+            pulumi.set(__self__, "refresh_token", refresh_token)
+        if refreshable is not None:
+            pulumi.set(__self__, "refreshable", refreshable)
+        if scopes is not None:
+            pulumi.set(__self__, "scopes", scopes)
+        if subject is not None:
+            pulumi.set(__self__, "subject", subject)
+        if token_type is not None:
+            pulumi.set(__self__, "token_type", token_type)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="accessToken")
+    def access_token(self) -> Optional[pulumi.Input[str]]:
+        """
+        Returns the access token to authenticate to Artifactory
+        """
+        return pulumi.get(self, "access_token")
+
+    @access_token.setter
+    def access_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access_token", value)
+
+    @property
+    @pulumi.getter
+    def audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        """
+        return pulumi.get(self, "audiences")
+
+    @audiences.setter
+    def audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "audiences", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Public description.
+        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="excludesPattern")
-    def excludes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="expiresIn")
+    def expires_in(self) -> Optional[pulumi.Input[int]]:
         """
-        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-        artifacts are excluded.
+        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
         """
-        return pulumi.get(self, "excludes_pattern")
+        return pulumi.get(self, "expires_in")
 
-    @excludes_pattern.setter
-    def excludes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "excludes_pattern", value)
+    @expires_in.setter
+    def expires_in(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "expires_in", value)
 
     @property
-    @pulumi.getter(name="includesPattern")
-    def includes_pattern(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def expiry(self) -> Optional[pulumi.Input[int]]:
         """
-        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        Returns the token expiry
         """
-        return pulumi.get(self, "includes_pattern")
+        return pulumi.get(self, "expiry")
 
-    @includes_pattern.setter
-    def includes_pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "includes_pattern", value)
+    @expiry.setter
+    def expiry(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "expiry", value)
 
     @property
-    @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="includeReferenceToken")
+    def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
         """
-        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-        contain spaces or special characters.
+        (Optional) Should a reference token also be created? Defaults to `false`
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "include_reference_token")
 
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
+    @include_reference_token.setter
+    def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "include_reference_token", value)
+
+    @property
+    @pulumi.getter(name="issuedAt")
+    def issued_at(self) -> Optional[pulumi.Input[int]]:
+        """
+        Returns the token issued at date/time
+        """
+        return pulumi.get(self, "issued_at")
+
+    @issued_at.setter
+    def issued_at(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "issued_at", value)
 
     @property
     @pulumi.getter
-    def notes(self) -> Optional[pulumi.Input[str]]:
+    def issuer(self) -> Optional[pulumi.Input[str]]:
         """
-        Internal description.
+        Returns the token issuer
         """
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "issuer")
 
-    @notes.setter
-    def notes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "notes", value)
+    @issuer.setter
+    def issuer(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "issuer", value)
 
     @property
-    @pulumi.getter(name="packageType")
-    def package_type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "package_type")
+    @pulumi.getter(name="referenceToken")
+    def reference_token(self) -> Optional[pulumi.Input[str]]:
+        """
+        Returns the reference token to authenticate to Artifactory
+        """
+        return pulumi.get(self, "reference_token")
 
-    @package_type.setter
-    def package_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "package_type", value)
+    @reference_token.setter
+    def reference_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "reference_token", value)
 
     @property
-    @pulumi.getter(name="projectEnvironments")
-    def project_environments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="refreshToken")
+    def refresh_token(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "refresh_token")
+
+    @refresh_token.setter
+    def refresh_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "refresh_token", value)
+
+    @property
+    @pulumi.getter
+    def refreshable(self) -> Optional[pulumi.Input[bool]]:
         """
-        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        (Optional) Is this token refreshable? Defaults to `false`
         """
-        return pulumi.get(self, "project_environments")
+        return pulumi.get(self, "refreshable")
 
-    @project_environments.setter
-    def project_environments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "project_environments", value)
+    @refreshable.setter
+    def refreshable(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "refreshable", value)
 
     @property
-    @pulumi.getter(name="projectKey")
-    def project_key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
         """
-        return pulumi.get(self, "project_key")
+        return pulumi.get(self, "scopes")
 
-    @project_key.setter
-    def project_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_key", value)
+    @scopes.setter
+    def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "scopes", value)
 
     @property
-    @pulumi.getter(name="repoLayoutRef")
-    def repo_layout_ref(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def subject(self) -> Optional[pulumi.Input[str]]:
         """
-        Repository layout key for the local repository
+        Returns the token type
         """
-        return pulumi.get(self, "repo_layout_ref")
+        return pulumi.get(self, "subject")
 
-    @repo_layout_ref.setter
-    def repo_layout_ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "repo_layout_ref", value)
+    @subject.setter
+    def subject(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="tokenType")
+    def token_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Returns the token type
+        """
+        return pulumi.get(self, "token_type")
+
+    @token_type.setter
+    def token_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token_type", value)
 
     @property
     @pulumi.getter
-    def repositories(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The effective list of actual repositories included in this virtual repository.
+        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
         """
-        return pulumi.get(self, "repositories")
+        return pulumi.get(self, "username")
 
-    @repositories.setter
-    def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "repositories", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
-class VirtualTerraformRepository(pulumi.CustomResource):
+class ScopedToken(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="terraform-remote",
-            notes="Internal description",
-            repositories=[])
-        ```
-
         ## Import
 
-        Virtual repositories can be imported using their name, e.g.
-
-        ```sh
-         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
-        ```
+        Artifactory **does not** retain scoped tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
+        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: VirtualTerraformRepositoryArgs,
+                 args: Optional[ScopedTokenArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_artifactory as artifactory
-
-        terraform_virtual = artifactory.VirtualTerraformRepository("terraform-virtual",
-            description="A test virtual repo",
-            excludes_pattern="com/google/**",
-            includes_pattern="com/jfrog/**,cloud/jfrog/**",
-            key="terraform-remote",
-            notes="Internal description",
-            repositories=[])
-        ```
-
         ## Import
 
-        Virtual repositories can be imported using their name, e.g.
-
-        ```sh
-         $ pulumi import artifactory:index/virtualTerraformRepository:VirtualTerraformRepository terraform-virtual terraform-remote
-        ```
+        Artifactory **does not** retain scoped tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
-        :param VirtualTerraformRepositoryArgs args: The arguments to use to populate this resource's properties.
+        :param ScopedTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(VirtualTerraformRepositoryArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ScopedTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-                 default_deployment_repo: Optional[pulumi.Input[str]] = None,
+                 audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 excludes_pattern: Optional[pulumi.Input[str]] = None,
-                 includes_pattern: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 notes: Optional[pulumi.Input[str]] = None,
-                 project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 project_key: Optional[pulumi.Input[str]] = None,
-                 repo_layout_ref: Optional[pulumi.Input[str]] = None,
-                 repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 expires_in: Optional[pulumi.Input[int]] = None,
+                 include_reference_token: Optional[pulumi.Input[bool]] = None,
+                 refreshable: Optional[pulumi.Input[bool]] = None,
+                 scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = VirtualTerraformRepositoryArgs.__new__(VirtualTerraformRepositoryArgs)
+            __props__ = ScopedTokenArgs.__new__(ScopedTokenArgs)
 
-            __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
-            __props__.__dict__["default_deployment_repo"] = default_deployment_repo
+            __props__.__dict__["audiences"] = audiences
             __props__.__dict__["description"] = description
-            __props__.__dict__["excludes_pattern"] = excludes_pattern
-            __props__.__dict__["includes_pattern"] = includes_pattern
-            if key is None and not opts.urn:
-                raise TypeError("Missing required property 'key'")
-            __props__.__dict__["key"] = key
-            __props__.__dict__["notes"] = notes
-            __props__.__dict__["project_environments"] = project_environments
-            __props__.__dict__["project_key"] = project_key
-            __props__.__dict__["repo_layout_ref"] = repo_layout_ref
-            __props__.__dict__["repositories"] = repositories
-            __props__.__dict__["package_type"] = None
-        super(VirtualTerraformRepository, __self__).__init__(
-            'artifactory:index/virtualTerraformRepository:VirtualTerraformRepository',
+            __props__.__dict__["expires_in"] = expires_in
+            __props__.__dict__["include_reference_token"] = include_reference_token
+            __props__.__dict__["refreshable"] = refreshable
+            __props__.__dict__["scopes"] = scopes
+            __props__.__dict__["username"] = username
+            __props__.__dict__["access_token"] = None
+            __props__.__dict__["expiry"] = None
+            __props__.__dict__["issued_at"] = None
+            __props__.__dict__["issuer"] = None
+            __props__.__dict__["reference_token"] = None
+            __props__.__dict__["refresh_token"] = None
+            __props__.__dict__["subject"] = None
+            __props__.__dict__["token_type"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "referenceToken", "refreshToken"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(ScopedToken, __self__).__init__(
+            'artifactory:index/scopedToken:ScopedToken',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            artifactory_requests_can_retrieve_remote_artifacts: Optional[pulumi.Input[bool]] = None,
-            default_deployment_repo: Optional[pulumi.Input[str]] = None,
+            access_token: Optional[pulumi.Input[str]] = None,
+            audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            excludes_pattern: Optional[pulumi.Input[str]] = None,
-            includes_pattern: Optional[pulumi.Input[str]] = None,
-            key: Optional[pulumi.Input[str]] = None,
-            notes: Optional[pulumi.Input[str]] = None,
-            package_type: Optional[pulumi.Input[str]] = None,
-            project_environments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            project_key: Optional[pulumi.Input[str]] = None,
-            repo_layout_ref: Optional[pulumi.Input[str]] = None,
-            repositories: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'VirtualTerraformRepository':
+            expires_in: Optional[pulumi.Input[int]] = None,
+            expiry: Optional[pulumi.Input[int]] = None,
+            include_reference_token: Optional[pulumi.Input[bool]] = None,
+            issued_at: Optional[pulumi.Input[int]] = None,
+            issuer: Optional[pulumi.Input[str]] = None,
+            reference_token: Optional[pulumi.Input[str]] = None,
+            refresh_token: Optional[pulumi.Input[str]] = None,
+            refreshable: Optional[pulumi.Input[bool]] = None,
+            scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            subject: Optional[pulumi.Input[str]] = None,
+            token_type: Optional[pulumi.Input[str]] = None,
+            username: Optional[pulumi.Input[str]] = None) -> 'ScopedToken':
         """
-        Get an existing VirtualTerraformRepository resource's state with the given name, id, and optional extra
+        Get an existing ScopedToken resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] artifactory_requests_can_retrieve_remote_artifacts: Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-               another Artifactory instance.
-        :param pulumi.Input[str] default_deployment_repo: Default repository to deploy artifacts.
-        :param pulumi.Input[str] description: Public description.
-        :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-               artifacts are excluded.
-        :param pulumi.Input[str] includes_pattern: List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-               used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
-        :param pulumi.Input[str] key: A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-               contain spaces or special characters.
-        :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-               Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-               attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-               be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
-        :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-               assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
-        :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
+        :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
+        :param pulumi.Input[str] description: (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
+        :param pulumi.Input[int] expires_in: (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
+        :param pulumi.Input[int] expiry: Returns the token expiry
+        :param pulumi.Input[bool] include_reference_token: (Optional) Should a reference token also be created? Defaults to `false`
+        :param pulumi.Input[int] issued_at: Returns the token issued at date/time
+        :param pulumi.Input[str] issuer: Returns the token issuer
+        :param pulumi.Input[str] reference_token: Returns the reference token to authenticate to Artifactory
+        :param pulumi.Input[bool] refreshable: (Optional) Is this token refreshable? Defaults to `false`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
+        :param pulumi.Input[str] subject: Returns the token type
+        :param pulumi.Input[str] token_type: Returns the token type
+        :param pulumi.Input[str] username: (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _VirtualTerraformRepositoryState.__new__(_VirtualTerraformRepositoryState)
+        __props__ = _ScopedTokenState.__new__(_ScopedTokenState)
 
-        __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
-        __props__.__dict__["default_deployment_repo"] = default_deployment_repo
+        __props__.__dict__["access_token"] = access_token
+        __props__.__dict__["audiences"] = audiences
         __props__.__dict__["description"] = description
-        __props__.__dict__["excludes_pattern"] = excludes_pattern
-        __props__.__dict__["includes_pattern"] = includes_pattern
-        __props__.__dict__["key"] = key
-        __props__.__dict__["notes"] = notes
-        __props__.__dict__["package_type"] = package_type
-        __props__.__dict__["project_environments"] = project_environments
-        __props__.__dict__["project_key"] = project_key
-        __props__.__dict__["repo_layout_ref"] = repo_layout_ref
-        __props__.__dict__["repositories"] = repositories
-        return VirtualTerraformRepository(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["expires_in"] = expires_in
+        __props__.__dict__["expiry"] = expiry
+        __props__.__dict__["include_reference_token"] = include_reference_token
+        __props__.__dict__["issued_at"] = issued_at
+        __props__.__dict__["issuer"] = issuer
+        __props__.__dict__["reference_token"] = reference_token
+        __props__.__dict__["refresh_token"] = refresh_token
+        __props__.__dict__["refreshable"] = refreshable
+        __props__.__dict__["scopes"] = scopes
+        __props__.__dict__["subject"] = subject
+        __props__.__dict__["token_type"] = token_type
+        __props__.__dict__["username"] = username
+        return ScopedToken(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="artifactoryRequestsCanRetrieveRemoteArtifacts")
-    def artifactory_requests_can_retrieve_remote_artifacts(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="accessToken")
+    def access_token(self) -> pulumi.Output[str]:
         """
-        Whether the virtual repository should search through remote repositories when trying to resolve an artifact requested by
-        another Artifactory instance.
+        Returns the access token to authenticate to Artifactory
         """
-        return pulumi.get(self, "artifactory_requests_can_retrieve_remote_artifacts")
+        return pulumi.get(self, "access_token")
 
     @property
-    @pulumi.getter(name="defaultDeploymentRepo")
-    def default_deployment_repo(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def audiences(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Default repository to deploy artifacts.
+        (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
         """
-        return pulumi.get(self, "default_deployment_repo")
+        return pulumi.get(self, "audiences")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Public description.
+        (Optional) Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="excludesPattern")
-    def excludes_pattern(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="expiresIn")
+    def expires_in(self) -> pulumi.Output[int]:
         """
-        List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*.By default no
-        artifacts are excluded.
+        (Optional) The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in `access.config.yaml`. See [API documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-RevokeTokenbyIDrevoketokenbyid) for details.
         """
-        return pulumi.get(self, "excludes_pattern")
+        return pulumi.get(self, "expires_in")
 
     @property
-    @pulumi.getter(name="includesPattern")
-    def includes_pattern(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def expiry(self) -> pulumi.Output[int]:
         """
-        List of comma-separated artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When
-        used, only artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
+        Returns the token expiry
         """
-        return pulumi.get(self, "includes_pattern")
+        return pulumi.get(self, "expiry")
 
     @property
-    @pulumi.getter
-    def key(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="includeReferenceToken")
+    def include_reference_token(self) -> pulumi.Output[Optional[bool]]:
         """
-        A mandatory identifier for the repository that must be unique. It cannot begin with a number or
-        contain spaces or special characters.
+        (Optional) Should a reference token also be created? Defaults to `false`
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "include_reference_token")
+
+    @property
+    @pulumi.getter(name="issuedAt")
+    def issued_at(self) -> pulumi.Output[int]:
+        """
+        Returns the token issued at date/time
+        """
+        return pulumi.get(self, "issued_at")
 
     @property
     @pulumi.getter
-    def notes(self) -> pulumi.Output[Optional[str]]:
+    def issuer(self) -> pulumi.Output[str]:
         """
-        Internal description.
+        Returns the token issuer
         """
-        return pulumi.get(self, "notes")
+        return pulumi.get(self, "issuer")
 
     @property
-    @pulumi.getter(name="packageType")
-    def package_type(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "package_type")
+    @pulumi.getter(name="referenceToken")
+    def reference_token(self) -> pulumi.Output[str]:
+        """
+        Returns the reference token to authenticate to Artifactory
+        """
+        return pulumi.get(self, "reference_token")
 
     @property
-    @pulumi.getter(name="projectEnvironments")
-    def project_environments(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="refreshToken")
+    def refresh_token(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "refresh_token")
+
+    @property
+    @pulumi.getter
+    def refreshable(self) -> pulumi.Output[Optional[bool]]:
+        """
+        (Optional) Is this token refreshable? Defaults to `false`
+        """
+        return pulumi.get(self, "refreshable")
+
+    @property
+    @pulumi.getter
+    def scopes(self) -> pulumi.Output[Sequence[str]]:
         """
-        Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
-        Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
-        attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
-        be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
+        (Optional) The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
         """
-        return pulumi.get(self, "project_environments")
+        return pulumi.get(self, "scopes")
 
     @property
-    @pulumi.getter(name="projectKey")
-    def project_key(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def subject(self) -> pulumi.Output[str]:
         """
-        Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
-        assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
+        Returns the token type
         """
-        return pulumi.get(self, "project_key")
+        return pulumi.get(self, "subject")
 
     @property
-    @pulumi.getter(name="repoLayoutRef")
-    def repo_layout_ref(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="tokenType")
+    def token_type(self) -> pulumi.Output[str]:
         """
-        Repository layout key for the local repository
+        Returns the token type
         """
-        return pulumi.get(self, "repo_layout_ref")
+        return pulumi.get(self, "token_type")
 
     @property
     @pulumi.getter
-    def repositories(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def username(self) -> pulumi.Output[Optional[str]]:
         """
-        The effective list of actual repositories included in this virtual repository.
+        (Optional) The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: `<service-id>/users/<username>`. Limited to 255 characters.
         """
-        return pulumi.get(self, "repositories")
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/PKG-INFO` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-artifactory
-Version: 3.4.0a1682378112
+Version: 3.4.0a1682710099
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-3.4.0a1682378112/pulumi_artifactory.egg-info/SOURCES.txt` & `pulumi_artifactory-3.4.0a1682710099/pulumi_artifactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.4.0a1682378112/setup.py` & `pulumi_artifactory-3.4.0a1682710099/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.4.0a1682378112"
-PLUGIN_VERSION = "3.4.0-alpha.1682378112+b647ac80"
+VERSION = "3.4.0a1682710099"
+PLUGIN_VERSION = "3.4.0-alpha.1682710099+7c304c82"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'artifactory', PLUGIN_VERSION])
         except OSError as error:
```

