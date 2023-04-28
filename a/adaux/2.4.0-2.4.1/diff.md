# Comparing `tmp/adaux-2.4.0.tar.gz` & `tmp/adaux-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.4.0.tar", last modified: Wed Apr 19 22:46:59 2023, max compression
+gzip compressed data, was "adaux-2.4.1.tar", last modified: Fri Apr 28 13:54:54 2023, max compression
```

## Comparing `adaux-2.4.0.tar` & `adaux-2.4.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.328294 adaux-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.4.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-19 22:46:59.332294 adaux-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-19 22:46:59.332294 adaux-2.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:58.924279 adaux-2.4.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.088285 adaux-2.4.0/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14267 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14303 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.140287 adaux-2.4.0/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-12 21:27:08.000000 adaux-2.4.0/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-12 23:18:12.000000 adaux-2.4.0/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    20260 2023-04-13 00:14:40.000000 adaux-2.4.0/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-12 23:43:59.000000 adaux-2.4.0/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.164288 adaux-2.4.0/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-12 15:47:50.000000 adaux-2.4.0/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15873 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.4.0/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.4.0/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-19 22:37:07.000000 adaux-2.4.0/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-12 09:55:20.000000 adaux-2.4.0/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.172288 adaux-2.4.0/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.172288 adaux-2.4.0/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.176288 adaux-2.4.0/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.184289 adaux-2.4.0/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.008282 adaux-2.4.0/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.192289 adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.196289 adaux-2.4.0/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.200289 adaux-2.4.0/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.204289 adaux-2.4.0/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.208289 adaux-2.4.0/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.248291 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.248291 adaux-2.4.0/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.252291 adaux-2.4.0/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.256291 adaux-2.4.0/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.256291 adaux-2.4.0/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.276292 adaux-2.4.0/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.284292 adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.288292 adaux-2.4.0/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.296293 adaux-2.4.0/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.296293 adaux-2.4.0/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.304293 adaux-2.4.0/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-12 15:47:50.000000 adaux-2.4.0/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.036283 adaux-2.4.0/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2530 2023-04-19 22:45:48.000000 adaux-2.4.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-12 23:05:47.000000 adaux-2.4.0/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.308293 adaux-2.4.0/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.312293 adaux-2.4.0/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.328294 adaux-2.4.0/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.328294 adaux-2.4.0/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.4.0/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:46:59.104286 adaux-2.4.0/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:45:47.000000 adaux-2.4.0/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 22:46:58.000000 adaux-2.4.0/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.555934 adaux-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-28 13:27:19.000000 adaux-2.4.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-28 13:54:54.555934 adaux-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-28 13:54:54.555934 adaux-2.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.447930 adaux-2.4.1/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.479931 adaux-2.4.1/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-28 13:34:29.000000 adaux-2.4.1/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-28 13:27:19.000000 adaux-2.4.1/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2023-04-28 13:27:19.000000 adaux-2.4.1/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14303 2023-04-28 13:27:19.000000 adaux-2.4.1/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.507933 adaux-2.4.1/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 13:27:19.000000 adaux-2.4.1/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-28 13:27:19.000000 adaux-2.4.1/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20260 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.511933 adaux-2.4.1/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15887 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.515933 adaux-2.4.1/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.515933 adaux-2.4.1/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.519933 adaux-2.4.1/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.519933 adaux-2.4.1/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.459931 adaux-2.4.1/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.519933 adaux-2.4.1/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.519933 adaux-2.4.1/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.523933 adaux-2.4.1/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.523933 adaux-2.4.1/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.523933 adaux-2.4.1/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.531933 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.531933 adaux-2.4.1/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.535934 adaux-2.4.1/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.535934 adaux-2.4.1/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.535934 adaux-2.4.1/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.535934 adaux-2.4.1/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.539934 adaux-2.4.1/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.539934 adaux-2.4.1/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.543934 adaux-2.4.1/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.543934 adaux-2.4.1/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.547934 adaux-2.4.1/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.547934 adaux-2.4.1/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.463931 adaux-2.4.1/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.547934 adaux-2.4.1/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.547934 adaux-2.4.1/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-04-28 13:51:13.000000 adaux-2.4.1/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.551934 adaux-2.4.1/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.551934 adaux-2.4.1/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.555934 adaux-2.4.1/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.555934 adaux-2.4.1/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-28 13:27:20.000000 adaux-2.4.1/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:54:54.487932 adaux-2.4.1/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-28 13:54:54.000000 adaux-2.4.1/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-04-28 13:54:54.000000 adaux-2.4.1/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:54:54.000000 adaux-2.4.1/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-28 13:54:54.000000 adaux-2.4.1/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:51:12.000000 adaux-2.4.1/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-28 13:54:54.000000 adaux-2.4.1/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 13:54:54.000000 adaux-2.4.1/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.4.0/LICENSE.txt` & `adaux-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/setup.cfg` & `adaux-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_base_parser.py` & `adaux-2.4.1/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_cli.py` & `adaux-2.4.1/source/adaux/_cli.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_cli_mixin.py` & `adaux-2.4.1/source/adaux/_cli_mixin.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_01_file_io_support.py` & `adaux-2.4.1/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_02_base.py` & `adaux-2.4.1/source/adaux/_components/_02_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_03_meta.py` & `adaux-2.4.1/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.4.1/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_05_project.py` & `adaux-2.4.1/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_06_dependency.py` & `adaux-2.4.1/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_07_package.py` & `adaux-2.4.1/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_08_pip.py` & `adaux-2.4.1/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_09_gitignore.py` & `adaux-2.4.1/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_10_gitlab.py` & `adaux-2.4.1/source/adaux/_components/_10_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_11_precommit.py` & `adaux-2.4.1/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_12_pylint.py` & `adaux-2.4.1/source/adaux/_components/_12_pylint.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_13_executable.py` & `adaux-2.4.1/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_14_mypy.py` & `adaux-2.4.1/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_15_pytest.py` & `adaux-2.4.1/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_17_docs.py` & `adaux-2.4.1/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_18_payload.py` & `adaux-2.4.1/source/adaux/_components/_18_payload.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_19_docker.py` & `adaux-2.4.1/source/adaux/_components/_19_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_20_ci.py` & `adaux-2.4.1/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_98_sentinel.py` & `adaux-2.4.1/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_99_all.py` & `adaux-2.4.1/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_aux_ci.py` & `adaux-2.4.1/source/adaux/_components/_aux_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/__init__.py` & `adaux-2.4.1/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/_base.py` & `adaux-2.4.1/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/_docker.py` & `adaux-2.4.1/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.4.1/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.4.1/source/adaux/_components/_payload/_docker_executors.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,16 +408,16 @@
         raise
 
 
 # try to download for caching (or reuse if already there)
 def check_and_pull_if_not_existent(
     remote_tag: str, local_tag: str, service: tp.Optional[str] = None
 ) -> None:
