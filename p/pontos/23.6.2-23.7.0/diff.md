# Comparing `tmp/pontos-23.6.2.tar.gz` & `tmp/pontos-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.6.2.tar", max compression
+gzip compressed data, was "pontos-23.7.0.tar", max compression
```

## Comparing `pontos-23.6.2.tar` & `pontos-23.7.0.tar`

### file list

```diff
@@ -1,253 +1,254 @@
--rw-r--r--   0        0        0    35149 2023-06-29 09:25:08.849093 pontos-23.6.2/LICENSE
--rw-r--r--   0        0        0     3836 2023-06-29 09:25:08.849093 pontos-23.6.2/README.md
--rw-r--r--   0        0        0   110365 2023-06-29 09:25:08.853093 pontos-23.6.2/poetry.lock
--rw-r--r--   0        0        0       32 2023-06-29 09:25:08.853093 pontos-23.6.2/poetry.toml
--rw-r--r--   0        0        0      791 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9995 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7327 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-06-29 09:25:08.853093 pontos-23.6.2/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4732 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/api.py
--rw-r--r--   0        0        0     2177 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     7339 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2646 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    11470 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/parser.py
--rw-r--r--   0        0        0    14408 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12149 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1596 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6445 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_java.py
--rw-r--r--   0        0        0     6365 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-06-29 09:25:08.857093 pontos-23.6.2/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-06-29 09:25:08.861093 pontos-23.6.2/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-06-29 09:25:08.861093 pontos-23.6.2/pontos/version/version.py
--rw-r--r--   0        0        0     2911 2023-06-29 09:25:08.861093 pontos-23.6.2/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-06-29 09:25:08.861093 pontos-23.6.2/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17925 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5430 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-06-29 09:25:08.861093 pontos-23.6.2/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15848 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    11614 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_java.py
--rw-r--r--   0        0        0    17081 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25664 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-06-29 09:25:08.865093 pontos-23.6.2/tests/version/test_version.py
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-03 08:55:56.699958 pontos-23.7.0/LICENSE
+-rw-r--r--   0        0        0     3836 2023-07-03 08:55:56.699958 pontos-23.7.0/README.md
+-rw-r--r--   0        0        0   110395 2023-07-03 08:55:56.703958 pontos-23.7.0/poetry.lock
+-rw-r--r--   0        0        0       32 2023-07-03 08:55:56.703958 pontos-23.7.0/poetry.toml
+-rw-r--r--   0        0        0      791 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9995 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4396 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-07-03 08:55:56.703958 pontos-23.7.0/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     5403 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/script/parser.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/__init__.py
+-rw-r--r--   0        0        0     1872 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/members.py
+-rw-r--r--   0        0        0     2179 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/repositories.py
+-rw-r--r--   0        0        0     6717 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/teams.py
+-rw-r--r--   0        0        0     2789 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/github/scripts/workflow-runs.py
+-rw-r--r--   0        0        0    14685 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4732 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2177 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     7339 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2646 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    11470 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/parser.py
+-rw-r--r--   0        0        0    14408 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/release.py
+-rw-r--r--   0        0        0    12463 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-07-03 08:55:56.707959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12149 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1596 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2871 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7901 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3816 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6591 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_java.py
+-rw-r--r--   0        0        0     6512 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8414 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-07-03 08:55:56.711959 pontos-23.7.0/pontos/version/version.py
+-rw-r--r--   0        0        0     2865 2023-07-03 08:55:56.711959 pontos-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1518 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17925 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-07-03 08:55:56.711959 pontos-23.7.0/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3863 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-07-03 08:55:56.715960 pontos-23.7.0/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15848 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    11614 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_java.py
+-rw-r--r--   0        0        0    17081 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16677 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25664 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-07-03 08:55:56.719960 pontos-23.7.0/tests/version/test_version.py
+-rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.7.0/PKG-INFO
```

### Comparing `pontos-23.6.2/LICENSE` & `pontos-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/README.md` & `pontos-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/poetry.lock` & `pontos-23.7.0/poetry.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1135,29 +1135,30 @@
 pygments = ">=2.13.0,<3.0.0"
 
 [package.extras]
 jupyter = ["ipywidgets (>=7.5.1,<9)"]
 
 [[package]]
 name = "rope"
