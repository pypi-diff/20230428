# Comparing `tmp/labgrid-23.1a1.tar.gz` & `tmp/labgrid-23.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgrid-23.1a1.tar", last modified: Thu Apr 27 11:28:04 2023, max compression
+gzip compressed data, was "labgrid-23.1a2.tar", last modified: Fri Apr 28 13:11:52 2023, max compression
```

## Comparing `labgrid-23.1a1.tar` & `labgrid-23.1a2.tar`

### file list

```diff
@@ -1,428 +1,428 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.641876 labgrid-23.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 11:27:51.000000 labgrid-23.1a1/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-27 11:27:51.000000 labgrid-23.1a1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/.crossbar/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 11:27:51.000000 labgrid-23.1a1/.crossbar/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-27 11:27:51.000000 labgrid-23.1a1/.crossbar/config-anonymous.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 11:27:51.000000 labgrid-23.1a1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 11:27:51.000000 labgrid-23.1a1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/workflows/build-and-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/workflows/push-pr-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/workflows/reusable-unit-tests-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/workflows/reusable-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-27 11:27:51.000000 labgrid-23.1a1/.github/workflows/scheduled-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-27 11:27:51.000000 labgrid-23.1a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 11:27:51.000000 labgrid-23.1a1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-04-27 11:27:51.000000 labgrid-23.1a1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 11:27:51.000000 labgrid-23.1a1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-04-27 11:27:51.000000 labgrid-23.1a1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-27 11:27:51.000000 labgrid-23.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-27 11:28:04.641876 labgrid-23.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-27 11:27:51.000000 labgrid-23.1a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/contrib/completion/
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/completion/labgrid-client.bash
--rwxr-xr-x   0 runner    (1001) docker     (123)     6195 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/coordinator-statsd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/sync-places.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/contrib/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/systemd/labgrid-coordinator.service
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/systemd/labgrid-exporter.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/contrib/systemd/sysusers.d/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/systemd/sysusers.d/labgrid.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/contrib/systemd/tmpfiles.d/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-27 11:27:51.000000 labgrid-23.1a1/contrib/systemd/tmpfiles.d/labgrid.conf
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-27 11:27:51.000000 labgrid-23.1a1/crossbar-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.597876 labgrid-23.1a1/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid-client
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid-exporter
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid-pytest
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid-suggest
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid.install
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid.manpages
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid.tmpfile
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid.triggers
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/labgrid.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-04-27 11:27:51.000000 labgrid-23.1a1/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    88737 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/design_decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/images/labgrid_logo_outline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/doc/man/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/man/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/man/device-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/man/exporter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/man.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/doc/res/
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/res/config_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/res/graphstrategy-via-nand.png
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/res/graphstrategy-via-nfs.png
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-04-27 11:27:51.000000 labgrid-23.1a1/doc/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/exporter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/exporter/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/staging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.589876 labgrid-23.1a1/dockerfiles/staging/client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/staging/client/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/client/.ssh/id_rsa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/staging/client/simple-test/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/client/simple-test/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/client/simple-test/remote_shell_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/staging/crossbar/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/crossbar/places_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/staging/dut/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/dut/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/dut/authorized_keys
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/dockerfiles/staging/exporter-conf/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 11:27:51.000000 labgrid-23.1a1/dockerfiles/staging/exporter-conf/exporter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.601876 labgrid-23.1a1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/barebox/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/local-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/test_barebox.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/test_bootchooser.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/test_sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/barebox/test_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/deditec-relais8/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/deditec-relais8/deditec.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/deditec-relais8/deditec_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/deditec-relais8/export-didicontrol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/deditec-relais8/import-dedicontrol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/docker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/docker/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/docker/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/docker/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/library/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/library/phytec.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/library/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/modbusrtu/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/modbusrtu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/modbusrtu/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/modbusrtu/test_modbusrtu_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/networkmanager/nm.env
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/networkmanager/nm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/power/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/power/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/power/power_example.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/pyvisa/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/pyvisa/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/pyvisa/pyvisa_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/qemu-networking/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/qemu-networking/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/qemu-networking/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/qemu-networking/qemunetworkstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/qemu-networking/test_qemu_networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.605876 labgrid-23.1a1/examples/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/remote/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/remote/test_barebox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/examples/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/shell/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/shell/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/shell/test_hwclock.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/shell/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/shell/test_rt.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/shell/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/examples/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/strategy/bareboxrebootstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/strategy/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/strategy/quartusstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/strategy/test_barebox_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/strategy/test_uboot_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/examples/sysfsgpio/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/sysfsgpio/export-gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/sysfsgpio/import-gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/sysfsgpio/sysfsgpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/sysfsgpio/sysfsgpio_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/examples/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usb/mass-storage-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usb/mxs-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usb/test_usb_mxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usb/test_usb_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/examples/usbpower/
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/examplestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/exports.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbpower/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/examples/usbsdmux/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbsdmux/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-27 11:27:51.000000 labgrid-23.1a1/examples/usbsdmux/test_sdmux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.609876 labgrid-23.1a1/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-04-27 11:27:51.000000 labgrid-23.1a1/helpers/labgrid-bound-connect
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.613876 labgrid-23.1a1/labgrid/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.613876 labgrid-23.1a1/labgrid/autoinstall/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/autoinstall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/autoinstall/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/consoleloggingreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.617876 labgrid-23.1a1/labgrid/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/bareboxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/commandmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/consoleexpectmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/dediprogflashdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/deditecrelaisdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/dfudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/dockerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/externalconsoledriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/fastbootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/filedigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/flashromdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/flashscriptdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/gpiodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/httpvideodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/lxaiobusdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/lxausbmuxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/manualswitchdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/modbusdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/modbusrtudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/networkinterfacedriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/onewiredriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/openocddriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.621876 labgrid-23.1a1/labgrid/driver/power/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/apc.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/digipower.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/digitalloggers_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/eaton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/eg_pms2_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/gude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/gude24.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/gude8031.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/gude8225.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/gude8316.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/netio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/netio_kshell.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/shelly_gen1.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/siglent.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/simplerest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/power/tplink.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/powerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/pyvisadriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/qemudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/quartushpsdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/resetdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/serialdigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/serialdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/shelldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/sigrokdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/smallubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/sshdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/ubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbaudiodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbhidrelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbsdmuxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbsdwiredriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbstoragedriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.621876 labgrid-23.1a1/labgrid/driver/usbtmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbtmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbtmc/keysight_dsox2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbtmc/tektronix_tds2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbtmcdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/usbvideodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/driver/xenadriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.621876 labgrid-23.1a1/labgrid/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/bootstrapprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/commandprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/consoleprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/digitaloutputprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/filesystemprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/filetransferprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/infoprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/linuxbootprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/mmioprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/powerprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/resetprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/protocol/videoprotocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.625876 labgrid-23.1a1/labgrid/pytestplugin/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/pytestplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/pytestplugin/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/pytestplugin/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/pytestplugin/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.625876 labgrid-23.1a1/labgrid/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/authenticator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81608 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32314 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/remote/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.629876 labgrid-23.1a1/labgrid/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/dediprogflasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/ethernetport.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/fastboot.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/flashrom.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/httpvideostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/lxaiobus.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/modbusrtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/networkservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/onewireport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/pyvisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/serialport.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/sigrok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/udev.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/xenamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/resource/ykushpowerport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/stepreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.629876 labgrid-23.1a1/labgrid/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/bareboxstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/dockerstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/graphstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/shellstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/strategy/ubootstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.629876 labgrid-23.1a1/labgrid/util/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.633876 labgrid-23.1a1/labgrid/util/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agents/deditec_relais8.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agents/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agents/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agents/sysfsgpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agents/usb_hid_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/agentwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/expect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/managedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/qmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.613876 labgrid-23.1a1/labgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-27 11:28:04.000000 labgrid-23.1a1/labgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-27 11:28:04.000000 labgrid-23.1a1/labgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:28:04.000000 labgrid-23.1a1/labgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-27 11:28:04.000000 labgrid-23.1a1/labgrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-27 11:28:04.000000 labgrid-23.1a1/labgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 11:28:04.000000 labgrid-23.1a1/labgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-27 11:27:51.000000 labgrid-23.1a1/labgrid_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.633876 labgrid-23.1a1/man/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-client.1
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-device-config.5
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-device-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-exporter.1
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-exporter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-pytest.7
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-pytest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-suggest.1
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-27 11:27:51.000000 labgrid-23.1a1/man/labgrid-suggest.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 11:27:51.000000 labgrid-23.1a1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-27 11:27:51.000000 labgrid-23.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:28:04.641876 labgrid-23.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:28:04.637876 labgrid-23.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_autoinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_bareboxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_crossbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_dediprogflasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_ethernetport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_externalconsoledriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_filedigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_flashrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_flashscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_graphstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_httpvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_lxaiobus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_manualswitchdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_modbusrtudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_onewire.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_openocd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_powerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_processwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_pyvisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_qemudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_sched.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_serialdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_serialport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_shelldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_sigrok.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_sispm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_sshdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_stepreporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_sysfsgpioagent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_tasmota.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_ubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_usbtmc.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_usbvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-27 11:27:51.000000 labgrid-23.1a1/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.777660 labgrid-23.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 13:11:41.000000 labgrid-23.1a2/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 13:11:41.000000 labgrid-23.1a2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.737660 labgrid-23.1a2/.crossbar/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 13:11:41.000000 labgrid-23.1a2/.crossbar/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 13:11:41.000000 labgrid-23.1a2/.crossbar/config-anonymous.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 13:11:41.000000 labgrid-23.1a2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 13:11:41.000000 labgrid-23.1a2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.737660 labgrid-23.1a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/build-and-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/push-pr-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/reusable-unit-tests-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/reusable-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 13:11:41.000000 labgrid-23.1a2/.github/workflows/scheduled-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-28 13:11:41.000000 labgrid-23.1a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 13:11:41.000000 labgrid-23.1a2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    28027 2023-04-28 13:11:41.000000 labgrid-23.1a2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 13:11:41.000000 labgrid-23.1a2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-04-28 13:11:41.000000 labgrid-23.1a2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 13:11:41.000000 labgrid-23.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-28 13:11:52.777660 labgrid-23.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-28 13:11:41.000000 labgrid-23.1a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/completion/
+-rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/completion/labgrid-client.bash
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6195 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/coordinator-statsd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/sync-places.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/labgrid-coordinator.service
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/labgrid-exporter.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/systemd/sysusers.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/sysusers.d/labgrid.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/contrib/systemd/tmpfiles.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 13:11:41.000000 labgrid-23.1a2/contrib/systemd/tmpfiles.d/labgrid.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 13:11:41.000000 labgrid-23.1a2/crossbar-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-client
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-exporter
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-pytest
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid-suggest
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.install
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.manpages
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.tmpfile
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.triggers
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/labgrid.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-04-28 13:11:41.000000 labgrid-23.1a2/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.741660 labgrid-23.1a2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88586 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/design_decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/images/labgrid_logo_outline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/doc/man/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man/device-config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man/exporter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/man.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/doc/res/
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/res/config_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/res/graphstrategy-via-nand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/res/graphstrategy-via-nfs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-04-28 13:11:41.000000 labgrid-23.1a2/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/exporter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/exporter/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.733660 labgrid-23.1a2/dockerfiles/staging/client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/client/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/client/.ssh/id_rsa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/client/simple-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/client/simple-test/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/client/simple-test/remote_shell_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/crossbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/crossbar/places_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/dut/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/dut/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/dut/authorized_keys
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/dockerfiles/staging/exporter-conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 13:11:41.000000 labgrid-23.1a2/dockerfiles/staging/exporter-conf/exporter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/examples/barebox/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/local-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_barebox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_bootchooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/barebox/test_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.745660 labgrid-23.1a2/examples/deditec-relais8/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/deditec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/deditec_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/export-didicontrol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/deditec-relais8/import-dedicontrol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/docker/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/library/phytec.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/library/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/modbusrtu/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/modbusrtu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/modbusrtu/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/modbusrtu/test_modbusrtu_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/networkmanager/nm.env
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/networkmanager/nm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/power/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/power/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/power/power_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/pyvisa/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/pyvisa/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/pyvisa/pyvisa_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/qemu-networking/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/qemunetworkstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/qemu-networking/test_qemu_networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/remote/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/remote/test_barebox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_hwclock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/shell/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/bareboxrebootstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/quartusstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/test_barebox_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/strategy/test_uboot_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/sysfsgpio/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/export-gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/import-gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/sysfsgpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/sysfsgpio/sysfsgpio_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.749660 labgrid-23.1a2/examples/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/mass-storage-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/mxs-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/test_usb_mxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usb/test_usb_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/examples/usbpower/
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/examplestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/exports.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbpower/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/examples/usbsdmux/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbsdmux/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-28 13:11:41.000000 labgrid-23.1a2/examples/usbsdmux/test_sdmux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-04-28 13:11:41.000000 labgrid-23.1a2/helpers/labgrid-bound-connect
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/labgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/labgrid/autoinstall/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/autoinstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/autoinstall/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/consoleloggingreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.757660 labgrid-23.1a2/labgrid/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/bareboxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/commandmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/consoleexpectmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/dediprogflashdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/deditecrelaisdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/dfudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/dockerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/externalconsoledriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/fastbootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/filedigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/flashromdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/flashscriptdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/gpiodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/httpvideodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/lxaiobusdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/lxausbmuxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/manualswitchdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/modbusdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/modbusrtudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/networkinterfacedriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/onewiredriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/openocddriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/driver/power/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/apc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/digipower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/digitalloggers_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/eaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/eg_pms2_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude8031.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude8225.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/gude8316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/netio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/netio_kshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/shelly_gen1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/siglent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/simplerest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/power/tplink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/powerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/pyvisadriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/qemudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/quartushpsdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/resetdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/serialdigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/serialdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/shelldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/sigrokdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/smallubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/sshdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/ubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbaudiodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbhidrelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbsdmuxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbsdwiredriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbstoragedriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/driver/usbtmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmc/keysight_dsox2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmc/tektronix_tds2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbtmcdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/usbvideodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/driver/xenadriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/bootstrapprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/commandprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/consoleprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/digitaloutputprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/filesystemprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/filetransferprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/infoprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/linuxbootprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/mmioprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/powerprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/resetprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/protocol/videoprotocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.761660 labgrid-23.1a2/labgrid/pytestplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/pytestplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/pytestplugin/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/pytestplugin/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.765660 labgrid-23.1a2/labgrid/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/authenticator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81571 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32314 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/remote/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.765660 labgrid-23.1a2/labgrid/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/dediprogflasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/ethernetport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/fastboot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/flashrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/httpvideostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/lxaiobus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/modbusrtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/networkservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/onewireport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/pyvisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/serialport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/sigrok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/udev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/xenamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/resource/ykushpowerport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/stepreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.765660 labgrid-23.1a2/labgrid/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/bareboxstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/dockerstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/graphstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/shellstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/strategy/ubootstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.769660 labgrid-23.1a2/labgrid/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.769660 labgrid-23.1a2/labgrid/util/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/deditec_relais8.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/sysfsgpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agents/usb_hid_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/agentwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/expect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/managedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/qmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.753660 labgrid-23.1a2/labgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 13:11:52.000000 labgrid-23.1a2/labgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-28 13:11:41.000000 labgrid-23.1a2/labgrid_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.769660 labgrid-23.1a2/man/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-client.1
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-device-config.5
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-device-config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-exporter.1
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-exporter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-pytest.7
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-pytest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-suggest.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-28 13:11:41.000000 labgrid-23.1a2/man/labgrid-suggest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 13:11:41.000000 labgrid-23.1a2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-28 13:11:41.000000 labgrid-23.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:11:52.777660 labgrid-23.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:11:52.777660 labgrid-23.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_autoinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_bareboxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_crossbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_dediprogflasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_ethernetport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_externalconsoledriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_filedigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_flashrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_flashscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_graphstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_httpvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_lxaiobus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_manualswitchdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_modbusrtudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_onewire.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_openocd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_powerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_processwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_pyvisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_qemudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_serialdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_serialport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_shelldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sigrok.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sispm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sshdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_steplogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_sysfsgpioagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_tasmota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_ubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_usbtmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_usbvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 13:11:41.000000 labgrid-23.1a2/tests/test_yaml.py
```

### Comparing `labgrid-23.1a1/.crossbar/config-anonymous.yaml` & `labgrid-23.1a2/.crossbar/config-anonymous.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/pull_request_template.md` & `labgrid-23.1a2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/workflows/build-and-release.yml` & `labgrid-23.1a2/.github/workflows/build-and-release.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/workflows/docker.yml` & `labgrid-23.1a2/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/workflows/push-pr-unit-tests.yml` & `labgrid-23.1a2/.github/workflows/push-pr-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/workflows/reusable-unit-tests-docker.yml` & `labgrid-23.1a2/.github/workflows/reusable-unit-tests-docker.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/workflows/reusable-unit-tests.yml` & `labgrid-23.1a2/.github/workflows/reusable-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/.github/workflows/scheduled-unit-tests.yml` & `labgrid-23.1a2/.github/workflows/scheduled-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/CHANGES.rst` & `labgrid-23.1a2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Release 23.1 (unreleased)
 ------------------------------------
 
 New Features in 23.1
 ~~~~~~~~~~~~~~~~~~~~
