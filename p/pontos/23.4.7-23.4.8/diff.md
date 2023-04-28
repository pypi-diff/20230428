# Comparing `tmp/pontos-23.4.7.tar.gz` & `tmp/pontos-23.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.7.tar", max compression
+gzip compressed data, was "pontos-23.4.8.tar", max compression
```

## Comparing `pontos-23.4.7.tar` & `pontos-23.4.8.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-04-27 09:37:35.119824 pontos-23.4.7/LICENSE
--rw-r--r--   0        0        0     3836 2023-04-27 09:37:35.119824 pontos-23.4.7/README.md
--rw-r--r--   0        0        0    97087 2023-04-27 09:37:35.123824 pontos-23.4.7/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-27 09:37:35.123824 pontos-23.4.7/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4427 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/parser.py
--rw-r--r--   0        0        0    13170 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13419 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2145 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16023 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-04-27 09:37:35.127824 pontos-23.4.7/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/test_parser.py
--rw-r--r--   0        0        0    78709 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_version.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.4.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-28 07:20:19.599260 pontos-23.4.8/LICENSE
+-rw-r--r--   0        0        0     3836 2023-04-28 07:20:19.599260 pontos-23.4.8/README.md
+-rw-r--r--   0        0        0    97087 2023-04-28 07:20:19.603260 pontos-23.4.8/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-28 07:20:19.603260 pontos-23.4.8/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/parser.py
+-rw-r--r--   0        0        0    13271 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-04-28 07:20:19.611260 pontos-23.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_parser.py
+-rw-r--r--   0        0        0    80450 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_version.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.4.8/PKG-INFO
```

### Comparing `pontos-23.4.7/LICENSE` & `pontos-23.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/README.md` & `pontos-23.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/poetry.lock` & `pontos-23.4.8/poetry.lock`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/__init__.py` & `pontos-23.4.8/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/changelog/__init__.py` & `pontos-23.4.8/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/changelog/conventional_commits.py` & `pontos-23.4.8/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/changelog/errors.py` & `pontos-23.4.8/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/changelog/main.py` & `pontos-23.4.8/pontos/changelog/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         description="Conventional commits utility.",
         prog="pontos-changelog",
     )
 
     parser.add_argument(
         "--config",
         "-C",
-        default="changelog.toml",
         type=Path,
         help="Conventional commits config file (toml), including conventions.",
     )
 
     parser.add_argument(
         "--project",
         required=True,
```

### Comparing `pontos-23.4.7/pontos/errors.py` & `pontos-23.4.8/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/git/__init__.py` & `pontos-23.4.8/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/git/git.py` & `pontos-23.4.8/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/git/status.py` & `pontos-23.4.8/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/__init__.py` & `pontos-23.4.8/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/__init__.py` & `pontos-23.4.8/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/argparser.py` & `pontos-23.4.8/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/cmds.py` & `pontos-23.4.8/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/core.py` & `pontos-23.4.8/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/env.py` & `pontos-23.4.8/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/errors.py` & `pontos-23.4.8/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/event.py` & `pontos-23.4.8/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/actions/main.py` & `pontos-23.4.8/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/__init__.py` & `pontos-23.4.8/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/api.py` & `pontos-23.4.8/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/artifacts.py` & `pontos-23.4.8/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/branch.py` & `pontos-23.4.8/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/client.py` & `pontos-23.4.8/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/contents.py` & `pontos-23.4.8/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/errors.py` & `pontos-23.4.8/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/helper.py` & `pontos-23.4.8/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/labels.py` & `pontos-23.4.8/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/organizations.py` & `pontos-23.4.8/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/pull_requests.py` & `pontos-23.4.8/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/release.py` & `pontos-23.4.8/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/repositories.py` & `pontos-23.4.8/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/search.py` & `pontos-23.4.8/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/tags.py` & `pontos-23.4.8/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/teams.py` & `pontos-23.4.8/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/api/workflows.py` & `pontos-23.4.8/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/argparser.py` & `pontos-23.4.8/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/cmds.py` & `pontos-23.4.8/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/main.py` & `pontos-23.4.8/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/__init__.py` & `pontos-23.4.8/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/artifact.py` & `pontos-23.4.8/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/base.py` & `pontos-23.4.8/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/branch.py` & `pontos-23.4.8/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/organization.py` & `pontos-23.4.8/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/pull_request.py` & `pontos-23.4.8/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/release.py` & `pontos-23.4.8/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/search.py` & `pontos-23.4.8/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/tag.py` & `pontos-23.4.8/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/models/workflow.py` & `pontos-23.4.8/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/pr_template.md` & `pontos-23.4.8/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/script/__init__.py` & `pontos-23.4.8/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/script/errors.py` & `pontos-23.4.8/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/script/load.py` & `pontos-23.4.8/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/github/script/parser.py` & `pontos-23.4.8/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/helper.py` & `pontos-23.4.8/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/models/__init__.py` & `pontos-23.4.8/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/__init__.py` & `pontos-23.4.8/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/api.py` & `pontos-23.4.8/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/cpe/__init__.py` & `pontos-23.4.8/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/cpe/api.py` & `pontos-23.4.8/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/cve/__init__.py` & `pontos-23.4.8/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/cve/api.py` & `pontos-23.4.8/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/models/__init__.py` & `pontos-23.4.8/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/models/cpe.py` & `pontos-23.4.8/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/models/cve.py` & `pontos-23.4.8/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.8/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.8/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/pontos.py` & `pontos-23.4.8/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/release/__init__.py` & `pontos-23.4.8/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/release/helper.py` & `pontos-23.4.8/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/release/main.py` & `pontos-23.4.8/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/release/parser.py` & `pontos-23.4.8/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/release/release.py` & `pontos-23.4.8/pontos/release/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,15 @@
         )
         self.git_tag_prefix = git_tag_prefix or ""
         self.project = (
             project if project is not None else get_git_repository_name()
         )
         self.space = space
 
