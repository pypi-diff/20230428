# Comparing `tmp/st4sd-runtime-core-2.0.0a9.dev2.tar.gz` & `tmp/st4sd-runtime-core-2.0.0a9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st4sd-runtime-core-2.0.0a9.dev2.tar", last modified: Fri Mar 10 15:17:45 2023, max compression
+gzip compressed data, was "dist/st4sd-runtime-core-2.0.0a9.dev3.tar", last modified: Fri Apr 28 14:42:18 2023, max compression
```

## Comparing `st4sd-runtime-core-2.0.0a9.dev2.tar` & `st4sd-runtime-core-2.0.0a9.dev3.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/.github/
--rw-rw-r--   0 root         (0) root         (0)      127 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/.github/dco.yml
--rw-rw-r--   0 root         (0) root         (0)     1799 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     8059 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/.travis.yml
--rw-rw-r--   0 root         (0) root         (0)       77 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/.whitesource
--rw-rw-r--   0 root         (0) root         (0)     3347 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 root         (0) root         (0)     2643 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/CONTRIBUTING.md
--rw-rw-r--   0 root         (0) root         (0)     2445 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)    10774 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/LICENSE.md
--rw-rw-r--   0 root         (0) root         (0)      439 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/MAINTAINERS.md
--rw-r--r--   0 root         (0) root         (0)     4097 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3334 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/
--rw-rw-r--   0 root         (0) root         (0)      180 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/creation_payload.json
--rwxrwxr-x   0 root         (0) root         (0)      292 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/skopeo_copy.sh
--rw-rw-r--   0 root         (0) root         (0)      635 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/st4sd-runtime-core-image.deploy
--rw-rw-r--   0 root         (0) root         (0)     1426 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/st4sd-runtime-core-multiarch.deploy
--rw-rw-r--   0 root         (0) root         (0)      291 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/st4sd-runtime-core-release-tag.deploy
--rwxrwxr-x   0 root         (0) root         (0)     2445 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/deploy/triggerExternalBuild.sh
--rw-rw-r--   0 root         (0) root         (0)     2442 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/py310.Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    35722 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/appenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/
--rw-rw-r--   0 root         (0) root         (0)      112 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2342 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/api.py
--rw-rw-r--   0 root         (0) root         (0)     2411 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     2891 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/context.py
--rw-rw-r--   0 root         (0) root         (0)      266 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/exit_codes.py
--rw-rw-r--   0 root         (0) root         (0)     1899 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/git.py
--rw-rw-r--   0 root         (0) root         (0)     5140 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/login.py
--rw-rw-r--   0 root         (0) root         (0)    18250 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/package.py
--rw-rw-r--   0 root         (0) root         (0)    31124 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/pvep_schema.jsonschema
--rw-rw-r--   0 root         (0) root         (0)     2300 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/stp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3003 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/codes.py
--rw-rw-r--   0 root         (0) root         (0)    82296 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/conf.py
--rw-rw-r--   0 root         (0) root         (0)   148053 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/data.py
--rw-rw-r--   0 root         (0) root         (0)    44154 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/errors.py
--rw-rw-r--   0 root         (0) root         (0)    57316 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   126138 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/cwl.py
--rw-rw-r--   0 root         (0) root         (0)    85741 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/dosini.py
--rw-rw-r--   0 root         (0) root         (0)   257676 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/flowir.py
--rw-rw-r--   0 root         (0) root         (0)   133899 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/
--rw-rw-r--   0 root         (0) root         (0)      683 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4236 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/hooks.py
--rw-rw-r--   0 root         (0) root         (0)    36110 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/interface.py
--rw-rw-r--   0 root         (0) root         (0)     2394 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/utils.py
--rw-rw-r--   0 root         (0) root         (0)     5562 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/interface.py
--rw-rw-r--   0 root         (0) root         (0)    67317 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package/
--rw-rw-r--   0 root         (0) root         (0)      544 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package/README.MD
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package/conf/
--rw-rw-r--   0 root         (0) root         (0)      376 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package/conf/flowir_package.yaml
--rw-rw-r--   0 root         (0) root         (0)     6144 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package.tar
--rw-rw-r--   0 root         (0) root         (0)      630 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/rewrite-rules.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      753 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/docker.py
--rw-rw-r--   0 root         (0) root         (0)   114992 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/k8s.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/localtask.py
--rw-rw-r--   0 root         (0) root         (0)   113109 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/lsf.py
--rwxrwxr-x   0 root         (0) root         (0)     1414 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/stage-out.sh
--rw-rw-r--   0 root         (0) root         (0)    13277 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/task_simulator.py
--rw-rw-r--   0 root         (0) root         (0)    34639 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backends.py
--rw-rw-r--   0 root         (0) root         (0)    23603 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backends_base.py
--rw-rw-r--   0 root         (0) root         (0)   118126 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/control.py
--rw-rw-r--   0 root         (0) root         (0)   104583 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/engine.py
--rw-rw-r--   0 root         (0) root         (0)     5429 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    26290 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/cwl.py
--rw-rw-r--   0 root         (0) root         (0)     9481 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/cwl_cmdline.py
--rw-rw-r--   0 root         (0) root         (0)     8089 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/js.py
--rw-rw-r--   0 root         (0) root         (0)    20080 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/monitor.py
--rw-rw-r--   0 root         (0) root         (0)    68147 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/optimizer.py
--rw-rw-r--   0 root         (0) root         (0)    34954 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/output.py
--rw-rw-r--   0 root         (0) root         (0)    45119 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/span.py
--rw-rw-r--   0 root         (0) root         (0)    35543 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/status.py
--rw-rw-r--   0 root         (0) root         (0)     5622 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3879 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/container_image_cache.py
--rw-rw-r--   0 root         (0) root         (0)     4089 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/rx.py
--rw-rw-r--   0 root         (0) root         (0)     5384 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/s3.py
--rw-rw-r--   0 root         (0) root         (0)    36584 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/service/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/service/__init__.py
--rw-rw-r--   0 root         (0) root         (0)   259382 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/service/db.py
--rw-rw-r--   0 root         (0) root         (0)     8206 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/service/errors.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/settings.py
--rw-rw-r--   0 root         (0) root         (0)     6441 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/
--rw-rw-r--   0 root         (0) root         (0)      104 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/README
--rw-rw-r--   0 root         (0) root         (0)      317 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    58393 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/data.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/fsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4097 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4567 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/requirement_files/
--rw-rw-r--   0 root         (0) root         (0)      133 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/requirement_files/requirements_base_3.7.txt
--rw-rw-r--   0 root         (0) root         (0)      423 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/requirement_files/requirements_base_3.txt
--rw-rw-r--   0 root         (0) root         (0)       18 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/requirement_files/requirements_deploy.txt
--rw-rw-r--   0 root         (0) root         (0)       94 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/requirement_files/requirements_lsf.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/
--rwxrwxr-x   0 root         (0) root         (0)     7054 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/ccommand.py
--rwxrwxr-x   0 root         (0) root         (0)    11413 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/cexecute.py
--rwxrwxr-x   0 root         (0) root         (0)     1239 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/checkpackage.py
--rwxrwxr-x   0 root         (0) root         (0)     4286 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/ctest.py
--rwxrwxr-x   0 root         (0) root         (0)     2567 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/ecreate.py
--rwxrwxr-x   0 root         (0) root         (0)     4196 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/eflowir.py
--rwxrwxr-x   0 root         (0) root         (0)     8094 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/einputs.py
--rwxrwxr-x   0 root         (0) root         (0)     8246 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/einspect.py
--rwxrwxr-x   0 root         (0) root         (0)   106886 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/elaunch.py
--rwxrwxr-x   0 root         (0) root         (0)    17228 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/ememo.py
--rwxrwxr-x   0 root         (0) root         (0)    46741 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/epatch-apply.py
--rwxrwxr-x   0 root         (0) root         (0)    33324 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/epatch.py
--rwxrwxr-x   0 root         (0) root         (0)    17371 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/etest.py
--rwxrwxr-x   0 root         (0) root         (0)    10419 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/ewrap.py
--rwxrwxr-x   0 root         (0) root         (0)      821 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/expstatus.sh
--rw-rw-r--   0 root         (0) root         (0)     3840 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/k8srun.py
--rwxrwxr-x   0 root         (0) root         (0)   106886 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/launchexperiment.py
--rwxrwxr-x   0 root         (0) root         (0)    14013 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/lsfsub.py
--rwxrwxr-x   0 root         (0) root         (0)      262 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/scripts/stp
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     4693 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:17:45.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10844 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/conftest.py
--rw-rw-r--   0 root         (0) root         (0)    11290 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/dont_test_cwl.py
--rw-rw-r--   0 root         (0) root         (0)     4541 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/reactive_testutils.py
--rw-rw-r--   0 root         (0) root         (0)    14765 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/saltcurve_paragon.py
--rw-rw-r--   0 root         (0) root         (0)    11225 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_array_variables.py
--rw-rw-r--   0 root         (0) root         (0)     6643 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_command.py
--rw-rw-r--   0 root         (0) root         (0)     7643 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_component.py
--rw-rw-r--   0 root         (0) root         (0)     2432 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_container_image_uri_manipulation.py
--rw-rw-r--   0 root         (0) root         (0)    44829 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_control.py
--rw-rw-r--   0 root         (0) root         (0)     4840 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_data.py
--rw-rw-r--   0 root         (0) root         (0)     5588 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_db.py
--rw-rw-r--   0 root         (0) root         (0)    40697 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_dosini.py
--rw-rw-r--   0 root         (0) root         (0)    35269 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_dowhile.py
--rw-rw-r--   0 root         (0) root         (0)    30930 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_engines.py
--rw-rw-r--   0 root         (0) root         (0)    57435 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_flowir.py
--rw-rw-r--   0 root         (0) root         (0)     3763 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_graph.py
--rw-rw-r--   0 root         (0) root         (0)     3286 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_identifier.py
--rw-rw-r--   0 root         (0) root         (0)    22435 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_interface.py
--rw-rw-r--   0 root         (0) root         (0)     6059 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_k8s.py
--rw-rw-r--   0 root         (0) root         (0)     2467 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_memoization.py
--rw-rw-r--   0 root         (0) root         (0)    13525 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_package_load.py
--rw-rw-r--   0 root         (0) root         (0)     1673 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_service.py
--rw-rw-r--   0 root         (0) root         (0)     2085 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     5739 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tests/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3119 2023-03-10 15:13:41.000000 st4sd-runtime-core-2.0.0a9.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/.github/
+-rw-rw-r--   0 root         (0) root         (0)      127 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.github/dco.yml
+-rw-rw-r--   0 root         (0) root         (0)     1799 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     8059 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)       77 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/.whitesource
+-rw-rw-r--   0 root         (0) root         (0)     3347 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 root         (0) root         (0)     2643 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/CONTRIBUTING.md
+-rw-rw-r--   0 root         (0) root         (0)     2445 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)    10774 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/LICENSE.md
+-rw-rw-r--   0 root         (0) root         (0)      439 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/MAINTAINERS.md
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3334 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/
+-rw-rw-r--   0 root         (0) root         (0)      180 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/creation_payload.json
+-rwxrwxr-x   0 root         (0) root         (0)      292 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/skopeo_copy.sh
+-rw-rw-r--   0 root         (0) root         (0)      635 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-image.deploy
+-rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-multiarch.deploy
+-rw-rw-r--   0 root         (0) root         (0)      291 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-release-tag.deploy
+-rwxrwxr-x   0 root         (0) root         (0)     2445 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/deploy/triggerExternalBuild.sh
+-rw-rw-r--   0 root         (0) root         (0)     2442 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/py310.Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    35722 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/appenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/
+-rw-rw-r--   0 root         (0) root         (0)      112 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2342 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2411 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     2891 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/context.py
+-rw-rw-r--   0 root         (0) root         (0)      266 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/exit_codes.py
+-rw-rw-r--   0 root         (0) root         (0)     1899 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/git.py
+-rw-rw-r--   0 root         (0) root         (0)     5140 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/login.py
+-rw-rw-r--   0 root         (0) root         (0)    18250 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/package.py
+-rw-rw-r--   0 root         (0) root         (0)    31124 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/pvep_schema.jsonschema
+-rw-rw-r--   0 root         (0) root         (0)     2300 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/stp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3003 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/codes.py
+-rw-rw-r--   0 root         (0) root         (0)    82296 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/conf.py
+-rw-rw-r--   0 root         (0) root         (0)   148053 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/data.py
+-rw-rw-r--   0 root         (0) root         (0)    44154 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/errors.py
+-rw-rw-r--   0 root         (0) root         (0)    57316 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   126138 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)    85741 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/dosini.py
+-rw-rw-r--   0 root         (0) root         (0)   257676 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/flowir.py
+-rw-rw-r--   0 root         (0) root         (0)   146796 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/
+-rw-rw-r--   0 root         (0) root         (0)      683 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4236 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/hooks.py
+-rw-rw-r--   0 root         (0) root         (0)    36110 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/interface.py
+-rw-rw-r--   0 root         (0) root         (0)     2394 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5562 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    67317 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/
+-rw-rw-r--   0 root         (0) root         (0)      544 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/README.MD
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/conf/
+-rw-rw-r--   0 root         (0) root         (0)      376 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/conf/flowir_package.yaml
+-rw-rw-r--   0 root         (0) root         (0)     6144 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package.tar
+-rw-rw-r--   0 root         (0) root         (0)      630 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/rewrite-rules.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      753 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/docker.py
+-rw-rw-r--   0 root         (0) root         (0)   114992 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/localtask.py
+-rw-rw-r--   0 root         (0) root         (0)   113109 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/lsf.py
+-rwxrwxr-x   0 root         (0) root         (0)     1414 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/stage-out.sh
+-rw-rw-r--   0 root         (0) root         (0)    13277 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/task_simulator.py
+-rw-rw-r--   0 root         (0) root         (0)    34639 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends.py
+-rw-rw-r--   0 root         (0) root         (0)    23603 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends_base.py
+-rw-rw-r--   0 root         (0) root         (0)   118126 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/control.py
+-rw-rw-r--   0 root         (0) root         (0)   104583 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/engine.py
+-rw-rw-r--   0 root         (0) root         (0)     5429 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    26290 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     9481 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl_cmdline.py
+-rw-rw-r--   0 root         (0) root         (0)     8089 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/js.py
+-rw-rw-r--   0 root         (0) root         (0)    20080 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/monitor.py
+-rw-rw-r--   0 root         (0) root         (0)    68147 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/optimizer.py
+-rw-rw-r--   0 root         (0) root         (0)    34954 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/output.py
+-rw-rw-r--   0 root         (0) root         (0)    45119 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/span.py
+-rw-rw-r--   0 root         (0) root         (0)    35543 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/status.py
+-rw-rw-r--   0 root         (0) root         (0)     5622 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3879 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/container_image_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4089 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/rx.py
+-rw-rw-r--   0 root         (0) root         (0)     5384 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/s3.py
+-rw-rw-r--   0 root         (0) root         (0)    36584 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)   259382 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/db.py
+-rw-rw-r--   0 root         (0) root         (0)     8206 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     6441 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/
+-rw-rw-r--   0 root         (0) root         (0)      104 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/README
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    58393 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/data.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/fsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/
+-rw-rw-r--   0 root         (0) root         (0)      133 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_base_3.7.txt
+-rw-rw-r--   0 root         (0) root         (0)      423 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_base_3.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_deploy.txt
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/requirement_files/requirements_lsf.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     7054 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ccommand.py
+-rwxrwxr-x   0 root         (0) root         (0)    11413 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/cexecute.py
+-rwxrwxr-x   0 root         (0) root         (0)     1239 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/checkpackage.py
+-rwxrwxr-x   0 root         (0) root         (0)     4286 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ctest.py
+-rwxrwxr-x   0 root         (0) root         (0)     2567 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ecreate.py
+-rwxrwxr-x   0 root         (0) root         (0)     4196 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/eflowir.py
+-rwxrwxr-x   0 root         (0) root         (0)     8094 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/einputs.py
+-rwxrwxr-x   0 root         (0) root         (0)     8246 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/einspect.py
+-rwxrwxr-x   0 root         (0) root         (0)   106886 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/elaunch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17228 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ememo.py
+-rwxrwxr-x   0 root         (0) root         (0)    46741 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch-apply.py
+-rwxrwxr-x   0 root         (0) root         (0)    33324 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch.py
+-rwxrwxr-x   0 root         (0) root         (0)    17371 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/etest.py
+-rwxrwxr-x   0 root         (0) root         (0)    10419 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/ewrap.py
+-rwxrwxr-x   0 root         (0) root         (0)      821 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/expstatus.sh
+-rw-rw-r--   0 root         (0) root         (0)     3840 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/k8srun.py
+-rwxrwxr-x   0 root         (0) root         (0)   106886 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/launchexperiment.py
+-rwxrwxr-x   0 root         (0) root         (0)    14013 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/lsfsub.py
+-rwxrwxr-x   0 root         (0) root         (0)      262 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/scripts/stp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     4693 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:42:18.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10844 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)    11290 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/dont_test_cwl.py
+-rw-rw-r--   0 root         (0) root         (0)     4541 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/reactive_testutils.py
+-rw-rw-r--   0 root         (0) root         (0)    14765 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/saltcurve_paragon.py
+-rw-rw-r--   0 root         (0) root         (0)    11225 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_array_variables.py
+-rw-rw-r--   0 root         (0) root         (0)     6643 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_command.py
+-rw-rw-r--   0 root         (0) root         (0)     7643 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_component.py
+-rw-rw-r--   0 root         (0) root         (0)     2432 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_container_image_uri_manipulation.py
+-rw-rw-r--   0 root         (0) root         (0)    44829 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_control.py
+-rw-rw-r--   0 root         (0) root         (0)     4840 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5588 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_db.py
+-rw-rw-r--   0 root         (0) root         (0)    40697 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_dosini.py
+-rw-rw-r--   0 root         (0) root         (0)    35269 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_dowhile.py
+-rw-rw-r--   0 root         (0) root         (0)    30930 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_engines.py
+-rw-rw-r--   0 root         (0) root         (0)    57435 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_flowir.py
+-rw-rw-r--   0 root         (0) root         (0)    17145 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_graph.py
+-rw-rw-r--   0 root         (0) root         (0)     3286 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_identifier.py
+-rw-rw-r--   0 root         (0) root         (0)    22435 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_interface.py
+-rw-rw-r--   0 root         (0) root         (0)     6059 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_k8s.py
+-rw-rw-r--   0 root         (0) root         (0)     2467 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_memoization.py
+-rw-rw-r--   0 root         (0) root         (0)    13525 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_package_load.py
+-rw-rw-r--   0 root         (0) root         (0)     1673 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_service.py
+-rw-rw-r--   0 root         (0) root         (0)     2085 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/test_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     5739 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tests/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3119 2023-04-28 14:38:42.000000 st4sd-runtime-core-2.0.0a9.dev3/tox.ini
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/.gitignore` & `st4sd-runtime-core-2.0.0a9.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/.travis.yml` & `st4sd-runtime-core-2.0.0a9.dev3/.travis.yml`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/CODE_OF_CONDUCT.md` & `st4sd-runtime-core-2.0.0a9.dev3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/CONTRIBUTING.md` & `st4sd-runtime-core-2.0.0a9.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/Dockerfile` & `st4sd-runtime-core-2.0.0a9.dev3/Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/LICENSE.md` & `st4sd-runtime-core-2.0.0a9.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/PKG-INFO` & `st4sd-runtime-core-2.0.0a9.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.0.0a9.dev2
+Version: 2.0.0a9.dev3
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/README.MD` & `st4sd-runtime-core-2.0.0a9.dev3/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/deploy/st4sd-runtime-core-image.deploy` & `st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-image.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/deploy/st4sd-runtime-core-multiarch.deploy` & `st4sd-runtime-core-2.0.0a9.dev3/deploy/st4sd-runtime-core-multiarch.deploy`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/deploy/triggerExternalBuild.sh` & `st4sd-runtime-core-2.0.0a9.dev3/deploy/triggerExternalBuild.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/py310.Dockerfile` & `st4sd-runtime-core-2.0.0a9.dev3/py310.Dockerfile`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/appenv.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/appenv.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/api.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/api.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/configuration.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/context.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/context.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/git.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/git.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/login.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/login.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/package.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/package.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/pvep_schema.jsonschema` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/pvep_schema.jsonschema`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/cli/stp.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/cli/stp.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/codes.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/codes.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/conf.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/conf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/data.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/errors.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/executors.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/executors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/cwl.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/dosini.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/frontends/flowir.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/frontends/flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/graph.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 import os.path
 import pprint
 import re
 import traceback
 import weakref
 from typing import (TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set,
                     Tuple, Union)
+from typing import cast
 
 import networkx
 import networkx.drawing.nx_agraph
 from future.utils import raise_with_traceback
 from past.builtins import cmp
 
+from collections import OrderedDict
 
 import experiment.appenv
 import experiment.model.conf
 import experiment.model.codes
 import experiment.model.errors
 import experiment.model.executors
 import experiment.model.frontends.flowir
@@ -1064,14 +1066,144 @@
                 raise ValueError("Cannot generate hash of %s: %s" % (type(obj), obj))
 
         md5 = hashlib.md5()
         md5.update(buf.encode('utf-8'))
 
         return md5.hexdigest()
 
+    def dsl_component_blueprint(self) -> Dict[str, Any]:
+        """Returns the component blueprint in the DSL of st4sd.
+
+        This is a WIP method and subject to changes.
+        """
+        comp_no_platform = self.workflowGraphRef().configurationForNode(
+            self.identification.identifier, raw=True,
+            omitDefault=True, is_primitive=True)
+        comp_with_platform = self.workflowGraphRef().configurationForNode(
+            self.identification.identifier, raw=True,
+            omitDefault=False, is_primitive=True)
+
+        comp_vars = OrderedDict(comp_no_platform.get('variables', {}))
+
+        all_var_refs = experiment.model.frontends.flowir.FlowIR.discover_references_to_variables(comp_with_platform)
+        parameters = [{'name': name} for name in sorted(set(all_var_refs).difference(comp_vars))]
+
+        command = comp_with_platform.get('command', {})
+
+        # VV: In the new DSL environment is either a dictionary of key: value items OR a reference to a parameter
+        if 'environment' in command:
+            # VV: We can generate a parameter, call it "env-vars" and assign the environment to it so that
+            # callers of this component can update the environment. If the component already has such a variable
+            # then just use the entire environment as is with no way to override it.
+
+            if any(filter(lambda x: x['name'] == 'env-vars', parameters)):
+                command['environment'] = self.environment
+            else:
+                parameters.append({'name': 'env-vars', 'default': self.environment})
+                command['environment'] = "$(env-vars)s"
+
+        # VV: In the new DSL the references are auto-generated from parameters whose value follows the
+        # <producer>[/fileref]:<method> schema. Need to auto-generate parameters for references and then rewrite
+        # the instances of references in the arguments (because that's the only place that they can appear) so that
+        # they look like parameter references (i.e. %(hello)s).
+        # Use param<index of reference> for the name of the auto-generated parameter.
+        # FIXME I cannot think of a way to fully handle a :copy reference - the developer may have used information
+        # encoded in the reference (e.g. the filename that gets copied into) in the arguments.
+        top_level_folders = self.workflowGraph.configuration.top_level_folders
+        app_deps = self.workflowGraph.configuration.get_application_dependencies()
+
+        arguments: str = command.get('arguments', '')
+
+        for (i, ref) in enumerate(comp_with_platform['references']):
+            new_param = f"param{i}"
+            parameters.append({'name': new_param})
+            if not arguments:
+                continue
+
+            # VV: Completely expand reference and identify whether it's to a Component or a directory (e.g. app-dep)
+            stageIndex, jobName, filename, method = experiment.model.frontends.flowir.FlowIR.ParseDataReferenceFull(
+                ref, index=self.identification.stageIndex,special_folders=top_level_folders,
+                application_dependencies=app_deps)
+            ref = experiment.model.frontends.flowir.FlowIR.compile_reference(jobName, filename, method, stageIndex)
+
+            dref = DataReference(ref)
+            arguments = arguments.replace(dref.absoluteReference, f'%({new_param})s')
+            if dref.stageIndex == self.identification.stageIndex:
+                arguments = arguments.replace(dref.relativeReference, f'%({new_param})s')
+
+        if arguments:
+            command['arguments'] = arguments
+
+        signature=OrderedDict( (('name', self.identification.identifier), ('parameters', parameters)) )
+        dsl = OrderedDict(( ('signature', signature), ))
+
+        if comp_vars:
+            dsl['variables'] = comp_vars
+
+        dsl['command'] = command
+
+        keep = ['resourceManager', 'resourceRequest', 'workflowAttributes']
+        for x in keep:
+            if x in comp_with_platform:
+                dsl[x] = comp_with_platform[x]
+
+        return dsl
+
+    def get_dsl_args(self, workflow_param_refs: Dict[str, str]) -> Dict[str, Any]:
+        """Returns the arguments for the DSL blueprint of this component
+
+        This is the dictionary for calling the "signature" of this component.
+
+        Arguments:
+            workflow_param_refs: A dictionary whose keys are references to external paths (e.g. app-deps, inputs, etc)
+              and values are names of the workflow parameter that the reference should be translated into.
+        """
+
+        comp_no_platform = self.workflowGraphRef().configurationForNode(
+            self.identification.identifier, raw=True,
+            omitDefault=True, is_primitive=True)
+        comp_with_platform = self.workflowGraphRef().configurationForNode(
+            self.identification.identifier, raw=True,
+            omitDefault=False, is_primitive=True)
+
+        own_vars = comp_no_platform.get('variables', {})
+
+        all_var_refs = experiment.model.frontends.flowir.FlowIR.discover_references_to_variables(comp_with_platform)
+
+        # VV: All variables that are not explicitly set by the component must be arguments of the parent workflow
+        my_args = {name: f"%({name})s" for name in sorted(set(all_var_refs).difference(own_vars))}
+
+        top_level_folders = self.workflowGraph.configuration.top_level_folders
+        app_deps = self.workflowGraph.configuration.get_application_dependencies()
+
+        # VV: References are just parameters called "param<Number>"
+        for (i, ref) in enumerate(comp_with_platform['references']):
+            new_param = f"param{i}"
+            # VV: Completely expand reference and identify whether it's to a Component or a directory (e.g. app-dep)
+            stageIndex, jobName, filename, method = experiment.model.frontends.flowir.FlowIR.ParseDataReferenceFull(
+                ref, index=self.identification.stageIndex, special_folders=top_level_folders,
+                application_dependencies=app_deps)
+            ref = experiment.model.frontends.flowir.FlowIR.compile_reference(jobName, filename, method, stageIndex)
+
+            if stageIndex is not None:
+                # VV: This is a dependency to a Component, rewrite the reference to <StepName>[/fileref]:method
+                dref = DataReference(ref)
+
+                step_ref = f"<{dref.producerIdentifier.identifier}>"
+                if dref.fileRef:
+                    step_ref += "/" + dref.fileRef
+                step_ref += ":" + dref.method
+                my_args[new_param] = step_ref
+            else:
+                # VV: this is a reference to a path that is not computed by other steps (app-dep, data, input, etc)
+                # this reference will have a corresponding workflow parameter.
+                my_args[new_param] = f"%({workflow_param_refs[ref]})s"
+
+        return my_args
+
     @property
     def memoization_info(self):
         if not self._memoization_info:
             self._memoization_info = self._compute_memoization_info(False)
         return copy.deepcopy(self._memoization_info)
 
     @property
@@ -1332,15 +1464,15 @@
 
     @property
     def identification(self):
         # type: () -> ComponentIdentifier
         return self._identification
 
     @property
-    def workflowGraph(self) -> experiment.model.graph.WorkflowGraph:
+    def workflowGraph(self) -> WorkflowGraph:
         '''Returns the experiment.model.graph.WorkflowGraph object the receiver is part of'''
 
         return self.workflowGraphRef()
 
     @property
     def configuration(self):
         # type: () -> DictFlowIRComponent
@@ -2103,14 +2235,155 @@
                 }
 
         if self.isPrimitive:
             self._graph = self._createPrimitiveGraph(inherit_graph)
         else:
             self._graph = self._createCompleteGraph(inherit_graph)
 
+    def to_dsl(self):
+        """Returns the entire DSL of the Workflowgrap (entrypoint, workflows, and components)
+
+        This is a WIP method and subject to changes.
+        """
+        graph = self.graph
+
+        """
+        entrypoint: # describes how to run this YAML file
+              entry-instance: the-identifier-of-a-class
+              execute: # the same as workflow.execute with the difference that there is always 1 step
+                # and the name of the step is always <entry-instance>
+                - target: "<entry-instance>"
+                  args: # Instantiate the class
+                    parameter-name: parameter value # see notes
+        """
+        platform_vars = self._concrete.get_platform_variables()[experiment.model.frontends.flowir.FlowIR.LabelGlobal]
+        workflow = self.dsl_workflow_blueprint()
+
+        main_args = OrderedDict()
+
+        for name in sorted(platform_vars):
+            main_args[name] = platform_vars[name]
+
+        top_level_folders = self.configuration.top_level_folders
+        app_deps = self.configuration.get_application_dependencies()
+
+        # VV: References that do not point to components are parameters of workflow
+        # Those that are pointing to `input` files should also be part of entrypoint.execute.args
+        # Those that point to app-deps/data, etc should not be part of entrypoint but should have a default value
+        #   (the reference string)
+        known_param_refs = set()
+
+        # VV: Must visit references in the correct order
+        for name in sorted(graph.nodes):
+            spec: ComponentSpecification = graph.nodes[name]['componentSpecification']
+            for ref in sorted(spec.rawDataReferences):
+
+                if ref in known_param_refs:
+                    continue
+
+                stageIndex, jobName, filename, method = experiment.model.frontends.flowir.FlowIR.ParseDataReferenceFull(
+                    ref, index=spec.identification.stageIndex, special_folders=top_level_folders,
+                    application_dependencies=app_deps)
+
+                if stageIndex is not None:
+                    # VV: This is a reference that points to a component, skip it
+                    continue
+
+                num_param = len(known_param_refs)
+
+                if jobName.split("/")[0] == "input":
+                    main_args[f'param{num_param}'] = ref
+
+                known_param_refs.add(ref)
+
+        entrypoint = OrderedDict(( ('entry-instance', 'main'), ))
+        entrypoint['execute'] = [
+                {
+                    "target": "<main>",
+                    "args": main_args
+                }
+            ]
+
+        dsl = OrderedDict()
+
+        dsl['entrypoint'] = entrypoint
+        dsl['workflows'] = [workflow]
+        dsl['components'] = [
+               cast(ComponentSpecification, graph.nodes[name]['componentSpecification']).dsl_component_blueprint()
+                    for name in networkx.topological_sort(graph)
+            ]
+
+        return dsl
+
+    def dsl_workflow_blueprint(self):
+        """Returns the workflow blueprint in the DSL of st4sd.
+
+        This is a WIP method and subject to changes.
+        """
+        platform_vars = self._concrete.get_platform_variables()[experiment.model.frontends.flowir.FlowIR.LabelGlobal]
+
+        # VV: The arguments to the workflow are platform variables
+        # TODO we need a way to handle stage variables - they are basically different variables which
+        # happen to occupy the same name as the global platform variables but only for a subset of components
+        # those that belong in that certain stage index
+        parameters = [
+            {'name': name, "default": platform_vars[name]} for name in sorted(platform_vars)
+        ]
+
+        graph = self.graph
+
+        top_level_folders = self.configuration.top_level_folders
+        app_deps = self.configuration.get_application_dependencies()
+
+        # VV: References that do not point to components are parameters of workflow
+        # Those that are pointing to `input` files should also be part of entrypoint.execute.args
+        # Those that point to app-deps/data, etc should not be part of entrypoint but should have a default value
+        #   (the reference string)
+        known_param_refs = dict()
+
+        # VV: Must visit references in the correct order
+        for name in sorted(graph.nodes):
+            spec: ComponentSpecification = graph.nodes[name]['componentSpecification']
+            for ref in sorted(spec.rawDataReferences):
+
+                if ref in known_param_refs:
+                    continue
+
+                stageIndex, jobName, filename, method = experiment.model.frontends.flowir.FlowIR.ParseDataReferenceFull(
+                    ref, index=spec.identification.stageIndex, special_folders=top_level_folders,
+                    application_dependencies=app_deps)
+
+                if stageIndex is not None:
+                    # VV: This is a reference that points to a component, skip it
+                    continue
+
+                num_param = len(known_param_refs)
+                param_name = f"param{num_param}"
+
+                if jobName.split("/")[0] != "input":
+                    parameters.append({'name': param_name, 'default': ref})
+                else:
+                    parameters.append({'name': param_name})
+
+                known_param_refs[ref] = param_name
+
+        signature = OrderedDict((('name', "main"), ('parameters', parameters)))
+        workflow = OrderedDict((('signature', signature),))
+
+        workflow['steps'] = OrderedDict( ((name, name) for name in networkx.topological_sort(graph)) )
+        workflow['execute'] = [
+            {
+                'target': f"<{name}>",
+                'args': cast(ComponentSpecification, graph.nodes[name]['componentSpecification'])
+                        .get_dsl_args(known_param_refs)
+            } for name in networkx.topological_sort(graph)
+        ]
+
+        return workflow
+
     @classmethod
     def graphFromExperimentInstanceDirectory(
             cls,
             experimentInstanceDir,  # type: ExperimentInstanceDirectory
             primitive=True,  # type: bool
             variable_substitute=True,  # type: bool
             systemvars=None,  # type: Optional[Dict[str, str]]
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/__init__.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/hooks.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/interface.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/hooks/utils.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/interface.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/model/storage.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/model/storage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package/README.MD` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package/README.MD`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/resources/Template.package.tar` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/resources/Template.package.tar`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/rewrite-rules.json` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/rewrite-rules.json`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/docker.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/docker.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/k8s.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/localtask.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/localtask.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/lsf.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/lsf.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/stage-out.sh` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/stage-out.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backend_interfaces/task_simulator.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backend_interfaces/task_simulator.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backends.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/backends_base.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/backends_base.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/control.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/engine.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/engine.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/errors.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/cwl.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/cwl_cmdline.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/cwl_cmdline.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/interpreters/js.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/interpreters/js.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/monitor.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/monitor.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/optimizer.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/optimizer.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/output.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/output.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/span.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/span.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/status.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/status.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/task.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/task.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/container_image_cache.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/container_image_cache.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/rx.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/rx.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/utilities/s3.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/utilities/s3.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/runtime/workflow.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/runtime/workflow.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/service/db.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/service/errors.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/service/errors.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/settings.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/test.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/test.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/data.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/experiment/utilities/fsearch.py` & `st4sd-runtime-core-2.0.0a9.dev3/python/experiment/utilities/fsearch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/PKG-INFO` & `st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st4sd-runtime-core
-Version: 2.0.0a9.dev2
+Version: 2.0.0a9.dev3
 Summary: A tool for creating and deploying computational experiments
 Home-page: https://github.com/st4sd/st4sd-runtime-core
 Author: Michael A. Johnston
 Author-email: michaelj@ie.ibm.com
 License: Apache 2.0
 Keywords: hpc kubernetes openshift lsf workflows experiments computational-chemistry simulation science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/python/st4sd_runtime_core.egg-info/SOURCES.txt` & `st4sd-runtime-core-2.0.0a9.dev3/python/st4sd_runtime_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/ccommand.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/ccommand.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/cexecute.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/cexecute.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/checkpackage.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/checkpackage.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/ctest.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/ctest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/ecreate.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/ecreate.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/eflowir.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/eflowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/einputs.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/einputs.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/einspect.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/einspect.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/elaunch.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/elaunch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/ememo.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/ememo.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/epatch-apply.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch-apply.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/epatch.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/epatch.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/etest.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/etest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/ewrap.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/ewrap.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/expstatus.sh` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/expstatus.sh`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/k8srun.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/k8srun.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/launchexperiment.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/launchexperiment.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/scripts/lsfsub.py` & `st4sd-runtime-core-2.0.0a9.dev3/scripts/lsfsub.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/setup.py` & `st4sd-runtime-core-2.0.0a9.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/conftest.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/dont_test_cwl.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/dont_test_cwl.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/reactive_testutils.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/reactive_testutils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/saltcurve_paragon.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/saltcurve_paragon.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_array_variables.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_array_variables.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_command.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_component.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_container_image_uri_manipulation.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_container_image_uri_manipulation.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_control.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_data.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_db.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_dosini.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_dosini.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_dowhile.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_dowhile.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_engines.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_flowir.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_flowir.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_identifier.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_interface.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_k8s.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_k8s.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_memoization.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_memoization.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_package_load.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_package_load.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_service.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/test_settings.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tests/utils.py` & `st4sd-runtime-core-2.0.0a9.dev3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `st4sd-runtime-core-2.0.0a9.dev2/tox.ini` & `st4sd-runtime-core-2.0.0a9.dev3/tox.ini`

 * *Files identical despite different names*

