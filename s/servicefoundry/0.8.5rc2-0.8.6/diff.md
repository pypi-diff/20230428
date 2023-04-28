# Comparing `tmp/servicefoundry-0.8.5rc2.tar.gz` & `tmp/servicefoundry-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.8.5rc2.tar", max compression
+gzip compressed data, was "servicefoundry-0.8.6.tar", max compression
```

## Comparing `servicefoundry-0.8.5rc2.tar` & `servicefoundry-0.8.6.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      672 2023-04-24 03:35:24.719930 servicefoundry-0.8.5rc2/README.md
--rw-r--r--   0        0        0     2119 2023-04-24 03:35:35.595909 servicefoundry-0.8.5rc2/pyproject.toml
--rw-r--r--   0        0        0     1266 2023-04-24 03:35:24.719930 servicefoundry-0.8.5rc2/servicefoundry/__init__.py
--rw-r--r--   0        0        0    36721 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4159 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      531 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1357 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6479 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6458 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2795 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3875 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3863 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      228 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     3032 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23939 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5624 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1028 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9608 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-04-24 03:35:24.723930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5276 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-04-24 03:35:24.727930 servicefoundry-0.8.5rc2/servicefoundry/version.py
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.8.5rc2/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/README.md
+-rw-r--r--   0        0        0     2116 2023-04-28 08:43:45.366068 servicefoundry-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1269 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    36574 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4159 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      531 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1357 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6479 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6458 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     2795 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     3875 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     3863 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      228 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     3032 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    23939 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     5624 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1028 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0     9608 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5196 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.8.6/PKG-INFO
```

### Comparing `servicefoundry-0.8.5rc2/README.md` & `servicefoundry-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/pyproject.toml` & `servicefoundry-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.8.5rc2"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.6"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/__init__.py` & `servicefoundry-0.8.6/servicefoundry/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from servicefoundry.auto_gen.models import (
     AppProtocol,
     CanaryStep,
     ConcurrencyPolicy,
     Protocol,
+    CapacityType,
 )
 from servicefoundry.core import login, logout
 from servicefoundry.lib.dao.application import (
     delete_application,
     get_application,
     list_applications,
     trigger_job,
@@ -31,15 +32,14 @@
     BasicAuthCreds,
     BlueGreen,
     Build,
     CPUUtilizationMetric,
     CUDAVersion,
     Canary,
     DockerFileBuild,
-    FileMount,
     GPU,
     GPUType,
     GitSource,
     HealthProbe,
     HttpProbe,
     HuggingfaceModelHub,
     Image,
```

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/auto_gen/models.py` & `servicefoundry-0.8.6/servicefoundry/auto_gen/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-04-06T11:36:11+00:00
+#   timestamp: 2023-04-27T20:26:32+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, confloat, conint, constr
@@ -82,35 +82,22 @@
     )
     command: Optional[Union[str, List[str]]] = Field(
         None,
         description="+label=Entrypoint Override\n+usage=Override the command to run when the container starts\nWhen deploying a Job, the command can be templatized by defining `params` and referencing them in command\nE.g. `python main.py --learning_rate {{learning_rate}}`",
     )
 
 
-class FileMount(BaseModel):
-    mount_path: str = Field(
-        ..., description="+usage=Path at which data is to be mounted"
-    )
-    is_base64_encoded: bool = Field(
-        False, description="+usage=Set this flag if your data values are base64 encoded"
-    )
-    data: Dict[str, str] = Field(
-        ...,
-        description="+usage=Data to be mounted. Each key will be the filename and the value will be the file content. Files will be mounted at mount_path",
-    )
-
-
 class GPU(BaseModel):
     type: str = Field(
         ...,
-        description="+label=Type\n+usage=Name of the Nvidia GPU. One of [K80, P4, P100, V100, T4, A10G, A100_40GB, A100_80GB]\nOne instance of the card contains the following amount of memory:\nK80: 12 GB\nP4: 8 GB\nP100: 16 GB\nV100: 16 GB\nT4: 16 GB\nA10G: 24 GB\nA100_40GB: 40GB\nA100_80GB: 80 GB",
+        description="+label=Type\n+usage=Name of the Nvidia GPU. One of [K80, P4, P100, V100, T4, A10G, A100_40GB, A100_80GB]\nOne instance of the card contains the following amount of memory -\nK80: 12 GB, P4: 8 GB, P100: 16 GB, V100: 16 GB, T4: 16 GB, A10G: 24 GB, A100_40GB: 40GB, A100_80GB: 80 GB",
     )
     count: conint(ge=1, le=16) = Field(
         1,
-        description="+label=Count\n+usage=Count of GPUs to provide to the application\nNote the exact count and max count available for a given GPU type depends on cloud provider and cluster type.\nK80: 1-16 on AWS EKS, 1-8 on GCP GKE Standard, NA on GCP GKE Autopilot\nP4: NA on AWS EKS, 1-4 on GCP GKE Standard, NA on GCP GKE Autopilot\nP100: NA on AWS EKS, 1-4 on GCP GKE Standard, NA on GCP GKE Autopilot\nV100: 1-8 on AWS EKS, 1-8 on GCP GKE Standard, NA on GCP GKE Autopilot\nT4: 1-8 on AWS EKS, 1-4 on GCP GKE Standard, exactly 1 or 2 or 4 on GCP GKE Autopilot\nA10G: 1-8 on AWS EKS, NA on GCP GKE Standard, NA on GCP GKE Autopilot\nA100_40GB: 1-8 on AWS EKS, 1-16 on GCP GKE Standard, exactly 1 or 2 or 4 or 8 or 16 on GCP GKE Autopilot\nA100_80GB: 1-8 on AWS EKS, 1-8 on GCP GKE Standard, NA on GCP GKE Autopilot",
+        description="+label=Count\n+usage=Count of GPUs to provide to the application\nNote the exact count and max count available for a given GPU type depends on cloud provider and cluster type.",
     )
 
 
 class GitSource(BaseModel):
     """
     +docs=Describes that we are using code stored in a git repository to build our image
     +label=Git Source
@@ -361,14 +348,28 @@
 
     type: constr(regex=r"^remote$") = Field(..., description="+value=remote")
     remote_uri: str = Field(
         ..., description="+docs=Remote repository URI\n+label=Remote URI"
     )
 
 
+class CapacityType(str, Enum):
+    """
+    +label=Capacity Type
+    +usage=Configure what type of nodes to run the app. By default no placement logic is applied.
+    "spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.
+    "spot" will strictly place the application on spot nodes.
+    "on_demand" will strictly place the application on on-demand nodes.
+    """
+
+    spot_fallback_on_demand = "spot_fallback_on_demand"
+    spot = "spot"
+    on_demand = "on_demand"
+
+
 class Resources(BaseModel):
     """
     +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
     To learn more you can go [here](https://docs.truefoundry.com/docs/resources)
     +icon=fa-microchip
     +label=Resources
     +usage=Set resource constraints for the application. [Docs](https://docs.truefoundry.com/docs/resources)
@@ -403,14 +404,18 @@
         None,
         description="+label=Instance family\n+usage=Instance family of the underlying machine to use. Multiple instance families can be supplied.\nThe workload is guaranteed to be scheduled on one of them.",
     )
     shared_memory_size: Optional[conint(ge=64, le=32000)] = Field(
         None,
         description="+label=Shared Memory Size\n+usage=Define the shared memory requirements for your workload. Machine learning libraries like Pytorch can use Shared Memory\nfor inter-process communication. If you use this, we will mount a `tmpfs` backed volume at the `/dev/shm` directory.\nAny usage will also count against the workload's memory limit (`resources.memory_limit`) along with your workload's memory usage.\nIf the overall usage goes above `resources.memory_limit` the user process may get killed.\nShared Memory Size cannot be more than the defined Memory Limit for the workload.",
     )
+    capacity_type: Optional[CapacityType] = Field(
+        None,
+        description='+label=Capacity Type\n+usage=Configure what type of nodes to run the app. By default no placement logic is applied.\n"spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.\n"spot" will strictly place the application on spot nodes.\n"on_demand" will strictly place the application on on-demand nodes.',
+    )
 
 
 class Rolling(BaseModel):
     """
     +docs=This strategy updates the pods in a rolling fashion such that a subset of the
     total pods are replaced with new version at one time.
     A commonly used strategy can be to have maxUnavailablePercentage close to 0 so that there
@@ -629,18 +634,14 @@
     env: Optional[Dict[str, str]] = Field(
         None,
         description="+label=Environment Variables\n+usage=Configure environment variables to be injected in the service. [Docs](https://docs.truefoundry.com/docs/env-variables)\n+icon=fa-globe\n+sort=8",
     )
     service_account: Optional[str] = Field(
         None, description="+usage=Service account that this workload should use"
     )
-    file_mounts: Optional[List[FileMount]] = Field(
-        None,
-        description="+usage=Files to be mounted to job pod(s). **Deprecated**\n+ignore\n+sort=10010",
-    )
     mounts: Optional[List[Union[SecretMount, StringDataMount, VolumeMount]]] = Field(
         None,
         description="+usage=Configure data to be mounted to job pod(s)\n+ignore\n+sort=10011",
     )
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
@@ -698,26 +699,26 @@
         description="+docs=Specify the ports you want the service to be exposed to\n+label=Ports (Ports to route customer traffic to)\n+icon=fa-plug\n+sort=4",
     )
     liveness_probe: Optional[HealthProbe] = None
     readiness_probe: Optional[HealthProbe] = None
     service_account: Optional[str] = Field(
         None, description="+usage=Service account that this workload should use"
     )
-    file_mounts: Optional[List[FileMount]] = Field(
-        None,
-        description="+usage=Files to be mounted to service pod(s). **Deprecated**\n+ignore\n+sort=10010",
-    )
     mounts: Optional[List[Union[SecretMount, StringDataMount, VolumeMount]]] = Field(
         None,
         description="+usage=Configure data to be mounted to service pod(s)\n+ignore\n+sort=10011",
     )
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
     rollout_strategy: Optional[Union[Rolling, Canary, BlueGreen]] = Field(
         None,
         description="+label=Rollout strategy\n+usage=Strategy to dictate how a rollout should happen when a new release for this service is made",
     )
+    allow_interception: bool = Field(
+        False,
+        description="+label=Allow intercepts\n+usage=Whether to allow intercepts to be applied for this service.\nThis would inject an additional sidecar in each pod of the service. Not recommended on production",
+    )
 
 
 class Application(BaseModel):
     __root__: Union[Service, Job, ModelDeployment]
```

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/builder/__init__.py` & `servicefoundry-0.8.6/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.8.6/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.8.6/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/builder/docker_service.py` & `servicefoundry-0.8.6/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/cli_main.py` & `servicefoundry-0.8.6/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.8.6/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/display_util.py` & `servicefoundry-0.8.6/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/cli/util.py` & `servicefoundry-0.8.6/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/__main__.py` & `servicefoundry-0.8.6/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/app.py` & `servicefoundry-0.8.6/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/build.py` & `servicefoundry-0.8.6/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.8.6/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.8.6/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/route.py` & `servicefoundry-0.8.6/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/service.py` & `servicefoundry-0.8.6/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/function_service/utils.py` & `servicefoundry-0.8.6/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/internal/experimental.py` & `servicefoundry-0.8.6/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/io/output_callback.py` & `servicefoundry-0.8.6/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.8.6/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.8.6/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.8.6/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.8.6/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.8.6/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.8.6/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.8.6/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.8.6/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.8.6/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.8.6/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.8.6/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.8.6/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.8.6/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.8.6/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.8.6/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/const.py` & `servicefoundry-0.8.6/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/dao/application.py` & `servicefoundry-0.8.6/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/dao/version.py` & `servicefoundry-0.8.6/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.8.6/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/exceptions.py` & `servicefoundry-0.8.6/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.8.6/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.8.6/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.8.6/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.8.6/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.8.6/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.8.6/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/messages.py` & `servicefoundry-0.8.6/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/model/entity.py` & `servicefoundry-0.8.6/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/session.py` & `servicefoundry-0.8.6/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/util.py` & `servicefoundry-0.8.6/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/lib/win32.py` & `servicefoundry-0.8.6/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/logger.py` & `servicefoundry-0.8.6/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.8.6/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.8.6/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/models.py` & `servicefoundry-0.8.6/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.8.6/servicefoundry/v2/lib/patched_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,19 +159,14 @@
 
 
 class Param(models.Param):
     class Config:
         extra = "forbid"
 
 
-class FileMount(models.FileMount):
-    class Config:
-        extra = "forbid"
-
-
 class CPUUtilizationMetric(models.CPUUtilizationMetric):
     class Config:
         extra = "forbid"
 
     type: Literal["cpu_utilization"] = "cpu_utilization"
```

### Comparing `servicefoundry-0.8.5rc2/servicefoundry/v2/lib/source.py` & `servicefoundry-0.8.6/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.5rc2/PKG-INFO` & `servicefoundry-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.8.5rc2
+Version: 0.8.6
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