-
+- When invoking tests with pytest, the ``--log-(cli|file)-(level|format)``
+  command line arguments and their corresponding pytest.ini configure options
+  are now respected (making it possible to have different format and logging
+  levels in the log file than then console).
+- A new log level called ``CONSOLE`` has been added between the default
+  ``INFO`` and ``DEBUG`` levels. This level will show all reads and writes made
+  to the serial console during testing.
 
 Bug fixes in 23.1
 ~~~~~~~~~~~~~~~~~
 - The pypi release now uses the labgrid pyserial fork in the form of the
   pyserial-labgrid package. This fixes installation with newer versions
   of pip.
 - Several tests have gained an importorskip() call to skip them if the
@@ -20,14 +26,38 @@
 
 Breaking changes in 23.1
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 - The Debian package (``debian/``) no longer contains crossbar. Use the
   `coordinator container <https://hub.docker.com/r/labgrid/coordinator>`_ or
   install it into a separate local venv as desribed in the
   `documentation <https://labgrid.readthedocs.io/en/latest/getting_started.html#coordinator>`_.
+- The `StepReporter` API has been changed. To start step reporting, you must
+  now call ``StepReporter.start()`` instead of ``StepReporter()``
+- Logging output when running pytest is no longer sent to stderr by default,
+  since this is both chatty and also unnecessary with the improved logging
+  flexibility. It it recommended to use the ``--log-cli-level=INFO`` command
+  line option, or ``log_cli_level = INFO`` option in pytest.ini, but if you
+  want to restore the old behavior add the following to your ``conftest.py``
+  file (note that doing so may affect the ability to use some more advanced
+  logging features)::
+
+     def pytest_configure(config):
+         import logging
+         import sys
+
+         logging.basicConfig(
+             level=logging.INFO,
+             format='%(levelname)8s: %(message)s',
+             stream=sys.stderr,
+         )
+
+- The interpretation of the ``-v`` command line argument to pytest has changed
+  slightly. ``-vv`` is now an alias for ``--log-cli-level=INFO`` (effectively
+  unchanged), ``-vvv`` is an alias for ``--log-cli-level=CONSOLE``, and
+  ``-vvvv`` is an alias for ``--log-cli-level=DEBUG``.
 
 Known issues in 23.1
 ~~~~~~~~~~~~~~~~~~~~
 
 
 Release 23.0 (Released Apr 24, 2023)
 ------------------------------------