-        self.terminal.info(
-            f"Using versioning scheme {versioning_scheme.__class__.__name__}"
-        )
+        self.terminal.info(f"Using versioning scheme {versioning_scheme.name}")
 
         try:
             last_release_version = get_last_release_version(
                 parse_version=versioning_scheme.parse_version,
                 git_tag_prefix=self.git_tag_prefix,
                 tag_name=f"{self.git_tag_prefix}{release_series}.*"
                 if release_series
@@ -281,17 +279,21 @@
             release_version, last_release_version, cc_config
         )
 
         self.terminal.info("Committing changes")
 
         commit_msg = f"Automatic release to {release_version}"
 
-        self.git.commit(
-            commit_msg, verify=False, gpg_signing_key=git_signing_key
-        )
+        # check if files have been modified and create a commit
+        status = list(self.git.status())
+        if status:
+            self.git.commit(
+                commit_msg, verify=False, gpg_signing_key=git_signing_key
+            )
+
         self.git.tag(
             git_version, gpg_key_id=git_signing_key, message=commit_msg
         )
 
         if not local:
             self.terminal.info("Pushing changes")
             self.git.push(follow_tags=True, remote=git_remote_name)
```

### Comparing `pontos-23.4.7/pontos/release/sign.py` & `pontos-23.4.8/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/terminal/__init__.py` & `pontos-23.4.8/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/terminal/null.py` & `pontos-23.4.8/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/terminal/rich.py` & `pontos-23.4.8/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/terminal/terminal.py` & `pontos-23.4.8/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/testing/__init__.py` & `pontos-23.4.8/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/updateheader/__init__.py` & `pontos-23.4.8/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/updateheader/__main__.py` & `pontos-23.4.8/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/updateheader/updateheader.py` & `pontos-23.4.8/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/__init__.py` & `pontos-23.4.8/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/__main__.py` & `pontos-23.4.8/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/_calculator.py` & `pontos-23.4.8/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/__init__.py` & `pontos-23.4.8/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/_cargo.py` & `pontos-23.4.8/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/_cmake.py` & `pontos-23.4.8/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/_command.py` & `pontos-23.4.8/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/_go.py` & `pontos-23.4.8/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/_javascript.py` & `pontos-23.4.8/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/commands/_python.py` & `pontos-23.4.8/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/errors.py` & `pontos-23.4.8/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/helper.py` & `pontos-23.4.8/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/main.py` & `pontos-23.4.8/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/parser.py` & `pontos-23.4.8/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/project.py` & `pontos-23.4.8/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/schemes/__init__.py` & `pontos-23.4.8/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pontos/version/schemes/_pep440.py` & `pontos-23.4.8/pontos/version/schemes/_pep440.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,7 +398,8 @@
 class PEP440VersioningScheme(VersioningScheme):
     """
     PEP 440 versioning scheme
     """
 
     version_calculator_cls = PEP440VersionCalculator
     version_cls = PEP440Version
