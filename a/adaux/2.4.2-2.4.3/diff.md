# Comparing `tmp/adaux-2.4.2.tar.gz` & `tmp/adaux-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.4.2.tar", last modified: Fri Apr 28 14:33:38 2023, max compression
+gzip compressed data, was "adaux-2.4.3.tar", last modified: Fri Apr 28 18:02:47 2023, max compression
```

## Comparing `adaux-2.4.2.tar` & `adaux-2.4.3.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.742743 adaux-2.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-28 13:27:19.000000 adaux-2.4.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-28 14:33:38.742743 adaux-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-28 14:33:38.746743 adaux-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.642739 adaux-2.4.2/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.670740 adaux-2.4.2/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-28 14:27:06.000000 adaux-2.4.2/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-28 13:27:19.000000 adaux-2.4.2/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14267 2023-04-28 13:27:19.000000 adaux-2.4.2/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14303 2023-04-28 13:27:19.000000 adaux-2.4.2/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.694741 adaux-2.4.2/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 13:27:19.000000 adaux-2.4.2/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-28 13:27:19.000000 adaux-2.4.2/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    20260 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.702742 adaux-2.4.2/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15887 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-04-28 14:27:06.000000 adaux-2.4.2/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3414 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.702742 adaux-2.4.2/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.706742 adaux-2.4.2/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.706742 adaux-2.4.2/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.706742 adaux-2.4.2/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.654740 adaux-2.4.2/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.710742 adaux-2.4.2/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.710742 adaux-2.4.2/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.710742 adaux-2.4.2/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.714742 adaux-2.4.2/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.714742 adaux-2.4.2/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.722742 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.722742 adaux-2.4.2/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.722742 adaux-2.4.2/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.722742 adaux-2.4.2/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.726743 adaux-2.4.2/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.726743 adaux-2.4.2/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.726743 adaux-2.4.2/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.730743 adaux-2.4.2/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.730743 adaux-2.4.2/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.730743 adaux-2.4.2/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.734743 adaux-2.4.2/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.734743 adaux-2.4.2/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.658740 adaux-2.4.2/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.734743 adaux-2.4.2/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.738743 adaux-2.4.2/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2530 2023-04-28 14:33:09.000000 adaux-2.4.2/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.738743 adaux-2.4.2/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.738743 adaux-2.4.2/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.742743 adaux-2.4.2/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.742743 adaux-2.4.2/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-28 13:27:20.000000 adaux-2.4.2/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:33:38.678741 adaux-2.4.2/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-28 14:33:38.000000 adaux-2.4.2/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-28 14:33:38.000000 adaux-2.4.2/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:33:38.000000 adaux-2.4.2/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-28 14:33:38.000000 adaux-2.4.2/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:33:07.000000 adaux-2.4.2/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-28 14:33:38.000000 adaux-2.4.2/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 14:33:38.000000 adaux-2.4.2/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.078908 adaux-2.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-28 13:27:19.000000 adaux-2.4.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-28 18:02:47.078908 adaux-2.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-28 18:02:47.078908 adaux-2.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:46.970904 adaux-2.4.3/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.006906 adaux-2.4.3/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-28 17:55:38.000000 adaux-2.4.3/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-28 13:27:19.000000 adaux-2.4.3/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2023-04-28 13:27:19.000000 adaux-2.4.3/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14719 2023-04-28 17:55:38.000000 adaux-2.4.3/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.030907 adaux-2.4.3/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 13:27:19.000000 adaux-2.4.3/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-28 13:27:19.000000 adaux-2.4.3/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20260 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12673 2023-04-28 17:55:38.000000 adaux-2.4.3/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.034907 adaux-2.4.3/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15887 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-04-28 14:27:06.000000 adaux-2.4.3/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.038907 adaux-2.4.3/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.038907 adaux-2.4.3/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.042907 adaux-2.4.3/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.042907 adaux-2.4.3/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:46.986905 adaux-2.4.3/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.042907 adaux-2.4.3/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.042907 adaux-2.4.3/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.046907 adaux-2.4.3/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.046907 adaux-2.4.3/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.046907 adaux-2.4.3/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-04-28 17:55:38.000000 adaux-2.4.3/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.054907 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.054907 adaux-2.4.3/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.058908 adaux-2.4.3/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.058908 adaux-2.4.3/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.058908 adaux-2.4.3/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.058908 adaux-2.4.3/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.062908 adaux-2.4.3/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.062908 adaux-2.4.3/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.066908 adaux-2.4.3/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.066908 adaux-2.4.3/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.066908 adaux-2.4.3/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.070908 adaux-2.4.3/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:46.990905 adaux-2.4.3/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.070908 adaux-2.4.3/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.070908 adaux-2.4.3/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-04-28 18:02:12.000000 adaux-2.4.3/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.070908 adaux-2.4.3/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.074908 adaux-2.4.3/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.074908 adaux-2.4.3/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.078908 adaux-2.4.3/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-28 13:27:20.000000 adaux-2.4.3/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:02:47.010906 adaux-2.4.3/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-28 18:02:46.000000 adaux-2.4.3/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-04-28 18:02:46.000000 adaux-2.4.3/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 18:02:46.000000 adaux-2.4.3/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-28 18:02:46.000000 adaux-2.4.3/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 18:02:11.000000 adaux-2.4.3/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-28 18:02:46.000000 adaux-2.4.3/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 18:02:46.000000 adaux-2.4.3/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.4.2/LICENSE.txt` & `adaux-2.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/setup.cfg` & `adaux-2.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_base_parser.py` & `adaux-2.4.3/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_cli.py` & `adaux-2.4.3/source/adaux/_cli.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_cli_mixin.py` & `adaux-2.4.3/source/adaux/_cli_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,19 +146,28 @@
         release_message: str,
         major: bool = False,
         minor: bool = False,
         commit: bool = False,
     ) -> None:
         if major and minor:
             raise RuntimeError("cannot set major and minor tick at the same time!")