@@ -168,15 +198,15 @@
 - Labgrid client lock now enforces that all matches need to be fulfilled.
 - Support for USB HID relays has been added.
 - UBootDriver now allows overriding of currently fixed await boot timeout
   via new ``boot_timeout`` argument.
 - With ``--lg-colored-steps``, two new ``dark`` and ``light`` color schemes
   which only use the standard 8 ANSI colors can be set in ``LG_COLOR_SCHEME``.
   The existing color schemes have been renamed to ``dark-256color`` and ``light-256color``.
-  Also, the `ColoredStepReporter` now tries to autodetect whether the terminal
+  Also, the ``ColoredStepReporter`` now tries to autodetect whether the terminal
   supports 8 or 256 colors, and defaults to the respective dark variant.
   The 256-color schemes now use purple instead of green for the ``run`` lines to
   make them easier distinguishable from pytest's "PASSED" output.
 - Network controlled relay providing GET/PUT based REST API
 - The QEMUDriver gains support for -bios and qcow2 images.
 - Support for audio input has been added.
 - Usage of sshpass for SSH password input has been replaced with the SSH_ASKPASS
```

### Comparing `labgrid-23.1a1/COPYING` & `labgrid-23.1a2/COPYING`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/LICENSE` & `labgrid-23.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/PKG-INFO` & `labgrid-23.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labgrid
-Version: 23.1a1
+Version: 23.1a2
 Summary: embedded systems control library for development, testing and installation
 Author-email: Rouven Czerwinski <entwicklung@pengutronix.de>, Jan Luebbe <entwicklung@pengutronix.de>
 License: Copyright (C) 2016-2017 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
         Copyright (C) 2016-2017 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
         
         This library is free software; you can redistribute it and/or
         modify it under the terms of the GNU Lesser General Public
```

### Comparing `labgrid-23.1a1/README.rst` & `labgrid-23.1a2/README.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/contrib/completion/labgrid-client.bash` & `labgrid-23.1a2/contrib/completion/labgrid-client.bash`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/contrib/coordinator-statsd.py` & `labgrid-23.1a2/contrib/coordinator-statsd.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/contrib/sync-places.py` & `labgrid-23.1a2/contrib/sync-places.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/debian/changelog` & `labgrid-23.1a2/debian/changelog`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/debian/control` & `labgrid-23.1a2/debian/control`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/debian/copyright` & `labgrid-23.1a2/debian/copyright`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/Makefile` & `labgrid-23.1a2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/RELEASE.rst` & `labgrid-23.1a2/doc/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/conf.py` & `labgrid-23.1a2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/configuration.rst` & `labgrid-23.1a2/doc/configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3019,18 +3019,14 @@
 
     >>> from labgrid import StepReporter
     >>> StepReporter.stop()
 
 Stopping the StepReporter if it has not been started will raise an
 AssertionError, as will starting an already started StepReporter.
 
-ColoredStepReporter
-~~~~~~~~~~~~~~~~~~~
-The ColoredStepReporter inherits from the StepReporter.
-The output is colored using ANSI color code sequences.
 
 ConsoleLoggingReporter
 ~~~~~~~~~~~~~~~~~~~~~~
 The ConsoleLoggingReporter outputs read calls from the console transports into
 files. It takes the path as a parameter.
 
 .. doctest::