+    name = "PEP440"
```

### Comparing `pontos-23.4.7/pontos/version/schemes/_scheme.py` & `pontos-23.4.8/pontos/version/schemes/_scheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             class MyVersioningScheme(VersioningScheme):
                 version_cls = MyVersion
                 version_calculator_cls = MyVersionCalculator
     """
 
     version_cls: Type[Version]
     version_calculator_cls: Type[VersionCalculator]
+    name: str
 
     @classmethod
     def parse_version(cls, version: str) -> Version:
         """
         Parse a version from a version string
 
         Raises:
```

### Comparing `pontos-23.4.7/pontos/version/schemes/_semantic.py` & `pontos-23.4.8/pontos/version/schemes/_semantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,7 +463,8 @@
             "-rc1"
         )
 
 
 class SemanticVersioningScheme(VersioningScheme):
     version_cls = SemanticVersion
     version_calculator_cls = SemanticVersionCalculator
+    name = "SemVer"
```

### Comparing `pontos-23.4.7/pontos/version/version.py` & `pontos-23.4.8/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/pyproject.toml` & `pontos-23.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.7"
+version = "23.4.8"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.4.7/scripts/github/artifacts-download.py` & `pontos-23.4.8/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/artifacts.py` & `pontos-23.4.8/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/branchprotection.py` & `pontos-23.4.8/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/create-repository.py` & `pontos-23.4.8/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/enforce-admins.py` & `pontos-23.4.8/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/lock-branch.py` & `pontos-23.4.8/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/members.py` & `pontos-23.4.8/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/release-assets-download.py` & `pontos-23.4.8/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/repositories.py` & `pontos-23.4.8/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/search-repositories.py` & `pontos-23.4.8/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/team-repositories.py` & `pontos-23.4.8/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/teams.py` & `pontos-23.4.8/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/scripts/github/workflow-runs.py` & `pontos-23.4.8/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/__init__.py` & `pontos-23.4.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/changelog/__init__.py` & `pontos-23.4.8/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/changelog/test_conventional_commits.py` & `pontos-23.4.8/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/changelog/test_parser.py` & `pontos-23.4.8/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/git/__init__.py` & `pontos-23.4.8/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/git/test_git.py` & `pontos-23.4.8/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/git/test_status.py` & `pontos-23.4.8/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/__init__.py` & `pontos-23.4.8/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/actions/__init__.py` & `pontos-23.4.8/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.8/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/actions/test_core.py` & `pontos-23.4.8/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/actions/test_env.py` & `pontos-23.4.8/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/actions/test_event.py` & `pontos-23.4.8/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/__init__.py` & `pontos-23.4.8/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/pr-files.json` & `pontos-23.4.8/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/release-response.json` & `pontos-23.4.8/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_artifacts.py` & `pontos-23.4.8/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_branch.py` & `pontos-23.4.8/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_client.py` & `pontos-23.4.8/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_contents.py` & `pontos-23.4.8/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_labels.py` & `pontos-23.4.8/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_organizations.py` & `pontos-23.4.8/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_pull_requests.py` & `pontos-23.4.8/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_release.py` & `pontos-23.4.8/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_repositories.py` & `pontos-23.4.8/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_search.py` & `pontos-23.4.8/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_tags.py` & `pontos-23.4.8/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_teams.py` & `pontos-23.4.8/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/api/test_workflows.py` & `pontos-23.4.8/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/__init__.py` & `pontos-23.4.8/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_artifact.py` & `pontos-23.4.8/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_base.py` & `pontos-23.4.8/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_branch.py` & `pontos-23.4.8/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_organization.py` & `pontos-23.4.8/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_pull_request.py` & `pontos-23.4.8/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_release.py` & `pontos-23.4.8/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_search.py` & `pontos-23.4.8/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_tag.py` & `pontos-23.4.8/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/models/test_workflow.py` & `pontos-23.4.8/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/script/__init__.py` & `pontos-23.4.8/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/script/test_load.py` & `pontos-23.4.8/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/script/test_parser.py` & `pontos-23.4.8/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/test_argparser.py` & `pontos-23.4.8/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/github/test_cmds.py` & `pontos-23.4.8/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/models/__init__.py` & `pontos-23.4.8/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/models/test_models.py` & `pontos-23.4.8/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/__init__.py` & `pontos-23.4.8/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/cpe/__init__.py` & `pontos-23.4.8/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/cpe/test_api.py` & `pontos-23.4.8/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/cve/__init__.py` & `pontos-23.4.8/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/cve/test_api.py` & `pontos-23.4.8/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/models/__init__.py` & `pontos-23.4.8/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/models/test_cpe.py` & `pontos-23.4.8/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/models/test_cve.py` & `pontos-23.4.8/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/nvd/test_api.py` & `pontos-23.4.8/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/release/__init__.py` & `pontos-23.4.8/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/release/test_helper.py` & `pontos-23.4.8/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/release/test_parser.py` & `pontos-23.4.8/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/release/test_release.py` & `pontos-23.4.8/tests/release/test_release.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from pathlib import Path
 from typing import Iterable, Optional, Union
 from unittest.mock import AsyncMock, MagicMock, call, patch
 
 from httpx import HTTPStatusError, Request, Response
 
 from pontos.git.git import ConfigScope, Git
