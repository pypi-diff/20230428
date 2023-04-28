# Comparing `tmp/pontos-23.4.8.tar.gz` & `tmp/pontos-23.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.8.tar", max compression
+gzip compressed data, was "pontos-23.4.9.tar", max compression
```

## Comparing `pontos-23.4.8.tar` & `pontos-23.4.9.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-04-28 07:20:19.599260 pontos-23.4.8/LICENSE
--rw-r--r--   0        0        0     3836 2023-04-28 07:20:19.599260 pontos-23.4.8/README.md
--rw-r--r--   0        0        0    97087 2023-04-28 07:20:19.603260 pontos-23.4.8/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-28 07:20:19.603260 pontos-23.4.8/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-28 07:20:19.603260 pontos-23.4.8/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/parser.py
--rw-r--r--   0        0        0    13271 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-04-28 07:20:19.607260 pontos-23.4.8/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-04-28 07:20:19.611260 pontos-23.4.8/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-04-28 07:20:19.611260 pontos-23.4.8/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-28 07:20:19.611260 pontos-23.4.8/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.611260 pontos-23.4.8/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-28 07:20:19.615260 pontos-23.4.8/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_parser.py
--rw-r--r--   0        0        0    80450 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-28 07:20:19.619260 pontos-23.4.8/tests/version/test_version.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.4.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-28 08:40:31.911312 pontos-23.4.9/LICENSE
+-rw-r--r--   0        0        0     3836 2023-04-28 08:40:31.911312 pontos-23.4.9/README.md
+-rw-r--r--   0        0        0    97087 2023-04-28 08:40:31.915312 pontos-23.4.9/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-28 08:40:31.915312 pontos-23.4.9/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-28 08:40:31.915312 pontos-23.4.9/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/release/parser.py
+-rw-r--r--   0        0        0    13491 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-28 08:40:31.919313 pontos-23.4.9/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-28 08:40:31.923313 pontos-23.4.9/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-04-28 08:40:31.923313 pontos-23.4.9/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-04-28 08:40:31.923313 pontos-23.4.9/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-04-28 08:40:31.923313 pontos-23.4.9/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-04-28 08:40:31.923313 pontos-23.4.9/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-04-28 08:40:31.923313 pontos-23.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-28 08:40:31.923313 pontos-23.4.9/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-28 08:40:31.923313 pontos-23.4.9/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/release/test_parser.py
+-rw-r--r--   0        0        0    81080 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-04-28 08:40:31.927313 pontos-23.4.9/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-28 08:40:31.931313 pontos-23.4.9/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-28 08:40:31.931313 pontos-23.4.9/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-28 08:40:31.931313 pontos-23.4.9/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-28 08:40:31.931313 pontos-23.4.9/tests/version/test_version.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.4.9/PKG-INFO
```

### Comparing `pontos-23.4.8/LICENSE` & `pontos-23.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/README.md` & `pontos-23.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/poetry.lock` & `pontos-23.4.9/poetry.lock`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/__init__.py` & `pontos-23.4.9/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/changelog/__init__.py` & `pontos-23.4.9/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/changelog/conventional_commits.py` & `pontos-23.4.9/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/changelog/errors.py` & `pontos-23.4.9/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/changelog/main.py` & `pontos-23.4.9/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/errors.py` & `pontos-23.4.9/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/git/__init__.py` & `pontos-23.4.9/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/git/git.py` & `pontos-23.4.9/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/git/status.py` & `pontos-23.4.9/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/__init__.py` & `pontos-23.4.9/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/__init__.py` & `pontos-23.4.9/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/argparser.py` & `pontos-23.4.9/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/cmds.py` & `pontos-23.4.9/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/core.py` & `pontos-23.4.9/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/env.py` & `pontos-23.4.9/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/errors.py` & `pontos-23.4.9/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/event.py` & `pontos-23.4.9/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/actions/main.py` & `pontos-23.4.9/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/__init__.py` & `pontos-23.4.9/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/api.py` & `pontos-23.4.9/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/artifacts.py` & `pontos-23.4.9/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/branch.py` & `pontos-23.4.9/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/client.py` & `pontos-23.4.9/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/contents.py` & `pontos-23.4.9/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/errors.py` & `pontos-23.4.9/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/helper.py` & `pontos-23.4.9/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/labels.py` & `pontos-23.4.9/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/organizations.py` & `pontos-23.4.9/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/pull_requests.py` & `pontos-23.4.9/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/release.py` & `pontos-23.4.9/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/repositories.py` & `pontos-23.4.9/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/search.py` & `pontos-23.4.9/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/tags.py` & `pontos-23.4.9/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/teams.py` & `pontos-23.4.9/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/api/workflows.py` & `pontos-23.4.9/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/argparser.py` & `pontos-23.4.9/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/cmds.py` & `pontos-23.4.9/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/main.py` & `pontos-23.4.9/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/__init__.py` & `pontos-23.4.9/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/artifact.py` & `pontos-23.4.9/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/base.py` & `pontos-23.4.9/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/branch.py` & `pontos-23.4.9/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/organization.py` & `pontos-23.4.9/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/pull_request.py` & `pontos-23.4.9/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/release.py` & `pontos-23.4.9/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/search.py` & `pontos-23.4.9/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/tag.py` & `pontos-23.4.9/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/models/workflow.py` & `pontos-23.4.9/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/pr_template.md` & `pontos-23.4.9/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/script/__init__.py` & `pontos-23.4.9/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/script/errors.py` & `pontos-23.4.9/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/script/load.py` & `pontos-23.4.9/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/github/script/parser.py` & `pontos-23.4.9/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/helper.py` & `pontos-23.4.9/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/models/__init__.py` & `pontos-23.4.9/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/__init__.py` & `pontos-23.4.9/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/api.py` & `pontos-23.4.9/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/cpe/__init__.py` & `pontos-23.4.9/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/cpe/api.py` & `pontos-23.4.9/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/cve/__init__.py` & `pontos-23.4.9/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/cve/api.py` & `pontos-23.4.9/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/models/__init__.py` & `pontos-23.4.9/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/models/cpe.py` & `pontos-23.4.9/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/models/cve.py` & `pontos-23.4.9/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.9/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.9/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/pontos.py` & `pontos-23.4.9/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/release/__init__.py` & `pontos-23.4.9/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/release/helper.py` & `pontos-23.4.9/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/release/main.py` & `pontos-23.4.9/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/release/parser.py` & `pontos-23.4.9/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/release/release.py` & `pontos-23.4.9/pontos/release/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,25 +275,26 @@
             f"{last_release_version}"
         )
 
         release_text = self._create_changelog(
             release_version, last_release_version, cc_config
         )
 
-        self.terminal.info("Committing changes")
-
         commit_msg = f"Automatic release to {release_version}"
 
         # check if files have been modified and create a commit
         status = list(self.git.status())
         if status:
+            self.terminal.info("Committing changes")
+
             self.git.commit(
                 commit_msg, verify=False, gpg_signing_key=git_signing_key
             )
 
+        self.terminal.info(f"Creating tag {git_version}")
         self.git.tag(
             git_version, gpg_key_id=git_signing_key, message=commit_msg
         )
 
         if not local:
             self.terminal.info("Pushing changes")
             self.git.push(follow_tags=True, remote=git_remote_name)
@@ -323,23 +324,26 @@
                 )
                 return ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
 
             for f in updated.changed_files:
                 self.terminal.info(f"Adding changes of {f}")
                 self.git.add(f)
 
-        commit_msg = f"""Automatic adjustments after release
+        # check if files have been modified and create a commit
+        status = list(self.git.status())
+        if status:
+            commit_msg = f"""Automatic adjustments after release
 
 * Update to version {next_version}
 """
 
-        self.terminal.info("Committing changes")
-        self.git.commit(
-            commit_msg, verify=False, gpg_signing_key=git_signing_key
-        )
+            self.terminal.info("Committing changes after release")
+            self.git.commit(
+                commit_msg, verify=False, gpg_signing_key=git_signing_key
+            )
 
         if not local:
             self.terminal.info("Pushing changes")
             self.git.push(follow_tags=True, remote=git_remote_name)
 
         return ReleaseReturnValue.SUCCESS
```