-        if len(release_message) < 16:
+        # empty mode, commit only
+        commit_with_release_msg = False
+        if len(release_message) == 0 and commit:
+            assert minor is False
+            assert major is False
+            commit_with_release_msg = True
+        elif len(release_message) < 16:
             raise RuntimeError("message cannot be shorter than 16 char")
-        ticker = TickSetter(self, release_message, major, minor)  # type: ignore
-        with self.extra():
-            ticker.bake()
+        with self.extra() as aux:
+            if commit_with_release_msg:
+                release_message = next(iter(aux.project.release_notes.values()))
+            ticker = TickSetter(self, release_message, major, minor)  # type: ignore
+            if not commit_with_release_msg:
+                ticker.bake()
             if commit:
                 ticker.commit()
 
     def release(
         self: "CliMixin", token: str, rerelease: bool = False
     ) -> tp.Tuple[bool, bool]:
         with self.extra():
```

### Comparing `adaux-2.4.2/source/adaux/_components/_01_file_io_support.py` & `adaux-2.4.3/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_02_base.py` & `adaux-2.4.3/source/adaux/_components/_02_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_03_meta.py` & `adaux-2.4.3/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.4.3/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_05_project.py` & `adaux-2.4.3/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_06_dependency.py` & `adaux-2.4.3/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_07_package.py` & `adaux-2.4.3/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_08_pip.py` & `adaux-2.4.3/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_09_gitignore.py` & `adaux-2.4.3/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_10_gitlab.py` & `adaux-2.4.3/source/adaux/_components/_10_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_11_precommit.py` & `adaux-2.4.3/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_12_pylint.py` & `adaux-2.4.3/source/adaux/_components/_12_pylint.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_13_executable.py` & `adaux-2.4.3/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_14_mypy.py` & `adaux-2.4.3/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_15_pytest.py` & `adaux-2.4.3/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_17_docs.py` & `adaux-2.4.3/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_18_payload.py` & `adaux-2.4.3/source/adaux/_components/_18_payload.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_19_docker.py` & `adaux-2.4.3/source/adaux/_components/_19_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_20_ci.py` & `adaux-2.4.3/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_98_sentinel.py` & `adaux-2.4.3/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_99_all.py` & `adaux-2.4.3/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_aux_ci.py` & `adaux-2.4.3/source/adaux/_components/_aux_ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,34 +334,31 @@
     def run_pipeline(self, show: bool = False) -> None:
         self.prune_unincluded(show=show)
         self.recurse(self.run_if_needed)
 
     def recurse(
         self,
         fct: tp.Callable[[T], None],
-        root_jobs: tp.Optional[tp.List[T]] = None,
-        seen: tp.Tuple[T, ...] = tuple(),
     ) -> None:
-        if root_jobs is None:
-            root_jobs = self.root_jobs
-        for job in root_jobs:
-            if job in seen:
-                continue
+        seen = []
+        open_jobs: tp.List[T] = self.root_jobs
+        all_vals = list(self.jobs.values())
+
+        while open_jobs:
+            job = open_jobs.pop(0)
+            assert job not in seen
             fct(job)
-            seen = seen + (job,)
+            seen.append(job)
 
-        todo = []
-        for job in root_jobs:
             for child in job.included_children:
-                if child not in todo:
-                    todo.append(child)
-        all_vals = list(self.jobs.values())
-        ordered = list(sorted(list(todo), key=all_vals.index))  # type: ignore
-        if ordered:
-            self.recurse(fct, ordered, seen)  # type: ignore
+                if child not in open_jobs:
+                    assert isinstance(child, T)
+                    open_jobs.append(child)
+
+            open_jobs = list(sorted(list(open_jobs), key=all_vals.index))
 
     def run_single(self, ident: str) -> None:
         for job in self.included_jobs:
             if job.ident != ident:
                 job.state.status = StateEnum.EXCLUDED
 
         self.env["run_single"] = True
```

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/__init__.py` & `adaux-2.4.3/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/_base.py` & `adaux-2.4.3/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/_docker.py` & `adaux-2.4.3/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.4.3/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.4.3/source/adaux/_components/_payload/_docker_executors.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/_python.py` & `adaux-2.4.3/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.4.3/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_create_badge.py` & `adaux-2.4.3/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_gitlab.py` & `adaux-2.4.3/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_parser.py` & `adaux-2.4.3/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_proto_namespace.py` & `adaux-2.4.3/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_tick.py` & `adaux-2.4.3/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_todo.py` & `adaux-2.4.3/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/_util.py` & `adaux-2.4.3/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.4.3/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.4.3/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.4.3/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.4.3/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/docs/postprocess_html.py` & `adaux-2.4.3/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.4.3/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.4.3/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.4.3/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.4.3/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/payload/python/functions.py` & `adaux-2.4.3/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.4.3/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.4.3/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.4.2/source/adaux.egg-info/SOURCES.txt` & `adaux-2.4.3/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