+from pontos.git.status import StatusEntry
 from pontos.release.main import parse_args
 from pontos.release.release import ReleaseReturnValue, release
 from pontos.terminal.terminal import Terminal
 from pontos.testing import temp_git_repository
 from pontos.version import VersionError, VersionUpdate
 from pontos.version.commands import GoVersionCommand
 from pontos.version.schemes._pep440 import PEP440Version, PEP440VersioningScheme
@@ -117,14 +118,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
@@ -137,15 +142,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
 
         command_mock.update_version.assert_has_calls(
@@ -156,33 +161,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -217,14 +222,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
@@ -235,15 +244,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
 
         command_mock.update_version.assert_has_calls(
@@ -254,33 +263,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 1.0.0",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.1.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v1.0.0", gpg_key_id="1234", message="Automatic release to 1.0.0"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -315,14 +324,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -335,15 +348,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
         command_mock.update_version.assert_has_calls(
             [
@@ -353,33 +366,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -415,14 +428,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -433,15 +450,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
 
         command_mock.update_version.assert_has_calls(
@@ -452,33 +469,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     f"Automatic release to {release_version}",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     f"* Update to version {next_version}\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             f"v{release_version}",
             gpg_key_id="1234",
             message=f"Automatic release to {release_version}",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
@@ -515,14 +532,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -535,15 +556,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
         command_mock.update_version.assert_has_calls(
             [
@@ -553,33 +574,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.1.0",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.1.1.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.1.0", gpg_key_id="1234", message="Automatic release to 0.1.0"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -614,14 +635,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -634,15 +659,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
         command_mock.update_version.assert_has_calls(
             [
@@ -652,33 +677,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 1.0.0",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.1.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v1.0.0", gpg_key_id="1234", message="Automatic release to 1.0.0"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -713,14 +738,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -731,15 +760,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
         command_mock.update_version.assert_has_calls(
             [
@@ -749,33 +778,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2a1",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.0.2a2.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2a1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.2a1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
@@ -812,14 +841,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -830,15 +863,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
         command_mock.update_version.assert_has_calls(
             [
@@ -848,33 +881,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2b1",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.0.2b2.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2b1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.2b1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
@@ -911,14 +944,18 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
@@ -929,15 +966,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
         command_mock.update_version.assert_has_calls(
             [
@@ -947,33 +984,33 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("MyProject.conf"), call("MyProject.conf")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2rc1",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.0.2rc2.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2rc1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.2rc1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
@@ -1044,14 +1081,16 @@
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2")
         create_changelog_mock.return_value = "A Changelog"
         get_last_release_version_mock.return_value = current_version
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = []
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
@@ -1065,43 +1104,38 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ],
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_not_called()
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.add.assert_not_called()
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
-                    "Automatic release to 0.0.2",
-                    verify=False,
-                    gpg_signing_key="1234",
-                ),
-                call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
         project_mock.assert_not_called()
 
@@ -1305,14 +1339,18 @@
         ]
         create_changelog_mock.return_value = "A Changelog"
         create_release_mock.side_effect = HTTPStatusError(
             "Error during a request",
             request=MagicMock(spec=Request),
             response=MagicMock(spec=Response),
         )
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
@@ -1327,22 +1365,22 @@
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         self.assertEqual(released, ReleaseReturnValue.CREATE_RELEASE_ERROR)
 
-        git_mock.return_value.push.assert_called_once_with(
+        git_instance_mock.push.assert_called_once_with(
             follow_tags=True, remote=None
         )
-        git_mock.return_value.add.assert_called_once_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_once_with(
+        git_instance_mock.add.assert_called_once_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_once_with(
             "Automatic release to 0.0.1", verify=False, gpg_signing_key="1234"
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
@@ -1375,14 +1413,18 @@
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionError("An error"),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
@@ -1395,15 +1437,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_called_once_with(
+        git_instance_mock.push.assert_called_once_with(
             follow_tags=True, remote=None
         )
 
         command_mock.update_version.assert_has_calls(
             [
                 call(release_version, force=False),
                 call(next_version, force=False),
@@ -1411,19 +1453,19 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        git_mock.return_value.add.assert_called_once_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_once_with(
+        git_instance_mock.add.assert_called_once_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_once_with(
             "Automatic release to 0.0.1", verify=False, gpg_signing_key="1234"
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(
             released, ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
         )
 
@@ -1881,14 +1923,16 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["project.conf", "version.lang"],
             ),
         ]
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [StatusEntry("M  project.conf")]
         cc_git_mock.return_value.log.return_value = [
             "1234567 Add: foo bar",
             "8abcdef Add: bar baz",
             "8abcd3f Add bar baz",
             "8abcd3d Adding bar baz",
             "1337abc Change: bar to baz",
             "42a42a4 Remove: foo bar again",
@@ -1930,21 +1974,21 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.list_tags.assert_called_once_with()
+        git_instance_mock.list_tags.assert_called_once_with()
 
         cc_git_mock.return_value.log.assert_called_once_with(
             "v0.0.1..HEAD", oneline=True
         )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
                 call(follow_tags=True, remote=None),
             ]
         )
 
         command_mock.update_version.assert_has_calls(
@@ -1955,21 +1999,21 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", expected_changelog),
         )
 
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
-        git_mock.return_value.add.assert_has_calls(
+        git_instance_mock.add.assert_has_calls(
             [call("project.conf"), call("project.conf"), call("version.lang")]
         )
-        git_mock.return_value.commit.assert_has_calls(
+        git_instance_mock.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
                 call(
```

### Comparing `pontos-23.4.7/tests/release/test_sign.py` & `pontos-23.4.8/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/terminal/__init__.py` & `pontos-23.4.8/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/terminal/test_terminal.py` & `pontos-23.4.8/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/test_helper.py` & `pontos-23.4.8/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/test_pontos.py` & `pontos-23.4.8/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/testing/__init__.py` & `pontos-23.4.8/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/testing/test_testing.py` & `pontos-23.4.8/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/updateheader/__init__.py` & `pontos-23.4.8/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/updateheader/test_header.py` & `pontos-23.4.8/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/__init__.py` & `pontos-23.4.8/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/commands/__init__.py` & `pontos-23.4.8/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/commands/test_cargo.py` & `pontos-23.4.8/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/commands/test_cmake.py` & `pontos-23.4.8/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/commands/test_go.py` & `pontos-23.4.8/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/commands/test_javascript.py` & `pontos-23.4.8/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/commands/test_python.py` & `pontos-23.4.8/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/schemes/__init__.py` & `pontos-23.4.8/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/schemes/test_pep440.py` & `pontos-23.4.8/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/schemes/test_semantic.py` & `pontos-23.4.8/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_commands.py` & `pontos-23.4.8/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_errors.py` & `pontos-23.4.8/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_helper.py` & `pontos-23.4.8/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_main.py` & `pontos-23.4.8/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_parser.py` & `pontos-23.4.8/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_project.py` & `pontos-23.4.8/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/tests/version/test_version.py` & `pontos-23.4.8/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.7/PKG-INFO` & `pontos-23.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.7
+Version: 23.4.8
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