### Comparing `pontos-23.4.8/pontos/release/sign.py` & `pontos-23.4.9/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/terminal/__init__.py` & `pontos-23.4.9/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/terminal/null.py` & `pontos-23.4.9/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/terminal/rich.py` & `pontos-23.4.9/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/terminal/terminal.py` & `pontos-23.4.9/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/testing/__init__.py` & `pontos-23.4.9/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/updateheader/__init__.py` & `pontos-23.4.9/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/updateheader/__main__.py` & `pontos-23.4.9/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/updateheader/updateheader.py` & `pontos-23.4.9/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/__init__.py` & `pontos-23.4.9/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/__main__.py` & `pontos-23.4.9/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/_calculator.py` & `pontos-23.4.9/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/__init__.py` & `pontos-23.4.9/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/_cargo.py` & `pontos-23.4.9/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/_cmake.py` & `pontos-23.4.9/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/_command.py` & `pontos-23.4.9/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/_go.py` & `pontos-23.4.9/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/_javascript.py` & `pontos-23.4.9/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/commands/_python.py` & `pontos-23.4.9/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/errors.py` & `pontos-23.4.9/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/helper.py` & `pontos-23.4.9/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/main.py` & `pontos-23.4.9/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/parser.py` & `pontos-23.4.9/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/project.py` & `pontos-23.4.9/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/schemes/__init__.py` & `pontos-23.4.9/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/schemes/_pep440.py` & `pontos-23.4.9/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/schemes/_scheme.py` & `pontos-23.4.9/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/schemes/_semantic.py` & `pontos-23.4.9/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pontos/version/version.py` & `pontos-23.4.9/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/pyproject.toml` & `pontos-23.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.8"
+version = "23.4.9"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.4.8/scripts/github/artifacts-download.py` & `pontos-23.4.9/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/artifacts.py` & `pontos-23.4.9/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/branchprotection.py` & `pontos-23.4.9/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/create-repository.py` & `pontos-23.4.9/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/enforce-admins.py` & `pontos-23.4.9/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/lock-branch.py` & `pontos-23.4.9/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/members.py` & `pontos-23.4.9/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/release-assets-download.py` & `pontos-23.4.9/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/repositories.py` & `pontos-23.4.9/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/search-repositories.py` & `pontos-23.4.9/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/team-repositories.py` & `pontos-23.4.9/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/teams.py` & `pontos-23.4.9/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/scripts/github/workflow-runs.py` & `pontos-23.4.9/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/__init__.py` & `pontos-23.4.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/changelog/__init__.py` & `pontos-23.4.9/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/changelog/test_conventional_commits.py` & `pontos-23.4.9/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/changelog/test_parser.py` & `pontos-23.4.9/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/git/__init__.py` & `pontos-23.4.9/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/git/test_git.py` & `pontos-23.4.9/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/git/test_status.py` & `pontos-23.4.9/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/__init__.py` & `pontos-23.4.9/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/actions/__init__.py` & `pontos-23.4.9/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.9/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/actions/test_core.py` & `pontos-23.4.9/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/actions/test_env.py` & `pontos-23.4.9/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/actions/test_event.py` & `pontos-23.4.9/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/__init__.py` & `pontos-23.4.9/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/pr-files.json` & `pontos-23.4.9/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/release-response.json` & `pontos-23.4.9/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_artifacts.py` & `pontos-23.4.9/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_branch.py` & `pontos-23.4.9/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_client.py` & `pontos-23.4.9/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_contents.py` & `pontos-23.4.9/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_labels.py` & `pontos-23.4.9/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_organizations.py` & `pontos-23.4.9/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_pull_requests.py` & `pontos-23.4.9/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_release.py` & `pontos-23.4.9/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_repositories.py` & `pontos-23.4.9/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_search.py` & `pontos-23.4.9/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_tags.py` & `pontos-23.4.9/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_teams.py` & `pontos-23.4.9/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/api/test_workflows.py` & `pontos-23.4.9/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/__init__.py` & `pontos-23.4.9/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_artifact.py` & `pontos-23.4.9/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_base.py` & `pontos-23.4.9/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_branch.py` & `pontos-23.4.9/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_organization.py` & `pontos-23.4.9/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_pull_request.py` & `pontos-23.4.9/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_release.py` & `pontos-23.4.9/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_search.py` & `pontos-23.4.9/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_tag.py` & `pontos-23.4.9/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/models/test_workflow.py` & `pontos-23.4.9/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/script/__init__.py` & `pontos-23.4.9/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/script/test_load.py` & `pontos-23.4.9/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/script/test_parser.py` & `pontos-23.4.9/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/test_argparser.py` & `pontos-23.4.9/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/github/test_cmds.py` & `pontos-23.4.9/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/models/__init__.py` & `pontos-23.4.9/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/models/test_models.py` & `pontos-23.4.9/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/__init__.py` & `pontos-23.4.9/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/cpe/__init__.py` & `pontos-23.4.9/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/cpe/test_api.py` & `pontos-23.4.9/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/cve/__init__.py` & `pontos-23.4.9/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/cve/test_api.py` & `pontos-23.4.9/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/models/__init__.py` & `pontos-23.4.9/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/models/test_cpe.py` & `pontos-23.4.9/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/models/test_cve.py` & `pontos-23.4.9/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/nvd/test_api.py` & `pontos-23.4.9/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/release/__init__.py` & `pontos-23.4.9/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/release/test_helper.py` & `pontos-23.4.9/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/release/test_parser.py` & `pontos-23.4.9/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/release/test_release.py` & `pontos-23.4.9/tests/release/test_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -1117,24 +1117,15 @@
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
         git_instance_mock.add.assert_not_called()
