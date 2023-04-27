# Comparing `tmp/nebari_workflow_controller-2023.4.2.tar.gz` & `tmp/nebari_workflow_controller-2023.4.3.tar.gz`

## Comparing `nebari_workflow_controller-2023.4.2.tar` & `nebari_workflow_controller-2023.4.3.tar`

### file list

```diff
@@ -1,24 +1,186 @@
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/nebari_workflow_controller/__init__.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/nebari_workflow_controller/__main__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/nebari_workflow_controller/_version.py
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/nebari_workflow_controller/app.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/nebari_workflow_controller/models.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_app.py
--rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/container_disallowed_conda_mount.yaml
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/container_disallowed_file_mount.yaml
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/container_empty_subPath.yaml
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/disallowed_volume.yaml
--rw-r--r--   0        0        0     8826 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/initContainer_disallowed_conda_mount.yaml
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/initContainer_disallowed_file_mount.yaml
--rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/initContainer_empty_subPath.yaml
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/argo_cli_hello_world.yaml
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/browser_hello_world.yaml
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/jupyterlab_pod.yaml
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/kubectl_malicious.yaml
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/LICENSE
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/README.md
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/__main__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/_version.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/app.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/models.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_app.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/README.md
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/convert_workflows.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_conda_mount.yaml
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_file_mount.yaml
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_empty_subPath.yaml
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/disallowed_volume.yaml
+-rw-r--r--   0        0        0     8826 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_conda_mount.yaml
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_file_mount.yaml
+-rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_empty_subPath.yaml
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/volumes-existing.yaml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/archive-location.yaml
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/argo_cli_hello_world.yaml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-artifacts.yaml
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-parameters-from-configmap.yaml
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-parameters.yaml
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-disable-archive.yaml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-gc-workflow.yaml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-passing-subpath.yaml
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-passing.yaml
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-path-placeholders.yaml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-repository-ref.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifactory-artifact.yaml
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/browser_hello_world.yaml
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/ci-output-artifact.yaml
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/ci.yaml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/coinflip-recursive.yaml
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/coinflip.yaml
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/colored-logs.yaml
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditional-artifacts.yaml
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditional-parameters.yaml
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditionals-complex.yaml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditionals.yaml
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/continue-on-fail.yaml
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/custom-metrics.yaml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemon-nginx.yaml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemon-step.yaml
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemoned-stateful-set-with-service.yaml
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-coinflip.yaml
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-conditional-artifacts.yaml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-conditional-parameters.yaml
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-continue-on-fail.yaml
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-custom-metrics.yaml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-daemon-task.yaml
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-diamond-steps.yaml
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-diamond.yaml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-disable-failFast.yaml
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-enhanced-depends.yaml
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-inline-workflow.yaml
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-multiroot.yaml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-nested.yaml
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-targets.yaml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-task-level-timeout.yaml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/data-transformations.yaml
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/default-pdb-support.yaml
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dns-config.yaml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-code-output-variable.yaml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-dag-level.yaml
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-slack.yaml
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-step-level.yaml
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-with-artifacts.yaml
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-with-param.yaml
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handlers.yaml
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-destructure-json.yaml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-reusing-verbose-snippets.yaml
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-tag-template-workflow.yaml
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/fibonacci-seq-conditional-param.yaml
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/forever.yaml
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/fun-with-gifs.yaml
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/gc-ttl.yaml
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-outputs.yaml
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters-from-configmap-referenced-as-local-variable.yaml
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters-from-configmap.yaml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters.yaml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/handle-large-output-results.yaml
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hdfs-artifact.yaml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-hybrid.yaml
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-windows.yaml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-world.yaml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/http-hello-world.yaml
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/http-success-condition.yaml
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/image-pull-secrets.yaml
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/influxdb-ci.yaml
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/init-container.yaml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-azure.yaml
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-gcs.yaml
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-git.yaml
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-http.yaml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-oss.yaml
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-raw.yaml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-s3.yaml
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/jupyterlab_pod.yaml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-jobs.yaml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-json-patch-workflow.yaml
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-orchestration.yaml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-owner-reference.yaml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-patch-basic.yaml
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-patch.yaml
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-resource-log-selector.yaml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-set-owner-reference.yaml
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-wait-wf.yaml
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/key-only-artifact.yaml
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/kubectl_malicious.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/label-value-from-workflow.yaml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/life-cycle-hooks-tmpl-level.yaml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/life-cycle-hooks-wf-level.yaml
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-arbitrary-sequential-steps.yaml
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-dag.yaml
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-maps.yaml
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-param-argument.yaml
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-param-result.yaml
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-sequence.yaml
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops.yaml
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/map-reduce.yaml
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/memoize-simple.yaml
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/nested-workflow.yaml
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/node-selector.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-azure.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-gcs.yaml
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-s3.yaml
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-parameter.yaml
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-limit.yaml
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested-dag.yaml
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested-workflow.yaml
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested.yaml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-template-limit.yaml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation-dag.yaml
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation-script.yaml
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation.yaml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-gc-strategy-with-label-selector.yaml
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-gc-strategy.yaml
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-metadata-wf-field.yaml
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-metadata.yaml
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-from-previous-step.yaml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-patch-wf-tmpl.yaml
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-patch.yaml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-yaml-patch.yaml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/recursive-for-loop.yaml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resource-delete-with-flags.yaml
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resource-flags.yaml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resubmit.yaml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-backoff.yaml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-conditional.yaml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-container-to-completion.yaml
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-container.yaml
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-on-error.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-script.yaml
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-with-steps.yaml
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-bash.yaml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-javascript.yaml
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-python.yaml
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/secrets.yaml
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar-dind.yaml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar-nginx.yaml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar.yaml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/status-reference.yaml
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/step-level-timeout.yaml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/steps-inline-workflow.yaml
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/steps.yaml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/suspend-template-outputs.yaml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/suspend-template.yaml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-mutex-tmpl-level.yaml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-mutex-wf-level.yaml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-tmpl-level.yaml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-wf-level.yaml
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/template-defaults.yaml
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/template-on-exit.yaml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/timeouts-step.yaml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/timeouts-workflow.yaml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/volumes-emptydir.yaml
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/volumes-pvc.yaml
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/webhdfs-input-output-artifacts.yaml
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/work-avoidance.yaml
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/workflow-of-workflows.yaml
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/LICENSE
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/README.md
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/PKG-INFO
```