```

### Comparing `labgrid-23.1a1/doc/design_decisions.rst` & `labgrid-23.1a2/doc/design_decisions.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/development.rst` & `labgrid-23.1a2/doc/development.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/getting_started.rst` & `labgrid-23.1a2/doc/getting_started.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/images/favicon.png` & `labgrid-23.1a2/doc/images/favicon.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/images/labgrid_logo_outline.svg` & `labgrid-23.1a2/doc/images/labgrid_logo_outline.svg`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/index.rst` & `labgrid-23.1a2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/overview.rst` & `labgrid-23.1a2/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/res/config_graph.svg` & `labgrid-23.1a2/doc/res/config_graph.svg`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/res/graphstrategy-via-nand.png` & `labgrid-23.1a2/doc/res/graphstrategy-via-nand.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/res/graphstrategy-via-nfs.png` & `labgrid-23.1a2/doc/res/graphstrategy-via-nfs.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/doc/usage.rst` & `labgrid-23.1a2/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/dockerfiles/Dockerfile` & `labgrid-23.1a2/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/dockerfiles/README.rst` & `labgrid-23.1a2/dockerfiles/README.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/dockerfiles/build.sh` & `labgrid-23.1a2/dockerfiles/build.sh`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/dockerfiles/staging/client/.ssh/id_rsa` & `labgrid-23.1a2/dockerfiles/staging/client/.ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/dockerfiles/staging/docker-compose.yml` & `labgrid-23.1a2/dockerfiles/staging/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/dockerfiles/staging/dut/Dockerfile` & `labgrid-23.1a2/dockerfiles/staging/dut/Dockerfile`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/barebox/test_sleep.py` & `labgrid-23.1a2/examples/barebox/test_sleep.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/deditec-relais8/deditec.py` & `labgrid-23.1a2/examples/deditec-relais8/deditec.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/deditec-relais8/deditec_remote.py` & `labgrid-23.1a2/examples/deditec-relais8/deditec_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/docker/README.md` & `labgrid-23.1a2/examples/docker/README.md`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/library/test.py` & `labgrid-23.1a2/examples/library/test.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/networkmanager/nm.py` & `labgrid-23.1a2/examples/networkmanager/nm.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/qemu-networking/conftest.py` & `labgrid-23.1a2/examples/qemu-networking/conftest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/qemu-networking/local.yaml` & `labgrid-23.1a2/examples/qemu-networking/local.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/qemu-networking/qemunetworkstrategy.py` & `labgrid-23.1a2/examples/qemu-networking/qemunetworkstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/qemu-networking/test_qemu_networking.py` & `labgrid-23.1a2/examples/qemu-networking/test_qemu_networking.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/shell/test_hwclock.py` & `labgrid-23.1a2/examples/shell/test_hwclock.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/shell/test_memory.py` & `labgrid-23.1a2/examples/shell/test_memory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/shell/test_rt.py` & `labgrid-23.1a2/examples/shell/test_rt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/strategy/bareboxrebootstrategy.py` & `labgrid-23.1a2/examples/strategy/bareboxrebootstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/strategy/quartusstrategy.py` & `labgrid-23.1a2/examples/strategy/quartusstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/strategy/test_barebox_strategy.py` & `labgrid-23.1a2/examples/strategy/test_barebox_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/strategy/test_uboot_strategy.py` & `labgrid-23.1a2/examples/strategy/test_uboot_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/sysfsgpio/sysfsgpio.py` & `labgrid-23.1a2/examples/sysfsgpio/sysfsgpio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/sysfsgpio/sysfsgpio_remote.py` & `labgrid-23.1a2/examples/sysfsgpio/sysfsgpio_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usb/mxs-usb.yaml` & `labgrid-23.1a2/examples/usb/mxs-usb.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usbpower/README.rst` & `labgrid-23.1a2/examples/usbpower/README.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usbpower/cycle.py` & `labgrid-23.1a2/examples/usbpower/cycle.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usbpower/examplestrategy.py` & `labgrid-23.1a2/examples/usbpower/examplestrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usbpower/exports.yaml` & `labgrid-23.1a2/examples/usbpower/exports.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usbpower/local.yaml` & `labgrid-23.1a2/examples/usbpower/local.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/examples/usbpower/test_example.py` & `labgrid-23.1a2/examples/usbpower/test_example.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/helpers/labgrid-bound-connect` & `labgrid-23.1a2/helpers/labgrid-bound-connect`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/autoinstall/main.py` & `labgrid-23.1a2/labgrid/autoinstall/main.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/binding.py` & `labgrid-23.1a2/labgrid/binding.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/config.py` & `labgrid-23.1a2/labgrid/config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/consoleloggingreporter.py` & `labgrid-23.1a2/labgrid/consoleloggingreporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,14 @@
 
         return log
 
     def notify(self, event):
         """This is the callback function for steps"""
         step = event.step
         if step.tag == 'console':
-            if str(step) == 'read':
+            if step.title == 'read':
                 if event.data.get('state') == 'stop':
                     if step.result and step.source:
                         log = self.get_logfile(event)
                         if not log:
                             return
                         log.write(step.result)
```

### Comparing `labgrid-23.1a1/labgrid/driver/__init__.py` & `labgrid-23.1a2/labgrid/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/bareboxdriver.py` & `labgrid-23.1a2/labgrid/driver/bareboxdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
-import re
 import shlex
 
 import attr
 from pexpect import TIMEOUT
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, ConsoleProtocol, LinuxBootProtocol
 from ..step import step