-version = "1.8.0"
+version = "1.9.0"
 description = "a python refactoring library..."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "rope-1.8.0-py3-none-any.whl", hash = "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd"},
-    {file = "rope-1.8.0.tar.gz", hash = "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"},
+    {file = "rope-1.9.0-py3-none-any.whl", hash = "sha256:2ed32d72cd2c4395bb1d569e38fd4f15d6080cfadd61b6e5c565fd39e3f677aa"},
+    {file = "rope-1.9.0.tar.gz", hash = "sha256:f48d708132c0e062b411308732ca13933b976486b4b53d1e804f94ed08d69503"},
 ]
 
 [package.dependencies]
 pytoolconfig = {version = ">=1.2.2", extras = ["global"]}
 
 [package.extras]
-dev = ["build (>=0.7.0)", "pip-tools (>=6.12.1)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)", "toml (>=0.10.2)"]
+dev = ["build (>=0.7.0)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)"]
 doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
+release = ["pip-tools (>=6.12.1)", "toml (>=0.10.2)", "twine (>=4.0.2)"]
 
 [[package]]
 name = "semver"
 version = "3.0.1"
 description = "Python helper for Semantic Versioning (https://semver.org)"
 optional = false
 python-versions = ">=3.7"
@@ -1410,21 +1411,21 @@
     {file = "tornado-6.3.2-cp38-abi3-win32.whl", hash = "sha256:7efcbcc30b7c654eb6a8c9c9da787a851c18f8ccd4a5a3a95b05c7accfa068d2"},
     {file = "tornado-6.3.2-cp38-abi3-win_amd64.whl", hash = "sha256:0c325e66c8123c606eea33084976c832aa4e766b7dff8aedd7587ea44a604cdf"},
     {file = "tornado-6.3.2.tar.gz", hash = "sha256:4b927c4f19b71e627b13f3db2324e4ae660527143f9e1f2e2fb404f3a187e2ba"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.6.3"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
-    {file = "typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "2.0.3"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 optional = false
@@ -1538,8 +1539,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "51dc5a3613b66d7e6b27730328d591479c920e148b95bf94b37f5f17be6ee117"
+content-hash = "d4878b00c9044f468f56232f9711780ccf479f6ca6f0e3f3749d07669fd97f48"
```

### Comparing `pontos-23.6.2/pontos/__init__.py` & `pontos-23.7.0/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/changelog/__init__.py` & `pontos-23.7.0/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/changelog/conventional_commits.py` & `pontos-23.7.0/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/changelog/errors.py` & `pontos-23.7.0/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/changelog/main.py` & `pontos-23.7.0/pontos/changelog/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                 next_version=parsed_args.next_version,
             )
         else:
             changelog = changelog_builder.create_changelog(
                 last_version=last_version,
                 next_version=parsed_args.next_version,
             )
-            print(changelog)
+            term.out(changelog)
     except PontosError as e:
         term.error(str(e))
         sys.exit(1)
 
     sys.exit(0)
```

### Comparing `pontos-23.6.2/pontos/errors.py` & `pontos-23.7.0/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/git/__init__.py` & `pontos-23.7.0/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/git/git.py` & `pontos-23.7.0/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/git/status.py` & `pontos-23.7.0/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/__init__.py` & `pontos-23.7.0/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/__init__.py` & `pontos-23.7.0/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/argparser.py` & `pontos-23.7.0/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/cmds.py` & `pontos-23.7.0/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/core.py` & `pontos-23.7.0/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/env.py` & `pontos-23.7.0/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/errors.py` & `pontos-23.7.0/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/event.py` & `pontos-23.7.0/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/actions/main.py` & `pontos-23.7.0/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/__init__.py` & `pontos-23.7.0/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/api.py` & `pontos-23.7.0/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/artifacts.py` & `pontos-23.7.0/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/branch.py` & `pontos-23.7.0/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/client.py` & `pontos-23.7.0/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/contents.py` & `pontos-23.7.0/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/errors.py` & `pontos-23.7.0/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/helper.py` & `pontos-23.7.0/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/labels.py` & `pontos-23.7.0/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/organizations.py` & `pontos-23.7.0/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/pull_requests.py` & `pontos-23.7.0/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/release.py` & `pontos-23.7.0/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/repositories.py` & `pontos-23.7.0/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/search.py` & `pontos-23.7.0/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/tags.py` & `pontos-23.7.0/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/teams.py` & `pontos-23.7.0/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/api/workflows.py` & `pontos-23.7.0/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/argparser.py` & `pontos-23.7.0/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/cmds.py` & `pontos-23.7.0/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/main.py` & `pontos-23.7.0/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/__init__.py` & `pontos-23.7.0/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/artifact.py` & `pontos-23.7.0/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/base.py` & `pontos-23.7.0/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/branch.py` & `pontos-23.7.0/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/organization.py` & `pontos-23.7.0/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/pull_request.py` & `pontos-23.7.0/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/release.py` & `pontos-23.7.0/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/search.py` & `pontos-23.7.0/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/tag.py` & `pontos-23.7.0/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/models/workflow.py` & `pontos-23.7.0/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/pr_template.md` & `pontos-23.7.0/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/script/__init__.py` & `pontos-23.7.0/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/script/errors.py` & `pontos-23.7.0/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/github/script/load.py` & `pontos-23.7.0/pontos/github/script/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,22 +49,30 @@
     Example:
         .. code-block:: python
 
             from pontos.github.script import load_script
 
             with load_script("path/to/script.py") as module:
                 module.func()
+
+            with load_script("some.python.module") as module:
+                module.func()
     """
     path = Path(script)
-    module_name = path.stem
+    if path.suffix == ".py":
+        module_name = path.stem
 
-    with add_sys_path(path.parent.absolute()), ensure_unload_module(
-        module_name
-    ):
-        yield importlib.import_module(module_name)
+        with add_sys_path(path.parent.absolute()), ensure_unload_module(
+            module_name
+        ):
+            yield importlib.import_module(module_name)
+    else:
+        module_name = str(path)
+        with ensure_unload_module(module_name):
+            yield importlib.import_module(module_name)
 
 
 def run_github_script_function(
     module: ModuleType, token: str, timeout: float, args: Namespace
 ) -> int:
     """
     Run a github_script function from a Python module
@@ -88,14 +96,17 @@
             from pontos.github.script import (
                 load_script,
                 run_github_script_function,
             )
 
             with load_script("path/to/script.py") as module:
                 return run_github_script_function(module, token, 60.0, args)
+
+            with load_script("some.python.module") as module:
+                return run_github_script_function(module, token, 60.0, args)
     """
     if not hasattr(module, GITHUB_SCRIPT_FUNCTION_NAME):
         raise GitHubScriptError(
             f"{module.__file__} is not a valid Pontos GitHub Script. A "
             f"{GITHUB_SCRIPT_FUNCTION_NAME} function is missing."
         )
     func = getattr(module, GITHUB_SCRIPT_FUNCTION_NAME)
@@ -148,11 +159,14 @@
                 run_github_script_function,
             )
 
             parser = ArgumentParser()
 
             with load_script("path/to/script.py") as module:
                 run_add_arguments_function(module, parser)
+
+            with load_script("some.python.module") as module:
+                run_add_arguments_function(module, parser)
     """
     func = getattr(module, GITHUB_SCRIPT_PARSER_FUNCTION_NAME, None)
     if func:
         func(parser)
```

### Comparing `pontos-23.6.2/pontos/github/script/parser.py` & `pontos-23.7.0/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/helper.py` & `pontos-23.7.0/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/models/__init__.py` & `pontos-23.7.0/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/__init__.py` & `pontos-23.7.0/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/api.py` & `pontos-23.7.0/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/cpe/__init__.py` & `pontos-23.7.0/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/cpe/api.py` & `pontos-23.7.0/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/cve/__init__.py` & `pontos-23.7.0/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/cve/api.py` & `pontos-23.7.0/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/models/__init__.py` & `pontos-23.7.0/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/models/cpe.py` & `pontos-23.7.0/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/models/cve.py` & `pontos-23.7.0/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/models/cvss_v2.py` & `pontos-23.7.0/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/nvd/models/cvss_v3.py` & `pontos-23.7.0/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/pontos.py` & `pontos-23.7.0/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/release/__init__.py` & `pontos-23.7.0/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/release/helper.py` & `pontos-23.7.0/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/release/main.py` & `pontos-23.7.0/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/release/parser.py` & `pontos-23.7.0/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/release/release.py` & `pontos-23.7.0/pontos/release/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/release/sign.py` & `pontos-23.7.0/pontos/release/sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,17 +218,15 @@
             # required # for public repositories.
             self.terminal.error(
                 "Token is missing. The GitHub token is required to upload "
                 "signature files."
             )
             return SignReturnValue.TOKEN_MISSING
 
-        self.terminal.info(
-            f"Using versioning scheme {versioning_scheme.__class__.__name__}"
-        )
+        self.terminal.info(f"Using versioning scheme {versioning_scheme.name}")
 
         try:
             project = (
                 project if project is not None else get_git_repository_name()
             )
         except GitError as e:
             self.terminal.error(f"Could not determine project. {e}")
```

### Comparing `pontos-23.6.2/pontos/terminal/__init__.py` & `pontos-23.7.0/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/terminal/null.py` & `pontos-23.7.0/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/terminal/rich.py` & `pontos-23.7.0/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/terminal/terminal.py` & `pontos-23.7.0/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/testing/__init__.py` & `pontos-23.7.0/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/updateheader/__init__.py` & `pontos-23.7.0/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/updateheader/__main__.py` & `pontos-23.7.0/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/updateheader/updateheader.py` & `pontos-23.7.0/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/__init__.py` & `pontos-23.7.0/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/__main__.py` & `pontos-23.7.0/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/_calculator.py` & `pontos-23.7.0/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/commands/__init__.py` & `pontos-23.7.0/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/commands/_cargo.py` & `pontos-23.7.0/pontos/version/commands/_cargo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
-from typing import Iterator, Tuple, Union, Literal
+from typing import Iterator, Literal, Tuple, Union
 
 import tomlkit
 
+from ..errors import VersionError
 from ..version import Version, VersionUpdate
 from ._command import VersionCommand
-from ..errors import VersionError
 
 
 class CargoVersionCommand(VersionCommand):
     project_file_name = "Cargo.toml"
 
     def __as_project_document(
         self, origin: Path
@@ -36,18 +36,22 @@
                         origin.parent / member / self.project_file_name
                     )
         return None
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
-        previous_version = self.get_current_version()
+        try:
+            previous_version = self.get_current_version()
 
-        if not force and new_version == previous_version:
-            return VersionUpdate(previous=previous_version, new=new_version)
+            if not force and new_version == previous_version:
+                return VersionUpdate(previous=previous_version, new=new_version)
+        except VersionError:
+            # just ignore current version and override it
+            previous_version = None
 
         changed_files = []
         for project_path, project in self.__as_project_document(
             self.project_file_path
         ):
             project["package"]["version"] = str(new_version)
             project_path.write_text(tomlkit.dumps(project))
```

### Comparing `pontos-23.6.2/pontos/version/commands/_cmake.py` & `pontos-23.7.0/pontos/version/commands/_cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,18 +29,23 @@
     project_file_name = "CMakeLists.txt"
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
         content = self.project_file_path.read_text(encoding="utf-8")
         cmake_version_parser = CMakeVersionParser(content)
-        previous_version = self.get_current_version()
 
-        if not force and new_version == previous_version:
-            return VersionUpdate(previous=previous_version, new=new_version)
+        try:
+            previous_version = self.get_current_version()
+
+            if not force and new_version == previous_version:
+                return VersionUpdate(previous=previous_version, new=new_version)
+        except VersionError:
+            # just ignore current version and override it
+            previous_version = None
 
         new_content = cmake_version_parser.update_version(new_version)
         self.project_file_path.write_text(new_content, encoding="utf-8")
         return VersionUpdate(
             previous=previous_version,
             new=new_version,
             changed_files=[self.project_file_path],
```

### Comparing `pontos-23.6.2/pontos/version/commands/_command.py` & `pontos-23.7.0/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/commands/_go.py` & `pontos-23.7.0/pontos/version/commands/_go.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,21 +88,20 @@
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
         """Update the current version of this project"""
         try:
             current_version = self.get_current_version()
+            if not force and new_version == current_version:
+                return VersionUpdate(previous=current_version, new=new_version)
         except VersionError:
-            # likely the initial release
+            # just ignore current version and override it
             current_version = None
 
-        if not force and new_version == current_version:
-            return VersionUpdate(previous=current_version, new=new_version)
-
         self._update_version_file(new_version=new_version)
 
         return VersionUpdate(
             previous=current_version,
             new=new_version,
             changed_files=[self.version_file_path],
         )
```

### Comparing `pontos-23.6.2/pontos/version/commands/_java.py` & `pontos-23.7.0/pontos/version/commands/_java.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 __version__ = "{}"\n"""
 
 
 def find_file(
     filename: Path, search_path: str, search_glob: str
 ) -> Optional[Path]:
-    """Find a file somewherre within an directory tree
+    """Find a file somewhere within an directory tree
     Arguments:
         filename (Path)     The file to look up
         search_path (str)   The path to look for the file
         search_glob (str)   The glob search pattern
 
     Returns:
     The file as Path object, if existing"""
@@ -176,17 +176,21 @@
                 f"current version {current_version} in "
                 f"{self.project_file_path}."
             )
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
-        package_version = self.get_current_version()
-        if not force and new_version == package_version:
-            return VersionUpdate(previous=package_version, new=new_version)
+        try:
+            package_version = self.get_current_version()
+            if not force and new_version == package_version:
+                return VersionUpdate(previous=package_version, new=new_version)
+        except VersionError:
+            # just ignore current version and override it
+            package_version = None
 
         changed_files = [self.project_file_path]
         self._update_pom_version(new_version=new_version)
         self._update_properties_file(new_version=new_version)
         self._update_swagger_config(new_version=new_version)
 
         return VersionUpdate(
```

### Comparing `pontos-23.6.2/pontos/version/commands/_javascript.py` & `pontos-23.7.0/pontos/version/commands/_javascript.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,21 @@
         content = content.replace(match.group("version"), str(new_version))
         version_file.write_text(content, encoding="utf-8")
         return True
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
-        package_version = self.get_current_version()
-        if not force and new_version == package_version:
-            return VersionUpdate(previous=package_version, new=new_version)
+        try:
+            package_version = self.get_current_version()
+            if not force and new_version == package_version:
+                return VersionUpdate(previous=package_version, new=new_version)
+        except VersionError:
+            # just ignore current version and override it
+            package_version = None
 
         changed_files = [self.project_file_path]
         self._update_package_json(new_version=new_version)
 
         for version_file in self.version_file_paths:
             updated = self._update_version_file(
                 version_file, new_version=new_version
```

### Comparing `pontos-23.6.2/pontos/version/commands/_python.py` & `pontos-23.7.0/pontos/version/commands/_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,31 +181,36 @@
                     f"Provided version {version} does not match the "
                     f"current version {current_version}."
                 )
 
     def update_version(
         self, new_version: Version, *, force: bool = False
     ) -> VersionUpdate:
-        try:
-            current_version = self.get_current_version()
-        except VersionError:
-            # maybe no version module exists yet. fallback to version from
-            # pyproject.toml
-            current_version = self._get_version_from_pyproject_toml()
-
         new_pep440_version = PEP440VersioningScheme.from_version(new_version)
-        current_converted_version = self.versioning_scheme.from_version(
-            current_version
-        )
 
-        if not force and new_pep440_version == current_version:
-            return VersionUpdate(
-                previous=current_converted_version, new=new_version
+        try:
+            try:
+                current_version = self.get_current_version()
+            except VersionError:
+                # maybe no version module exists yet. fallback to version from
+                # pyproject.toml
+                current_version = self._get_version_from_pyproject_toml()
+
+            current_converted_version = self.versioning_scheme.from_version(
+                current_version
             )
 
+            if not force and new_pep440_version == current_version:
+                return VersionUpdate(
+                    previous=current_converted_version, new=new_version
+                )
+        except VersionError:
+            # just ignore current version and override it
+            current_converted_version = None
+
         try:
             self._update_pyproject_version(new_version=new_pep440_version)
         except OSError as e:
             raise VersionError(
                 "Unable to update version in "
                 f"{self.project_file_path.absolute()}. Error was {e}"
             ) from e
```

### Comparing `pontos-23.6.2/pontos/version/errors.py` & `pontos-23.7.0/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/helper.py` & `pontos-23.7.0/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/main.py` & `pontos-23.7.0/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/parser.py` & `pontos-23.7.0/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/project.py` & `pontos-23.7.0/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/schemes/__init__.py` & `pontos-23.7.0/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/schemes/_pep440.py` & `pontos-23.7.0/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/schemes/_scheme.py` & `pontos-23.7.0/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/schemes/_semantic.py` & `pontos-23.7.0/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pontos/version/version.py` & `pontos-23.7.0/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/pyproject.toml` & `pontos-23.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.6.2"
+version = "23.7.0"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -23,15 +23,14 @@
 ]
 
 packages = [
   { include = "pontos"},
   { include = "tests", format = "sdist" },
   { include = "poetry.lock", format = "sdist" },
   { include = "poetry.toml", format = "sdist" },
-  { include = "scripts/", format = "sdist" },
 ]
 include = [
   "pontos/updateheader/templates/",
   "pontos/github/pr_template.md"
 ]
 
 [tool.poetry.dependencies]
@@ -47,15 +46,15 @@
 lxml = "^4.9.0"
 
 [tool.poetry.dev-dependencies]
 autohooks = ">=22.7.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-isort = ">=22.3.0"
-rope = "^1.8.0"
+rope = "^1.9.0"
 coverage = "^7.2"
 myst-parser = ">=0.19.1"
 Sphinx = "^7.0.1"
 furo = "^2023.5.20"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.black]
```

### Comparing `pontos-23.6.2/scripts/github/artifacts-download.py` & `pontos-23.7.0/pontos/github/scripts/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/artifacts.py` & `pontos-23.7.0/pontos/github/scripts/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/branchprotection.py` & `pontos-23.7.0/pontos/github/scripts/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/create-repository.py` & `pontos-23.7.0/pontos/github/scripts/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/enforce-admins.py` & `pontos-23.7.0/pontos/github/scripts/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/lock-branch.py` & `pontos-23.7.0/pontos/github/scripts/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/members.py` & `pontos-23.7.0/pontos/github/scripts/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/release-assets-download.py` & `pontos-23.7.0/pontos/github/scripts/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/repositories.py` & `pontos-23.7.0/pontos/github/scripts/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/search-repositories.py` & `pontos-23.7.0/pontos/github/scripts/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/team-repositories.py` & `pontos-23.7.0/pontos/github/scripts/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/teams.py` & `pontos-23.7.0/pontos/github/scripts/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/scripts/github/workflow-runs.py` & `pontos-23.7.0/pontos/github/scripts/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/__init__.py` & `pontos-23.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/changelog/__init__.py` & `pontos-23.7.0/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/changelog/test_conventional_commits.py` & `pontos-23.7.0/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/changelog/test_parser.py` & `pontos-23.7.0/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/git/__init__.py` & `pontos-23.7.0/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/git/test_git.py` & `pontos-23.7.0/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/git/test_status.py` & `pontos-23.7.0/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/__init__.py` & `pontos-23.7.0/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/actions/__init__.py` & `pontos-23.7.0/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/actions/test-pull-request-event.json` & `pontos-23.7.0/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/actions/test_core.py` & `pontos-23.7.0/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/actions/test_env.py` & `pontos-23.7.0/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/actions/test_event.py` & `pontos-23.7.0/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/__init__.py` & `pontos-23.7.0/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/pr-files.json` & `pontos-23.7.0/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/release-response.json` & `pontos-23.7.0/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_artifacts.py` & `pontos-23.7.0/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_branch.py` & `pontos-23.7.0/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_client.py` & `pontos-23.7.0/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_contents.py` & `pontos-23.7.0/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_labels.py` & `pontos-23.7.0/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_organizations.py` & `pontos-23.7.0/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_pull_requests.py` & `pontos-23.7.0/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_release.py` & `pontos-23.7.0/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_repositories.py` & `pontos-23.7.0/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_search.py` & `pontos-23.7.0/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_tags.py` & `pontos-23.7.0/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_teams.py` & `pontos-23.7.0/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/api/test_workflows.py` & `pontos-23.7.0/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/__init__.py` & `pontos-23.7.0/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_artifact.py` & `pontos-23.7.0/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_base.py` & `pontos-23.7.0/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_branch.py` & `pontos-23.7.0/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_organization.py` & `pontos-23.7.0/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_pull_request.py` & `pontos-23.7.0/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_release.py` & `pontos-23.7.0/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_search.py` & `pontos-23.7.0/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_tag.py` & `pontos-23.7.0/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/models/test_workflow.py` & `pontos-23.7.0/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/script/__init__.py` & `pontos-23.7.0/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/script/test_load.py` & `pontos-23.7.0/tests/github/script/test_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,27 +22,35 @@
 
 from pontos.github.script.errors import GitHubScriptError
 from pontos.github.script.load import (
     load_script,
     run_add_arguments_function,
     run_github_script_function,
 )
-from pontos.testing import temp_file
+from pontos.testing import temp_file, temp_python_module
 from tests import IsolatedAsyncioTestCase
 
 
 class LoadScriptTestCase(unittest.TestCase):
     def test_load_script(self):
         with temp_file(
             "def foo():\n\treturn 1", name="foo.py"
         ) as f, load_script(f) as module:
             self.assertIsNotNone(module)
             self.assertIsNotNone(module.foo)
             self.assertEqual(module.foo(), 1)
 
+    def test_load_script_module(self):
+        with temp_python_module(
+            "def foo():\n\treturn 1", name="github-foo-script"
+        ), load_script("github-foo-script") as module:
+            self.assertIsNotNone(module)
+            self.assertIsNotNone(module.foo)
+            self.assertEqual(module.foo(), 1)
+
     def test_load_script_failure(self):
         with self.assertRaisesRegex(
             ModuleNotFoundError, "No module named 'baz'"
         ):
             with load_script("foo/bar/baz.py"):
                 pass
```

### Comparing `pontos-23.6.2/tests/github/script/test_parser.py` & `pontos-23.7.0/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/test_argparser.py` & `pontos-23.7.0/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/github/test_cmds.py` & `pontos-23.7.0/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/models/__init__.py` & `pontos-23.7.0/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/models/test_models.py` & `pontos-23.7.0/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/__init__.py` & `pontos-23.7.0/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/cpe/__init__.py` & `pontos-23.7.0/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/cpe/test_api.py` & `pontos-23.7.0/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/cve/__init__.py` & `pontos-23.7.0/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/cve/test_api.py` & `pontos-23.7.0/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/models/__init__.py` & `pontos-23.7.0/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/models/test_cpe.py` & `pontos-23.7.0/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/models/test_cve.py` & `pontos-23.7.0/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/nvd/test_api.py` & `pontos-23.7.0/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/release/__init__.py` & `pontos-23.7.0/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/release/test_helper.py` & `pontos-23.7.0/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/release/test_parser.py` & `pontos-23.7.0/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/release/test_release.py` & `pontos-23.7.0/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/release/test_sign.py` & `pontos-23.7.0/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/terminal/__init__.py` & `pontos-23.7.0/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/terminal/test_terminal.py` & `pontos-23.7.0/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/test_helper.py` & `pontos-23.7.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/test_pontos.py` & `pontos-23.7.0/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/testing/__init__.py` & `pontos-23.7.0/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/testing/test_testing.py` & `pontos-23.7.0/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/updateheader/__init__.py` & `pontos-23.7.0/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/updateheader/test_header.py` & `pontos-23.7.0/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/__init__.py` & `pontos-23.7.0/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/__init__.py` & `pontos-23.7.0/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/test_cargo.py` & `pontos-23.7.0/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/test_cmake.py` & `pontos-23.7.0/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/test_go.py` & `pontos-23.7.0/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/test_java.py` & `pontos-23.7.0/tests/version/commands/test_java.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/test_javascript.py` & `pontos-23.7.0/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/commands/test_python.py` & `pontos-23.7.0/tests/version/commands/test_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,26 +151,26 @@
         self.assertEqual(version_line, '__version__ = "22.2"')
 
     def test_empty_pyproject_toml(self):
         with temp_file(
             "", name="pyproject.toml", change_into=True
         ), self.assertRaisesRegex(
             VersionError,
-            r"Version information not found in .*pyproject\.toml file\.",
+            r"\[tool.pontos.version\] section missing in .*pyproject\.toml\.",
         ):
             cmd = PythonVersionCommand(PEP440VersioningScheme)
             new_version = PEP440VersioningScheme.parse_version("22.1.2")
             cmd.update_version(new_version)
 
     def test_empty_tool_section(self):
         with temp_file(
             "[tool]", name="pyproject.toml", change_into=True
         ), self.assertRaisesRegex(
             VersionError,
-            r"Version information not found in .*pyproject\.toml file\.",
+            r"\[tool.pontos.version\] section missing in .*pyproject\.toml\.",
         ):
             cmd = PythonVersionCommand(PEP440VersioningScheme)
             new_version = PEP440VersioningScheme.parse_version("22.1.2")
             cmd.update_version(new_version)
 
     def test_empty_tool_poetry_section(self):
         content = "__version__ = '22.1'"
```

### Comparing `pontos-23.6.2/tests/version/schemes/__init__.py` & `pontos-23.7.0/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/schemes/test_pep440.py` & `pontos-23.7.0/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/schemes/test_semantic.py` & `pontos-23.7.0/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_commands.py` & `pontos-23.7.0/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_errors.py` & `pontos-23.7.0/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_helper.py` & `pontos-23.7.0/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_main.py` & `pontos-23.7.0/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_parser.py` & `pontos-23.7.0/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_project.py` & `pontos-23.7.0/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/tests/version/test_version.py` & `pontos-23.7.0/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.2/PKG-INFO` & `pontos-23.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.6.2
+Version: 23.7.0
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