### Comparing `nebari_workflow_controller-2023.4.2/.pre-commit-config.yaml` & `nebari_workflow_controller-2023.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/.github/workflows/release.yaml` & `nebari_workflow_controller-2023.4.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/nebari_workflow_controller/__init__.py` & `nebari_workflow_controller-2023.4.3/nebari_workflow_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/container_disallowed_conda_mount.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_conda_mount.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                         subPath: mocked_username
                     -   mountPath: /home/conda/global
                         name: conda-store
                         subPath: global
                     -   mountPath: /home/conda/global
                         name: conda-store
                         subPath: global
-                    -   mountPath: /home/conda/super-admin
+                    -   mountPath: /home/conda/super-admin  # disallowed
                         name: conda-store
                         subPath: super-admin
                     -   mountPath: /home/conda/analyst
                         name: conda-store
                         subPath: analyst
                     -   mountPath: /etc/dask
                         name: dask-etc
```

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/container_disallowed_file_mount.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_file_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/container_empty_subPath.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_empty_subPath.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/disallowed_volume.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/disallowed_volume.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/initContainer_disallowed_conda_mount.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_conda_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/initContainer_disallowed_file_mount.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_file_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/fail/initContainer_empty_subPath.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_empty_subPath.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/argo_cli_hello_world.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/argo_cli_hello_world.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/browser_hello_world.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/browser_hello_world.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/jupyterlab_pod.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/jupyterlab_pod.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/tests/test_data/requests/pass/kubectl_malicious.yaml` & `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/kubectl_malicious.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/.gitignore` & `nebari_workflow_controller-2023.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/LICENSE` & `nebari_workflow_controller-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/pyproject.toml` & `nebari_workflow_controller-2023.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.2/PKG-INFO` & `nebari_workflow_controller-2023.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari-workflow-controller
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: An admission controller for argo workflows in Nebari
 Project-URL: Documentation, https://github.com/nebari-dev/nebari-workflow-controller
 Project-URL: Source, https://github.com/nebari-dev/nebari-workflow-controller
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: admission-controller,argo-workflows,fastapi,kubernetes,nebari
```