-from ..util import gen_marker, Timeout
+from ..util import gen_marker, Timeout, re_vt100
 from .common import Driver
 from .commandmixin import CommandMixin
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class BareboxDriver(CommandMixin, Driver, CommandProtocol, LinuxBootProtocol):
@@ -37,17 +36,14 @@
     interrupt = attr.ib(default="\n", validator=attr.validators.instance_of(str))
     bootstring = attr.ib(default=r"Linux version \d", validator=attr.validators.instance_of(str))
     password = attr.ib(default="", validator=attr.validators.instance_of(str))
     login_timeout = attr.ib(default=60, validator=attr.validators.instance_of(int))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.re_vt100 = re.compile(
-            r'(\x1b\[|\x9b)[^@-_a-z]*[@-_a-z]|\x1b[@-_a-z]'
-        )
         self.logger = logging.getLogger(f"{self}:{self.target}")
         self._status = 0
 
     def on_activate(self):
         """Activate the BareboxDriver
 
         This function tries to login if not already active
@@ -85,15 +81,15 @@
         cmp_command = f'''echo -o /cmd {shlex.quote(cmd)}; echo {hidden_marker}; sh /cmd; echo {hidden_marker} $?;'''  # pylint: disable=line-too-long
         if self._status == 1:
             self.console.sendline(cmp_command)
             _, _, match, _ = self.console.expect(
                 rf'{marker}(.*){marker}\s+(\d+)\s+.*{self.prompt}',
                 timeout=timeout)
             # Remove VT100 Codes and split by newline
-            data = self.re_vt100.sub('', match.group(1).decode('utf-8')).split('\r\n')[1:-1]
+            data = re_vt100.sub('', match.group(1).decode('utf-8')).split('\r\n')[1:-1]
             self.logger.debug("Received Data: %s", data)
             # Get exit code
             exitcode = int(match.group(2))
             return (data, [], exitcode)
 
         return None
```

### Comparing `labgrid-23.1a1/labgrid/driver/commandmixin.py` & `labgrid-23.1a2/labgrid/driver/commandmixin.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/common.py` & `labgrid-23.1a2/labgrid/driver/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/consoleexpectmixin.py` & `labgrid-23.1a2/labgrid/driver/consoleexpectmixin.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/dediprogflashdriver.py` & `labgrid-23.1a2/labgrid/driver/dediprogflashdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/deditecrelaisdriver.py` & `labgrid-23.1a2/labgrid/driver/deditecrelaisdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/dfudriver.py` & `labgrid-23.1a2/labgrid/driver/dfudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/dockerdriver.py` & `labgrid-23.1a2/labgrid/driver/dockerdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/externalconsoledriver.py` & `labgrid-23.1a2/labgrid/driver/externalconsoledriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/fake.py` & `labgrid-23.1a2/labgrid/driver/fake.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/fastbootdriver.py` & `labgrid-23.1a2/labgrid/driver/fastbootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/filedigitaloutput.py` & `labgrid-23.1a2/labgrid/driver/filedigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/flashromdriver.py` & `labgrid-23.1a2/labgrid/driver/flashromdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/flashscriptdriver.py` & `labgrid-23.1a2/labgrid/driver/flashscriptdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/gpiodriver.py` & `labgrid-23.1a2/labgrid/driver/gpiodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/httpvideodriver.py` & `labgrid-23.1a2/labgrid/driver/httpvideodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/lxaiobusdriver.py` & `labgrid-23.1a2/labgrid/driver/lxaiobusdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/lxausbmuxdriver.py` & `labgrid-23.1a2/labgrid/driver/lxausbmuxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/manualswitchdriver.py` & `labgrid-23.1a2/labgrid/driver/manualswitchdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/modbusdriver.py` & `labgrid-23.1a2/labgrid/driver/modbusdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/modbusrtudriver.py` & `labgrid-23.1a2/labgrid/driver/modbusrtudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/mqtt.py` & `labgrid-23.1a2/labgrid/driver/mqtt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/networkinterfacedriver.py` & `labgrid-23.1a2/labgrid/driver/networkinterfacedriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/onewiredriver.py` & `labgrid-23.1a2/labgrid/driver/onewiredriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/openocddriver.py` & `labgrid-23.1a2/labgrid/driver/openocddriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/apc.py` & `labgrid-23.1a2/labgrid/driver/power/apc.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/digipower.py` & `labgrid-23.1a2/labgrid/driver/power/digipower.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/digitalloggers_http.py` & `labgrid-23.1a2/labgrid/driver/power/digitalloggers_http.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/eaton.py` & `labgrid-23.1a2/labgrid/driver/power/eaton.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/eg_pms2_network.py` & `labgrid-23.1a2/labgrid/driver/power/eg_pms2_network.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/gude.py` & `labgrid-23.1a2/labgrid/driver/power/gude.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/gude24.py` & `labgrid-23.1a2/labgrid/driver/power/gude24.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/gude8031.py` & `labgrid-23.1a2/labgrid/driver/power/gude8031.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/gude8225.py` & `labgrid-23.1a2/labgrid/driver/power/gude8225.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/gude8316.py` & `labgrid-23.1a2/labgrid/driver/power/gude8316.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/netio.py` & `labgrid-23.1a2/labgrid/driver/power/netio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/netio_kshell.py` & `labgrid-23.1a2/labgrid/driver/power/netio_kshell.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/rest.py` & `labgrid-23.1a2/labgrid/driver/power/rest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/sentry.py` & `labgrid-23.1a2/labgrid/driver/power/sentry.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/shelly_gen1.py` & `labgrid-23.1a2/labgrid/driver/power/shelly_gen1.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/siglent.py` & `labgrid-23.1a2/labgrid/driver/power/siglent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/simplerest.py` & `labgrid-23.1a2/labgrid/driver/power/simplerest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/power/tplink.py` & `labgrid-23.1a2/labgrid/driver/power/tplink.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/powerdriver.py` & `labgrid-23.1a2/labgrid/driver/powerdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/provider.py` & `labgrid-23.1a2/labgrid/driver/provider.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/pyvisadriver.py` & `labgrid-23.1a2/labgrid/driver/pyvisadriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/qemudriver.py` & `labgrid-23.1a2/labgrid/driver/qemudriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,10 +306,12 @@
             size = 4096
             size = min(max_size, size) if max_size else size
             res = self._clientsocket.recv(size)
         else:
             raise TIMEOUT(f"Timeout of {timeout:.2f} seconds exceeded")
         return res
 
-    @step(args=['data'])
     def _write(self, data):
         return self._clientsocket.send(data)
+
+    def __str__(self):
+        return f"QemuDriver({self.target.name})"
```

### Comparing `labgrid-23.1a1/labgrid/driver/quartushpsdriver.py` & `labgrid-23.1a2/labgrid/driver/quartushpsdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/resetdriver.py` & `labgrid-23.1a2/labgrid/driver/resetdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/serialdigitaloutput.py` & `labgrid-23.1a2/labgrid/driver/serialdigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/serialdriver.py` & `labgrid-23.1a2/labgrid/driver/serialdriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,7 +110,10 @@
             self.status = 1
 
     def close(self):
         """Closes the serialport, does nothing if it is already closed"""
         if self.status:
             self.serial.close()
             self.status = 0
+
+    def __str__(self):
+        return f"SerialDriver({self.target.name})"
```

### Comparing `labgrid-23.1a1/labgrid/driver/shelldriver.py` & `labgrid-23.1a2/labgrid/driver/shelldriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import attr
 from pexpect import TIMEOUT
 import xmodem
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, ConsoleProtocol, FileTransferProtocol
 from ..step import step
-from ..util import gen_marker, Timeout
+from ..util import gen_marker, Timeout, re_vt100
 from .commandmixin import CommandMixin
 from .common import Driver
 from .exception import ExecutionError
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
@@ -54,17 +54,14 @@
     console_ready = attr.ib(default="", validator=attr.validators.instance_of(str))
     await_login_timeout = attr.ib(default=2, validator=attr.validators.instance_of(int))
     post_login_settle_time = attr.ib(default=0, validator=attr.validators.instance_of(int))
 
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.re_vt100 = re.compile(
-            r'(\x1b\[|\x9b)[^@-_a-z]*[@-_a-z]|\x1b[@-_a-z]'
-        )
         self.logger = logging.getLogger(f"{self}:{self.target}")
         self._status = 0
 
         self._xmodem_cached_rx_cmd = ""
         self._xmodem_cached_sx_cmd = ""
 
     def on_activate(self):
@@ -96,15 +93,15 @@
         cmp_command = f'''MARKER='{marker[:4]}''{marker[4:]}' run {shlex.quote(cmd)}'''
         self.console.sendline(cmp_command)
         _, _, match, _ = self.console.expect(
             rf'{marker}(.*){marker}\s+(\d+)\s+{self.prompt}',
             timeout=timeout
         )
         # Remove VT100 Codes, split by newline and remove surrounding newline
-        data = self.re_vt100.sub('', match.group(1).decode(codec, decodeerrors)).split('\r\n')
+        data = re_vt100.sub('', match.group(1).decode(codec, decodeerrors)).split('\r\n')
         if data and not data[-1]:
             del data[-1]
         self.logger.debug("Received Data: %s", data)
         # Get exit code
         exitcode = int(match.group(2))
         return (data, [], exitcode)
```

### Comparing `labgrid-23.1a1/labgrid/driver/sigrokdriver.py` & `labgrid-23.1a2/labgrid/driver/sigrokdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/smallubootdriver.py` & `labgrid-23.1a2/labgrid/driver/smallubootdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ..factory import target_factory
 from ..util import gen_marker
 from ..step import step
 from .common import Driver
 
 from .ubootdriver import UBootDriver
+from ..util import re_vt100
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class SmallUBootDriver(UBootDriver):
     """
     SmallUBootDriver is meant as a driver for UBoot with only little
     functionality compared to standard a standard UBoot.
@@ -93,15 +94,15 @@
         # additionally we are not able to get the command's return code and
         # will always return 0.
         cmp_command = f"echo{marker}; {cmd}; echo{marker}"
 
         self.console.sendline(cmp_command)
         _, before, _, _ = self.console.expect(self.prompt, timeout=timeout)
 