-    if local_tag and exists_locally(local_tag):
-        pass
+    if exists_locally(local_tag):
+        tag_image(local_tag, remote_tag)
     elif not exists_locally(remote_tag):
         cmd = ["docker", "pull", remote_tag]
         res = subprocess_run(cmd, check=False, capture_output=True)
         if res.returncode != 0:
             return
 
     tag_image(remote_tag, local_tag)
```

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/_python.py` & `adaux-2.4.1/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.4.1/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_create_badge.py` & `adaux-2.4.1/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_gitlab.py` & `adaux-2.4.1/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_parser.py` & `adaux-2.4.1/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_proto_namespace.py` & `adaux-2.4.1/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_tick.py` & `adaux-2.4.1/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/_todo.py` & `adaux-2.4.1/source/adaux/_todo.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
         self.data.setdefault(self.user, {})
 
     def dump(self) -> None:
         path = self.json_path
         with open(path, "w", encoding="utf-8") as f:
             json.dump(self.data, f, indent=4)
+            f.write("\n")
 
     def add_gitignore(self) -> None:
         gitignore = self.json_path.parent / ".gitignore"
         if gitignore.exists():
             self._print(".gitignore already exists", fg="green")
         else:
             with open(gitignore, "w", encoding="utf-8") as f:
```

### Comparing `adaux-2.4.0/source/adaux/_util.py` & `adaux-2.4.1/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.4.1/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.4.1/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -34,9 +34,10 @@
 
 ENV PYTHONPATH="{{ aux.project.source_dir }}"
 {% if aux.docs.framework == "sphinx" -%}
 CMD ["/bin/sh", "-c", "sphinx-apidoc -o {{ aux.docs.root }} {{ aux.project.module_dir }} &&\
     sphinx-build -M html {{ aux.docs.root }} devops/cache/docs{% if aux.docs.get('strict', True) == True %} -W{% endif %} &&\
     python devops/docs/postprocess_html.py devops/cache/docs/html/{{ aux.project.second_name }}.html"]
 {% elif aux.docs.framework == "mkdocs" -%}
+RUN git config --global --add safe.directory /home/container/workdir
 CMD ["mkdocs", "build", "-f", "{{ aux.docs.root }}/mkdocs.yml"]
 {%- endif %}
```

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 
 COPY --chown=container --from=build /home/container/.local/bin/ .local/bin/
 COPY --chown=container --from=build /home/container/.local/lib/ .local/lib/
 COPY --chown=container --from=build /home/container/.local/share/ .local/share/
 COPY --chown=container --from=build /home/container/.cache/pre-commit/ .cache/pre-commit/
 
 ENV PYTHONPATH='{{ aux.project.get("source_dir", "source") }}'
+RUN git config --global --add safe.directory /home/container/workdir
 CMD ["pre-commit", "run"]
```

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files 16% similar despite different names*

```diff
@@ -4,9 +4,8 @@
     {{ opts.service_name }}:
         {{ x.include_docker_build(aux, opts) }}
         {{ x.include_platform(aux) }}
         image: {{ opts.image_name }}
         volumes:
             - {{ aux.payload.docker_settings.project_dir }}:/home/container/workdir:rw
         working_dir: /home/container/workdir
-        command: [/bin/sh, -c,
-            "git config --global --add safe.directory `pwd` && pre-commit run --config=devops/pre-commit/config.yaml {% if "cmd" in opts %}{{ opts.cmd }}{% else %}--from-ref HEAD~1 --to-ref HEAD{% endif %}"]
+        command: ["pre-commit", "run", "--config=devops/pre-commit/config.yaml", {% if "cmd" in opts %}"{{ opts.cmd }}"{% else %}"--from-ref", "HEAD~1", "--to-ref", "HEAD"{% endif %}]
```

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.4.1/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.4.1/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/docs/postprocess_html.py` & `adaux-2.4.1/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.4.1/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.4.1/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.4.1/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.4.1/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 12 23:05:47 2023 UTC, .py size: 3046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4b39 3764 e60b 0000  o.......K97d....
+00000000: 6f0d 0d0a 0000 0000 b8c9 4b64 e60b 0000  o.........Kd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c04 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d07 5a07 0100 6402 6406 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6407 6509 6408 6401 6604  m.Z...d.e.d.d.f.
```

### Comparing `adaux-2.4.0/source/adaux/src/payload/python/functions.py` & `adaux-2.4.1/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.4.1/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.4.1/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.0/source/adaux.egg-info/SOURCES.txt` & `adaux-2.4.1/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