-        git_instance_mock.commit.assert_has_calls(
-            [
-                call(
-                    "Automatic adjustments after release\n\n"
-                    "* Update to version 1.0.0.dev1\n",
-                    verify=False,
-                    gpg_signing_key="1234",
-                ),
-            ]
-        )
+        git_instance_mock.commit.assert_not_called()
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
         project_mock.assert_not_called()
@@ -1501,14 +1492,18 @@
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
         create_changelog_mock.return_value = "A Changelog"
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
@@ -1525,15 +1520,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote="upstream"),
                 call(follow_tags=True, remote="upstream"),
             ],
         )
 
         self.assertEqual(
@@ -1544,22 +1539,22 @@
         command_mock.update_version.assert_has_calls(
             [
                 call(release_version, force=False),
                 call(next_version, force=False),
             ],
         )
 
-        git_mock.return_value.add.assert_called_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_with(
+        git_instance_mock.add.assert_called_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
             "* Update to version 0.0.2.dev1\n",
             verify=False,
             gpg_signing_key="1234",
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -1593,14 +1588,18 @@
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
         create_changelog_mock.return_value = "A Changelog"
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
@@ -1615,15 +1614,15 @@
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
@@ -1634,22 +1633,22 @@
         command_mock.update_version.assert_has_calls(
             [
                 call(release_version, force=False),
                 call(next_version, force=False),
             ],
         )
 
-        git_mock.return_value.add.assert_called_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_with(
+        git_instance_mock.add.assert_called_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
             "* Update to version 0.0.2.dev1\n",
             verify=False,
             gpg_signing_key="1234",
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -1683,14 +1682,18 @@
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
         create_changelog_mock.return_value = "A Changelog"
         create_api_mock = AsyncMock()
         github_api_mock.return_value.releases.create = create_api_mock
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--space",
                 "bar",
                 "--project",
@@ -1707,15 +1710,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote="upstream"),
                 call(follow_tags=True, remote="upstream"),
             ],
         )
 
         create_api_mock.assert_awaited_once_with(
@@ -1729,22 +1732,22 @@
         command_mock.update_version.assert_has_calls(
             [
                 call(release_version, force=False),
                 call(next_version, force=False),
             ],
         )
 
-        git_mock.return_value.add.assert_called_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_with(
+        git_instance_mock.add.assert_called_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
             "* Update to version 0.0.2.dev1\n",
             verify=False,
             gpg_signing_key="1234",
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.release.release.get_last_release_version", autospec=True)
@@ -1778,14 +1781,18 @@
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
         create_changelog_mock.return_value = "A Changelog"
         create_api_mock = AsyncMock()
         github_api_mock.return_value.releases.create = create_api_mock
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry("M  MyProject.conf")
+        ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--space",
                 "bar",
                 "--project",
@@ -1802,15 +1809,15 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_has_calls(
+        git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote="upstream"),
                 call(follow_tags=True, remote="upstream"),
             ],
         )
 
         create_api_mock.assert_awaited_once_with(
@@ -1824,22 +1831,22 @@
         command_mock.update_version.assert_has_calls(
             [
                 call(release_version, force=False),
                 call(next_version, force=False),
             ],
         )
 
-        git_mock.return_value.add.assert_called_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_with(
+        git_instance_mock.add.assert_called_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
             "* Update to version 0.0.1a1+dev1\n",
             verify=False,
             gpg_signing_key="1234",
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.1a1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.1a1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
@@ -1856,38 +1863,42 @@
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         git_mock,
     ):
         release_version = PEP440Version("0.0.2")
 
         create_changelog_mock.return_value = "A Changelog"
+
+        git_instance_mock: MagicMock = git_mock.return_value
+        git_instance_mock.status.return_value = [
+            StatusEntry(f"M  {GoVersionCommand.version_file_path}")
+        ]
+
         _, token, args = parse_args(["release", "--release-type", "patch"])
 
         with setup_go_project(current_version="0.0.1", tags=["0.0.1"]):
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
-        git_mock.return_value.push.assert_called_with(
-            follow_tags=True, remote=None
-        )
-        git_mock.return_value.add.assert_called_with(
+        git_instance_mock.push.assert_called_with(follow_tags=True, remote=None)
+        git_instance_mock.add.assert_called_with(
             GoVersionCommand.version_file_path
         )
-        git_mock.return_value.commit.assert_called_with(
+        git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
             "* Update to version 0.0.3.dev1\n",
             verify=False,
             gpg_signing_key="1234",
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
@@ -2059,14 +2070,18 @@
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
         create_changelog_mock.return_value = "A Changelog"
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
@@ -2080,33 +2095,33 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        git_mock.return_value.push.assert_not_called()
+        git_instance_mock.push.assert_not_called()
 
         create_release_mock.assert_not_awaited()
 
         command_mock.update_version.assert_has_calls(
             [
                 call(release_version, force=False),
                 call(next_version, force=False),
             ]
         )
 
-        git_mock.return_value.add.assert_called_with("MyProject.conf")
-        git_mock.return_value.commit.assert_called_with(
+        git_instance_mock.add.assert_called_with("MyProject.conf")
+        git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
             "* Update to version 0.0.2.dev1\n",
             verify=False,
             gpg_signing_key="1234",
         )
-        git_mock.return_value.tag.assert_called_once_with(
+        git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
 
 @dataclass
```

### Comparing `pontos-23.4.8/tests/release/test_sign.py` & `pontos-23.4.9/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/terminal/__init__.py` & `pontos-23.4.9/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/terminal/test_terminal.py` & `pontos-23.4.9/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/test_helper.py` & `pontos-23.4.9/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/test_pontos.py` & `pontos-23.4.9/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/testing/__init__.py` & `pontos-23.4.9/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/testing/test_testing.py` & `pontos-23.4.9/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/updateheader/__init__.py` & `pontos-23.4.9/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/updateheader/test_header.py` & `pontos-23.4.9/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/__init__.py` & `pontos-23.4.9/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/commands/__init__.py` & `pontos-23.4.9/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/commands/test_cargo.py` & `pontos-23.4.9/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/commands/test_cmake.py` & `pontos-23.4.9/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/commands/test_go.py` & `pontos-23.4.9/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/commands/test_javascript.py` & `pontos-23.4.9/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/commands/test_python.py` & `pontos-23.4.9/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/schemes/__init__.py` & `pontos-23.4.9/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/schemes/test_pep440.py` & `pontos-23.4.9/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/schemes/test_semantic.py` & `pontos-23.4.9/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_commands.py` & `pontos-23.4.9/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_errors.py` & `pontos-23.4.9/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_helper.py` & `pontos-23.4.9/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_main.py` & `pontos-23.4.9/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_parser.py` & `pontos-23.4.9/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_project.py` & `pontos-23.4.9/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/tests/version/test_version.py` & `pontos-23.4.9/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.8/PKG-INFO` & `pontos-23.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.8
+Version: 23.4.9
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