-        data = self.re_vt100.sub(
+        data = re_vt100.sub(
             '', before.decode('utf-8'), count=1000000
         ).replace("\r", "").split("\n")
         data = data[1:]
         data = data[data.index(f"Unknown command 'echo{marker}' - try 'help'") +1 :]
         data = data[:data.index(f"Unknown command 'echo{marker}' - try 'help'")]
         if len(data) >= 1:
             if data[0].startswith("Unknown command '"):
```

### Comparing `labgrid-23.1a1/labgrid/driver/sshdriver.py` & `labgrid-23.1a2/labgrid/driver/sshdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/ubootdriver.py` & `labgrid-23.1a2/labgrid/driver/ubootdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """The U-Boot Module contains the UBootDriver"""
 import logging
-import re
 
 import attr
 from pexpect import TIMEOUT
 
 from ..factory import target_factory
 from ..protocol import CommandProtocol, ConsoleProtocol, LinuxBootProtocol
-from ..util import gen_marker, Timeout
+from ..util import gen_marker, Timeout, re_vt100
 from ..step import step
 from .common import Driver
 from .commandmixin import CommandMixin
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
@@ -45,17 +44,14 @@
     boot_command = attr.ib(default="run bootcmd", validator=attr.validators.instance_of(str))
     boot_commands = attr.ib(default=attr.Factory(dict), validator=attr.validators.instance_of(dict))
     login_timeout = attr.ib(default=30, validator=attr.validators.instance_of(int))
     boot_timeout = attr.ib(default=30, validator=attr.validators.instance_of(int))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
-        self.re_vt100 = re.compile(
-            r'(\x1b\[|\x9b)[^@-_a-z]*[@-_a-z]|\x1b[@-_a-z]'
-        )
         self.logger = logging.getLogger(f"{self}:{self.target}")
         self._status = 0
 
         if self.boot_expression:
             import warnings
             warnings.warn("boot_expression is deprecated and will be ignored", DeprecationWarning)
 
@@ -79,15 +75,15 @@
         # TODO: Shell Escaping for the U-Boot Shell
         marker = gen_marker()
         cmp_command = f"""echo '{marker[:4]}''{marker[4:]}'; {cmd}; echo "$?"; echo '{marker[:4]}''{marker[4:]}';"""  # pylint: disable=line-too-long
         if self._status == 1:
             self.console.sendline(cmp_command)
             _, before, _, _ = self.console.expect(self.prompt, timeout=timeout)
             # Remove VT100 Codes and split by newline
-            data = self.re_vt100.sub(
+            data = re_vt100.sub(
                 '', before.decode('utf-8'), count=1000000
             ).replace("\r", "").split("\n")
             self.logger.debug("Received Data: %s", data)
             # Remove first element, the invoked cmd
             data = data[data.index(marker) + 1:]
             data = data[:data.index(marker)]
             exitcode = int(data[-1])
```

### Comparing `labgrid-23.1a1/labgrid/driver/usbaudiodriver.py` & `labgrid-23.1a2/labgrid/driver/usbaudiodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbhidrelay.py` & `labgrid-23.1a2/labgrid/driver/usbhidrelay.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbloader.py` & `labgrid-23.1a2/labgrid/driver/usbloader.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbsdmuxdriver.py` & `labgrid-23.1a2/labgrid/driver/usbsdmuxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbsdwiredriver.py` & `labgrid-23.1a2/labgrid/driver/usbsdwiredriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbstoragedriver.py` & `labgrid-23.1a2/labgrid/driver/usbstoragedriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbtmc/keysight_dsox2000.py` & `labgrid-23.1a2/labgrid/driver/usbtmc/keysight_dsox2000.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbtmc/tektronix_tds2000.py` & `labgrid-23.1a2/labgrid/driver/usbtmc/tektronix_tds2000.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbtmcdriver.py` & `labgrid-23.1a2/labgrid/driver/usbtmcdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/usbvideodriver.py` & `labgrid-23.1a2/labgrid/driver/usbvideodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/driver/xenadriver.py` & `labgrid-23.1a2/labgrid/driver/xenadriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/environment.py` & `labgrid-23.1a2/labgrid/environment.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/exceptions.py` & `labgrid-23.1a2/labgrid/exceptions.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/factory.py` & `labgrid-23.1a2/labgrid/factory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/protocol/__init__.py` & `labgrid-23.1a2/labgrid/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/protocol/commandprotocol.py` & `labgrid-23.1a2/labgrid/protocol/commandprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/protocol/consoleprotocol.py` & `labgrid-23.1a2/labgrid/protocol/consoleprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/protocol/infoprotocol.py` & `labgrid-23.1a2/labgrid/protocol/infoprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/pytestplugin/fixtures.py` & `labgrid-23.1a2/labgrid/pytestplugin/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import subprocess
 import pytest
 
 from ..exceptions import NoResourceFoundError, NoDriverFoundError
 from ..remote.client import UserError
 from ..resource.remote import RemotePlace
 from ..util.ssh import sshmanager
+from ..logging import DEFAULT_FORMAT
 
 # pylint: disable=redefined-outer-name
 
 
 def pytest_addoption(parser):
     group = parser.getgroup('labgrid')
     group.addoption(
@@ -44,14 +45,19 @@
     group.addoption(
         '--lg-initial-state',
         action='store',
         dest='lg_initial_state',
         metavar='STATE_NAME',
         help='set the strategy\'s initial state (during development)')
 
+    # We would like to use a default value hook for log_format in the logging plugin,
+    # similar to the approach below:
+    # https://docs.pytest.org/en/latest/how-to/writing_hook_functions.html#using-hooks-in-pytest-addoption
+    parser.addini("log_format", default=DEFAULT_FORMAT, help="Default value for log_format (overwritten by labgrid)")
+
 
 @pytest.fixture(scope="session")
 def env(request, record_testsuite_property):
     """Return the environment configured in the supplied configuration file.
     It contains the targets contained in the configuration file.
     """
     env = request.config._labgrid_env
```

### Comparing `labgrid-23.1a1/labgrid/remote/authenticator.py` & `labgrid-23.1a2/labgrid/remote/authenticator.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/remote/client.py` & `labgrid-23.1a2/labgrid/remote/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .. import Environment, Target, target_factory
 from ..exceptions import NoDriverFoundError, NoResourceFoundError, InvalidConfigError
 from ..resource.remote import RemotePlaceManager, RemotePlace
 from ..util import diff_dict, flat_dict, filter_dict, dump, atomic_replace, Timeout
 from ..util.proxy import proxymanager
 from ..util.helper import processwrapper
 from ..driver import Mode, ExecutionError
+from ..logging import basicConfig, StepLogger
 
 txaio.config.loop = asyncio.get_event_loop()  # pylint: disable=no-member
 
 
 class Error(Exception):
     pass
 
@@ -664,17 +665,14 @@
             if self.role is None:
                 self.role = find_role_by_place(self.env.config.get_targets(), place.name)
                 if self.role is not None:
                     print(f"Selected role {self.role} from configuration file")
             target = self.env.get_target(self.role)
         if target:
             if self.args.state:
-                if self.args.verbose >= 2:
-                    from .. import StepReporter
-                    StepReporter.start()
                 strategy = target.get_driver("Strategy")
                 if self.args.initial_state:
                     print(f"Setting initial state to {self.args.initial_state}")
                     strategy.force(self.args.initial_state)
                 print(f"Transitioning into state {self.args.state}")
                 strategy.transition(self.args.state)
                 # deactivate console drivers so we are able to connect with microcom later
@@ -1398,21 +1396,22 @@
     JSON = "json"
 
     def __str__(self):
         return self.value
 
 
 def main():
-    processwrapper.enable_logging()
-    logging.basicConfig(
+    basicConfig(
         level=logging.WARNING,
-        format='%(levelname)7s: %(message)s',
         stream=sys.stderr,
     )
 
+    StepLogger.start()
+    processwrapper.enable_logging()
+
     # Support both legacy variables and properly namespaced ones
     place = os.environ.get('PLACE', None)
     place = os.environ.get('LG_PLACE', place)
     state = os.environ.get('STATE', None)
     state = os.environ.get('LG_STATE', state)
     initial_state = os.environ.get('LG_INITIAL_STATE', None)
     token = os.environ.get('LG_TOKEN', None)
@@ -1793,15 +1792,17 @@
     if args.command not in ['ssh', 'rsync', 'forward']:
         args = parser.parse_args()
     else:
         args.leftover = leftover
 
     if args.verbose:
         logging.getLogger().setLevel(logging.INFO)
-    if args.debug or args.verbose > 1:
+    if args.verbose > 1:
+        logging.getLogger().setLevel(logging.CONSOLE)
+    if args.debug or args.verbose > 2:
         logging.getLogger().setLevel(logging.DEBUG)
 
     if not args.config and (args.state or args.initial_state):
         print("Setting the state requires a configuration file", file=sys.stderr)
         exit(1)
     if args.initial_state and not args.state:
         print("Setting the initial state requires a desired state", file=sys.stderr)
```

### Comparing `labgrid-23.1a1/labgrid/remote/common.py` & `labgrid-23.1a2/labgrid/remote/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/remote/config.py` & `labgrid-23.1a2/labgrid/remote/config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/remote/coordinator.py` & `labgrid-23.1a2/labgrid/remote/coordinator.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/remote/exporter.py` & `labgrid-23.1a2/labgrid/remote/exporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/remote/scheduler.py` & `labgrid-23.1a2/labgrid/remote/scheduler.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/__init__.py` & `labgrid-23.1a2/labgrid/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/base.py` & `labgrid-23.1a2/labgrid/resource/base.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/common.py` & `labgrid-23.1a2/labgrid/resource/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/docker.py` & `labgrid-23.1a2/labgrid/resource/docker.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/ethernetport.py` & `labgrid-23.1a2/labgrid/resource/ethernetport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/lxaiobus.py` & `labgrid-23.1a2/labgrid/resource/lxaiobus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/modbus.py` & `labgrid-23.1a2/labgrid/resource/modbus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/modbusrtu.py` & `labgrid-23.1a2/labgrid/resource/modbusrtu.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/mqtt.py` & `labgrid-23.1a2/labgrid/resource/mqtt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/onewireport.py` & `labgrid-23.1a2/labgrid/resource/onewireport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/power.py` & `labgrid-23.1a2/labgrid/resource/power.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/provider.py` & `labgrid-23.1a2/labgrid/resource/provider.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/pyvisa.py` & `labgrid-23.1a2/labgrid/resource/pyvisa.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/remote.py` & `labgrid-23.1a2/labgrid/resource/remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/serialport.py` & `labgrid-23.1a2/labgrid/resource/serialport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/sigrok.py` & `labgrid-23.1a2/labgrid/resource/sigrok.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/suggest.py` & `labgrid-23.1a2/labgrid/resource/suggest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/resource/udev.py` & `labgrid-23.1a2/labgrid/resource/udev.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/step.py` & `labgrid-23.1a2/labgrid/step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import warnings
 import inspect
+import os
+import warnings
 from functools import wraps
 from time import monotonic
 
 
 # TODO: collect events from all Steps and combine when possible, only flush
 # after some time
 class Steps:
     def __init__(self):
         self._stack = []
         self._subscribers = []
 
     def get_current(self):
         return self._stack[-1] if self._stack else None
 
-    def get_new(self, title, tag, source):
-        step = Step(title, level=len(self._stack) + 1, tag=tag, source=source)  # pylint: disable=redefined-outer-name
+    def get_new(self, title, tag, source, sourceinfo):
+        step = Step(title, level=len(self._stack) + 1, tag=tag, source=source, sourceinfo=sourceinfo)  # pylint: disable=redefined-outer-name
         return step
 
     def push(self, step):  # pylint: disable=redefined-outer-name
         assert step not in self._stack
         self._stack.append(step)
         step.parent = self.get_current()
         step.level = len(self._stack)
@@ -51,15 +52,15 @@
         self.ts = monotonic()  # used to keep track of the events age
         self.step = step
         self.data = data
         self.resource = resource
         self.stream = stream
 
     def __str__(self):
-        result = [str(self.step)]
+        result = [self.step.title]
         if self.resource:
             result.append(self.resource.__class__.__name__)
         data = self.data.copy()
         duration = data.pop('duration', 0.0)
         pairs = [f"{k}={repr(v)}" for k, v in data.items() if v is not None]
         if duration >= 0.001:
             pairs.append(f"duration={duration:.3f}")
@@ -93,19 +94,20 @@
     @property
     def age(self):
         return monotonic() - self.ts
 
 
 # TODO: allow attaching log information, using a Resource as meta-data
 class Step:
-    def __init__(self, title, level, tag, source):
+    def __init__(self, title, level, tag, source, sourceinfo):
         self.title = title
         self.level = level
-        self.source = source
         self.tag = tag
+        self.source = source
+        self.sourceinfo = sourceinfo
         self.args = None
         self.result = None
         self.exception = None
         self._start_ts = None
         self._stop_ts = None
         self._skipped = False
 
@@ -121,17 +123,14 @@
             result.append(f", result={self.result}")
         duration = self.duration
         if duration >= 0.001:
             result.append(f", duration={duration:.3f}")
         result.append(")")
         return "".join(result)
 
-    def __str__(self):
-        return f"{self.title}"
-
     @property
     def duration(self):
         if self._start_ts is None:
             return 0.0
         if self._stop_ts is None:
             return monotonic() - self._start_ts
 
@@ -194,21 +193,22 @@
 def step(*, title=None, args=[], result=False, tag=None):
     def decorator(func):
         # resolve default title
         nonlocal title
         title = title or func.__name__
 
         signature = inspect.signature(func)
-
         @wraps(func)
         def wrapper(*_args, **_kwargs):
             bound = signature.bind_partial(*_args, **_kwargs)
             bound.apply_defaults()
             source = func.__self__ if inspect.ismethod(func) else bound.arguments.get('self')
-            step = steps.get_new(title, tag, source)  # pylint: disable=redefined-outer-name
+            pathname = func.__code__.co_filename
+            sourceinfo = (pathname,  os.path.basename(pathname), func.__code__.co_firstlineno)
+            step = steps.get_new(title, tag, source, sourceinfo)  # pylint: disable=redefined-outer-name
             # optionally pass the step object
             if 'step' in signature.parameters:
                 _kwargs['step'] = step
             if args:
                 step.args = {k: bound.arguments[k] for k in args}
             step.start()
             try:
```

### Comparing `labgrid-23.1a1/labgrid/stepreporter.py` & `labgrid-23.1a2/labgrid/stepreporter.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,23 @@
             DeprecationWarning,
             stacklevel=2,
         )
 
     @classmethod
     def start(cls):
         """starts the StepReporter"""
+        from warnings import warn
+        warn(
+            """
+            StepLogger is deprecated, use the StepLogger and basicConfig from labgrid.logging
+            instead which integrates with the python logging infrastructure.
+            """,
+            DeprecationWarning,
+            stacklevel=2,
+        )
         assert not cls._started
         steps.subscribe(cls.notify)
         cls._started = True
 
     @classmethod
     def stop(cls):
         """stops the StepReporter"""
```

### Comparing `labgrid-23.1a1/labgrid/strategy/bareboxstrategy.py` & `labgrid-23.1a2/labgrid/strategy/bareboxstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/strategy/common.py` & `labgrid-23.1a2/labgrid/strategy/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/strategy/dockerstrategy.py` & `labgrid-23.1a2/labgrid/strategy/dockerstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/strategy/graphstrategy.py` & `labgrid-23.1a2/labgrid/strategy/graphstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/strategy/shellstrategy.py` & `labgrid-23.1a2/labgrid/strategy/shellstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/strategy/ubootstrategy.py` & `labgrid-23.1a2/labgrid/strategy/ubootstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/target.py` & `labgrid-23.1a2/labgrid/target.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/agent.py` & `labgrid-23.1a2/labgrid/util/agent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/agents/deditec_relais8.py` & `labgrid-23.1a2/labgrid/util/agents/deditec_relais8.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/agents/network_interface.py` & `labgrid-23.1a2/labgrid/util/agents/network_interface.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/agents/sysfsgpio.py` & `labgrid-23.1a2/labgrid/util/agents/sysfsgpio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/agents/usb_hid_relay.py` & `labgrid-23.1a2/labgrid/util/agents/usb_hid_relay.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/agentwrapper.py` & `labgrid-23.1a2/labgrid/util/agentwrapper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/dict.py` & `labgrid-23.1a2/labgrid/util/dict.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/expect.py` & `labgrid-23.1a2/labgrid/util/expect.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/helper.py` & `labgrid-23.1a2/labgrid/util/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import fcntl
 import os
 import logging
 import pty
+import re
 import select
 import subprocess
 import errno
 from socket import socket, AF_INET, SOCK_STREAM
 from contextlib import closing
 
 import attr
 
 from ..step import step
 
+re_vt100 = re.compile(r"(\x1b\[|\x9b)[^@-_a-z]*[@-_a-z]|\x1b[@-_a-z]")
+
 def get_free_port():
     """Helper function to always return an unused port."""
     with closing(socket(AF_INET, SOCK_STREAM)) as s:
         s.bind(('', 0))
         return s.getsockname()[1]
```

### Comparing `labgrid-23.1a1/labgrid/util/managedfile.py` & `labgrid-23.1a2/labgrid/util/managedfile.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/proxy.py` & `labgrid-23.1a2/labgrid/util/proxy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/qmp.py` & `labgrid-23.1a2/labgrid/util/qmp.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/ssh.py` & `labgrid-23.1a2/labgrid/util/ssh.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/timeout.py` & `labgrid-23.1a2/labgrid/util/timeout.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid/util/yaml.py` & `labgrid-23.1a2/labgrid/util/yaml.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid.egg-info/PKG-INFO` & `labgrid-23.1a2/labgrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labgrid
-Version: 23.1a1
+Version: 23.1a2
 Summary: embedded systems control library for development, testing and installation
 Author-email: Rouven Czerwinski <entwicklung@pengutronix.de>, Jan Luebbe <entwicklung@pengutronix.de>
 License: Copyright (C) 2016-2017 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
         Copyright (C) 2016-2017 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
         
         This library is free software; you can redistribute it and/or
         modify it under the terms of the GNU Lesser General Public
```

### Comparing `labgrid-23.1a1/labgrid.egg-info/SOURCES.txt` & `labgrid-23.1a2/labgrid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 labgrid/__init__.py
 labgrid/binding.py
 labgrid/config.py
 labgrid/consoleloggingreporter.py
 labgrid/environment.py
 labgrid/exceptions.py
 labgrid/factory.py
+labgrid/logging.py
 labgrid/step.py
 labgrid/stepreporter.py
 labgrid/target.py
 labgrid.egg-info/PKG-INFO
 labgrid.egg-info/SOURCES.txt
 labgrid.egg-info/dependency_links.txt
 labgrid.egg-info/entry_points.txt
@@ -239,15 +240,14 @@
 labgrid/protocol/mmioprotocol.py
 labgrid/protocol/powerprotocol.py
 labgrid/protocol/resetprotocol.py
 labgrid/protocol/videoprotocol.py
 labgrid/pytestplugin/__init__.py
 labgrid/pytestplugin/fixtures.py
 labgrid/pytestplugin/hooks.py
-labgrid/pytestplugin/reporter.py
 labgrid/remote/__init__.py
 labgrid/remote/authenticator.py
 labgrid/remote/client.py
 labgrid/remote/common.py
 labgrid/remote/config.py
 labgrid/remote/coordinator.py
 labgrid/remote/exporter.py
@@ -353,15 +353,15 @@
 tests/test_serialdriver.py
 tests/test_serialport.py
 tests/test_shelldriver.py
 tests/test_sigrok.py
 tests/test_sispm.py
 tests/test_sshdriver.py
 tests/test_step.py
-tests/test_stepreporter.py
+tests/test_steplogger.py
 tests/test_strategy.py
 tests/test_sysfsgpioagent.py
 tests/test_target.py
 tests/test_tasmota.py
 tests/test_timeout.py
 tests/test_ubootdriver.py
 tests/test_usbtmc.py
```

### Comparing `labgrid-23.1a1/labgrid.egg-info/requires.txt` & `labgrid-23.1a2/labgrid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/labgrid_logo.png` & `labgrid-23.1a2/labgrid_logo.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-client.1` & `labgrid-23.1a2/man/labgrid-client.1`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-client.rst` & `labgrid-23.1a2/man/labgrid-client.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-device-config.5` & `labgrid-23.1a2/man/labgrid-device-config.5`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-device-config.rst` & `labgrid-23.1a2/man/labgrid-device-config.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-exporter.1` & `labgrid-23.1a2/man/labgrid-exporter.1`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-exporter.rst` & `labgrid-23.1a2/man/labgrid-exporter.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-pytest.7` & `labgrid-23.1a2/man/labgrid-pytest.7`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-pytest.rst` & `labgrid-23.1a2/man/labgrid-pytest.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-suggest.1` & `labgrid-23.1a2/man/labgrid-suggest.1`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/man/labgrid-suggest.rst` & `labgrid-23.1a2/man/labgrid-suggest.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/pyproject.toml` & `labgrid-23.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/conftest.py` & `labgrid-23.1a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_agent.py` & `labgrid-23.1a2/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_autoinstall.py` & `labgrid-23.1a2/tests/test_autoinstall.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_bareboxdriver.py` & `labgrid-23.1a2/tests/test_bareboxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_config.py` & `labgrid-23.1a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_crossbar.py` & `labgrid-23.1a2/tests/test_crossbar.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_dediprogflasher.py` & `labgrid-23.1a2/tests/test_dediprogflasher.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_docker.py` & `labgrid-23.1a2/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_environment.py` & `labgrid-23.1a2/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_export.py` & `labgrid-23.1a2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_externalconsoledriver.py` & `labgrid-23.1a2/tests/test_externalconsoledriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_factory.py` & `labgrid-23.1a2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_filedigitaloutput.py` & `labgrid-23.1a2/tests/test_filedigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_fixtures.py` & `labgrid-23.1a2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_flags.py` & `labgrid-23.1a2/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_flashrom.py` & `labgrid-23.1a2/tests/test_flashrom.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_flashscript.py` & `labgrid-23.1a2/tests/test_flashscript.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_graphstrategy.py` & `labgrid-23.1a2/tests/test_graphstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_lxaiobus.py` & `labgrid-23.1a2/tests/test_lxaiobus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_manualswitchdriver.py` & `labgrid-23.1a2/tests/test_manualswitchdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_modbusrtudriver.py` & `labgrid-23.1a2/tests/test_modbusrtudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_onewire.py` & `labgrid-23.1a2/tests/test_onewire.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_openocd.py` & `labgrid-23.1a2/tests/test_openocd.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_powerdriver.py` & `labgrid-23.1a2/tests/test_powerdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_processwrapper.py` & `labgrid-23.1a2/tests/test_processwrapper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_qemudriver.py` & `labgrid-23.1a2/tests/test_qemudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_remote.py` & `labgrid-23.1a2/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_reporter.py` & `labgrid-23.1a2/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_resource.py` & `labgrid-23.1a2/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_sched.py` & `labgrid-23.1a2/tests/test_sched.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_serialdriver.py` & `labgrid-23.1a2/tests/test_serialdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_shelldriver.py` & `labgrid-23.1a2/tests/test_shelldriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_sigrok.py` & `labgrid-23.1a2/tests/test_sigrok.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_sshdriver.py` & `labgrid-23.1a2/tests/test_sshdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_step.py` & `labgrid-23.1a2/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_strategy.py` & `labgrid-23.1a2/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_sysfsgpioagent.py` & `labgrid-23.1a2/tests/test_sysfsgpioagent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_target.py` & `labgrid-23.1a2/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_tasmota.py` & `labgrid-23.1a2/tests/test_tasmota.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_timeout.py` & `labgrid-23.1a2/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_ubootdriver.py` & `labgrid-23.1a2/tests/test_ubootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_usbtmc.py` & `labgrid-23.1a2/tests/test_usbtmc.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_util.py` & `labgrid-23.1a2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.1a1/tests/test_yaml.py` & `labgrid-23.1a2/tests/test_yaml.py`

 * *Files identical despite different names*

