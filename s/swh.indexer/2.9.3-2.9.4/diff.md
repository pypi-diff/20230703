# Comparing `tmp/swh.indexer-2.9.3.tar.gz` & `tmp/swh.indexer-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.indexer-2.9.3.tar", last modified: Mon Feb 13 10:03:47 2023, max compression
+gzip compressed data, was "dist/swh.indexer-2.9.4.tar", last modified: Mon Apr 17 14:37:24 2023, max compression
```

## Comparing `swh.indexer-2.9.3.tar` & `swh.indexer-2.9.4.tar`

### file list

```diff
@@ -1,195 +1,197 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      173 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      909 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       71 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      233 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)     1149 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/codemeta.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1086 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       64 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      155 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      151 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4896 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/dev-info.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)       28 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      194 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2842 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/images/tasks-metadata-indexers.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      539 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    10881 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/docs/metadata-workflow.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      593 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       99 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      138 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      145 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      238 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2320 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1741 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/bin/db-upgrade
--rwxr-xr-x   0 jenkins    (115) docker     (999)      393 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/bin/dot_add_content
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/doc/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/doc/json/
--rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      269 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/indexer_configuration.tool_configuration.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/doc/json/revision_metadata.translated_metadata.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/sql/json/
--rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      269 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/indexer_configuration.tool_configuration.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1283 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/sql/json/revision_metadata.translated_metadata.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/
--rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12476 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7466 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/codemeta.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     1030 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/Gitea.csv
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/
--rw-r--r--   0 jenkins    (115) docker     (999)      490 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/CITATION
--rw-r--r--   0 jenkins    (115) docker     (999)    10253 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)     4362 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/codemeta.jsonld
--rw-r--r--   0 jenkins    (115) docker     (999)    14995 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/codemeta/crosswalk.csv
--rw-r--r--   0 jenkins    (115) docker     (999)     1023 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/composer.csv
--rw-r--r--   0 jenkins    (115) docker     (999)      990 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/nuget.csv
--rw-r--r--   0 jenkins    (115) docker     (999)     1019 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/data/pubspec.csv
--rw-r--r--   0 jenkins    (115) docker     (999)     5921 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/fossology_license.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24988 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/indexer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1644 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20357 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)      954 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_detector.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/
--rw-r--r--   0 jenkins    (115) docker     (999)     2005 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14971 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2461 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/cff.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7872 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/codemeta.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1897 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/composer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2178 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/dart.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4534 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5037 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/github.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6056 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/maven.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10946 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/npm.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3311 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/nuget.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2793 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/python.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4568 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/ruby.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3788 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/metadata_dictionary/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4863 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/mimetype.py
--rw-r--r--   0 jenkins    (115) docker     (999)      544 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/namespaces.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5933 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/origin_head.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/rehash.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      121 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5728 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/50-data.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    12719 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/50-func.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)     1301 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/115.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3665 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/116.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      530 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/117.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      432 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/118.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2930 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/119.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2284 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/120.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      475 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/121.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/122.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3743 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/123.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      387 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/124.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1568 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/125.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1677 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/126.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2734 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/127.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      311 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/128.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3718 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/129.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1506 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/130.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     7560 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/131.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1618 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/132.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5324 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/133.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6879 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/134.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4417 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/135.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6094 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/136.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      607 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/sql/upgrades/137.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/storage/
--rw-r--r--   0 jenkins    (115) docker     (999)    24539 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/storage/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      806 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3365 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1486 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14976 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)      598 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16262 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13021 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2197 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2398 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/storage/writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1438 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      349 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4019 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5712 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_cff.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18435 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_codemeta.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2125 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_composer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3965 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_dart.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4209 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5419 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_github.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13207 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_maven.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13676 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_npm.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5961 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_nuget.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3600 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_python.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4433 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_ruby.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/
--rw-r--r--   0 jenkins    (115) docker     (999)      351 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2736 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5198 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/generate_data_test.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3768 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2229 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)      522 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3262 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1728 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1702 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3966 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    63148 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/storage/test_storage.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1325 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    26663 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7747 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_codemeta.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4714 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_fossology_license.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7625 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_indexer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4045 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16076 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4288 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_mimetype.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8300 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_origin_head.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12457 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/test_origin_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)    23669 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/README
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3185 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/swh/indexer/tests/zz_celery/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh.indexer.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     5398 2023-02-13 10:03:47.000000 swh.indexer-2.9.3/swh.indexer.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      379 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-02-13 10:03:46.000000 swh.indexer-2.9.3/swh.indexer.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1641 2023-02-13 10:03:45.000000 swh.indexer-2.9.3/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      173 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      909 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       71 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      233 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)     1149 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/codemeta.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1086 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       64 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      155 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      151 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4896 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/dev-info.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)       28 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      194 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1138 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/images/tasks-extrinsic-metadata-indexers.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     2959 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/images/tasks-intrinsic-metadata-indexers.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      553 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    10995 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/metadata-workflow.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4055 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/docs/swhpkg.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      593 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       99 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      138 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      145 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      238 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2320 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/sql/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/sql/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1741 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/bin/db-upgrade
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      393 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/bin/dot_add_content
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/sql/doc/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/sql/doc/json/
+-rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/doc/json/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/doc/json/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      269 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/doc/json/indexer_configuration.tool_configuration.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1283 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/doc/json/revision_metadata.translated_metadata.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/sql/json/
+-rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/json/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/json/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      269 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/json/indexer_configuration.tool_configuration.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1283 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/sql/json/revision_metadata.translated_metadata.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/
+-rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12476 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7466 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/codemeta.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1030 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/Gitea.csv
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/data/codemeta/
+-rw-r--r--   0 jenkins    (115) docker     (999)      490 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/codemeta/CITATION
+-rw-r--r--   0 jenkins    (115) docker     (999)    10253 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/codemeta/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)     4362 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/codemeta/codemeta.jsonld
+-rw-r--r--   0 jenkins    (115) docker     (999)    14995 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/codemeta/crosswalk.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)     1023 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/composer.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)      990 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/nuget.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)     1019 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/data/pubspec.csv
+-rw-r--r--   0 jenkins    (115) docker     (999)     5921 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/fossology_license.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    24988 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/indexer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1644 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20357 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      954 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_detector.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2005 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15139 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2517 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/cff.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7872 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/codemeta.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1897 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/composer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2234 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/dart.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4534 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5037 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6056 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/maven.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10946 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/npm.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3045 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/nuget.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2793 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/python.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4236 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/ruby.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3788 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/metadata_dictionary/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4863 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/mimetype.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      544 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/namespaces.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5933 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/origin_head.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/rehash.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      121 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5728 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/50-data.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    12719 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/50-func.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1301 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/115.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3665 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/116.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      530 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/117.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      432 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/118.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2930 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/119.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2284 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/120.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      475 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/121.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/122.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3743 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/123.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      387 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/124.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1568 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/125.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1677 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/126.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2734 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/127.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      311 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/128.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3718 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/129.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1506 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/130.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     7560 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/131.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1618 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/132.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5324 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/133.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6879 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/134.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4417 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/135.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6094 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/136.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      607 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/sql/upgrades/137.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/storage/
+-rw-r--r--   0 jenkins    (115) docker     (999)    24539 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/storage/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      806 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3365 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1486 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14976 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      598 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16262 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13021 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2197 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2398 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/storage/writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1438 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      349 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4019 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5712 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_cff.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18435 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_codemeta.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2125 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_composer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4050 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_dart.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4209 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5419 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13207 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_maven.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13676 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_npm.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5961 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_nuget.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3600 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_python.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4433 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_ruby.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/
+-rw-r--r--   0 jenkins    (115) docker     (999)      351 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2736 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5198 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/generate_data_test.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3768 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2229 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      522 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3262 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1728 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1702 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3966 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    63148 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/storage/test_storage.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1325 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    26663 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7747 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_codemeta.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4714 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_fossology_license.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7625 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_indexer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4045 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16076 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4288 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_mimetype.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8300 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_origin_head.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12457 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/test_origin_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    23669 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh/indexer/tests/zz_celery/
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/zz_celery/README
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/zz_celery/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3185 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/swh/indexer/tests/zz_celery/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     5474 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      379 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-17 14:37:24.000000 swh.indexer-2.9.4/swh.indexer.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1617 2023-04-17 14:37:22.000000 swh.indexer-2.9.4/tox.ini
```

### Comparing `swh.indexer-2.9.3/.pre-commit-config.yaml` & `swh.indexer-2.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/CODE_OF_CONDUCT.md` & `swh.indexer-2.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/LICENSE` & `swh.indexer-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/PKG-INFO` & `swh.indexer-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.indexer
-Version: 2.9.3
+Version: 2.9.4
 Summary: Software Heritage Content Indexer
 Home-page: https://forge.softwareheritage.org/diffusion/78/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-indexer
```

### Comparing `swh.indexer-2.9.3/README.md` & `swh.indexer-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/codemeta.json` & `swh.indexer-2.9.4/codemeta.json`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/conftest.py` & `swh.indexer-2.9.4/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/docs/README.md` & `swh.indexer-2.9.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/docs/dev-info.rst` & `swh.indexer-2.9.4/docs/dev-info.rst`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/docs/images/tasks-metadata-indexers.uml` & `swh.indexer-2.9.4/docs/images/tasks-intrinsic-metadata-indexers.uml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 @startuml
   participant LOADERS as "Loaders"
+  participant STORAGE as "Graph Storage"
   participant JOURNAL as "Journal"
   participant IDX_ORIG_META as "Origin Metadata Indexer"
   participant IDX_ORIG_HEAD as "Origin-Head Indexer"
   participant IDX_DIR_META as "Directory Metadata Indexer"
   participant IDX_CONT_META as "Content Metadata Indexer"
   participant IDX_STORAGE as "Indexer Storage"
-  participant STORAGE as "Graph Storage"
   participant OBJ_STORAGE as "Object Storage"
 
   activate OBJ_STORAGE
   activate IDX_STORAGE
   activate STORAGE
   activate JOURNAL
   activate IDX_ORIG_META
 
   activate LOADERS
 
-  LOADERS->>JOURNAL: Origin http://example.org/repo.git\nwas added/revisited
+  LOADERS->>STORAGE: Repository content
+  LOADERS->>STORAGE: Origin http://example.org/repo.git\nwas added/revisited
+  STORAGE->>JOURNAL: Origin http://example.org/repo.git\nwas added/revisited
   deactivate LOADERS
 
   JOURNAL->>IDX_ORIG_META: run indexers on origin\nhttp://example.org/repo.git
 
   IDX_ORIG_META->>IDX_ORIG_HEAD: Find HEAD revision of\nhttp://example.org/repo.git
   activate IDX_ORIG_HEAD
```

### Comparing `swh.indexer-2.9.3/docs/index.rst` & `swh.indexer-2.9.4/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .. toctree::
    :maxdepth: 1
    :caption: Contents:
 
    README.md
    dev-info.rst
    metadata-workflow.rst
+   swhpkg.rst
 
 
 Reference Documentation
 -----------------------
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `swh.indexer-2.9.3/docs/metadata-workflow.rst` & `swh.indexer-2.9.4/docs/metadata-workflow.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 In order to deduplicate the work between origins, we split this work between
 multiple indexers, which coordinate with each other and save their results
 at each step in the indexer storage.
 
 Indexer architecture
 ^^^^^^^^^^^^^^^^^^^^
 
-.. thumbnail:: images/tasks-metadata-indexers.svg
+.. thumbnail:: images/tasks-intrinsic-metadata-indexers.svg
 
 
 Origin-Head Indexer
 ^^^^^^^^^^^^^^^^^^^
 
 First, the Origin-Head indexer gets called externally, with an origin as
 argument (or multiple origins, that are handled sequentially).
@@ -92,14 +92,19 @@
 .. _crosswalk table: https://codemeta.github.io/crosswalk/
 .. _CSV file: https://github.com/codemeta/codemeta/blob/master/crosswalk.csv
 
 
 Extrinsic metadata
 ------------------
 
+Indexer architecture
+^^^^^^^^^^^^^^^^^^^^
+
+.. thumbnail:: images/tasks-extrinsic-metadata-indexers.svg
+
 The :term:`extrinsic metadata` indexer works very differently from
 the :term:`intrinsic metadata` indexers we saw above.
 While the latter extract metadata from software artefacts (files and directories)
 which are already a core part of the archive, the former extracts such data from
 API calls pulled from forges and package managers, or pushed via the
 :ref:`SWORD deposit <swh-deposit>`.
```

### Comparing `swh.indexer-2.9.3/mypy.ini` & `swh.indexer-2.9.4/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/setup.py` & `swh.indexer-2.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/sql/bin/db-upgrade` & `swh.indexer-2.9.4/sql/bin/db-upgrade`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/sql/doc/json/revision_metadata.translated_metadata.json` & `swh.indexer-2.9.4/sql/doc/json/revision_metadata.translated_metadata.json`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/sql/json/revision_metadata.translated_metadata.json` & `swh.indexer-2.9.4/sql/json/revision_metadata.translated_metadata.json`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/cli.py` & `swh.indexer-2.9.4/swh/indexer/cli.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/codemeta.py` & `swh.indexer-2.9.4/swh/indexer/codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/Gitea.csv` & `swh.indexer-2.9.4/swh/indexer/data/Gitea.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/codemeta/LICENSE` & `swh.indexer-2.9.4/swh/indexer/data/codemeta/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/codemeta/codemeta.jsonld` & `swh.indexer-2.9.4/swh/indexer/data/codemeta/codemeta.jsonld`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/codemeta/crosswalk.csv` & `swh.indexer-2.9.4/swh/indexer/data/codemeta/crosswalk.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/composer.csv` & `swh.indexer-2.9.4/swh/indexer/data/composer.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/nuget.csv` & `swh.indexer-2.9.4/swh/indexer/data/nuget.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/data/pubspec.csv` & `swh.indexer-2.9.4/swh/indexer/data/pubspec.csv`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/fossology_license.py` & `swh.indexer-2.9.4/swh/indexer/fossology_license.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/indexer.py` & `swh.indexer-2.9.4/swh/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/journal_client.py` & `swh.indexer-2.9.4/swh/indexer/journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata.py` & `swh.indexer-2.9.4/swh/indexer/metadata.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_detector.py` & `swh.indexer-2.9.4/swh/indexer/metadata_detector.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/__init__.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/base.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2017-2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import json
 import logging
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar
+from typing import Any, Callable, Dict, List, Optional, Pattern, Tuple, TypeVar, Union
 import uuid
 import xml.parsers.expat
 
 from pyld import jsonld
 import rdflib
 from typing_extensions import TypedDict
 import xmltodict
@@ -127,24 +127,29 @@
     def normalize_translation(self, metadata: Dict[str, Any]) -> Dict[str, Any]:
         return compact(metadata, forgefed=False)
 
 
 class SingleFileIntrinsicMapping(BaseIntrinsicMapping):
     """Base class for all intrinsic metadata mappings that use a single file as input."""
 
-    @property
-    def filename(self):
-        """The .json file to extract metadata from."""
-        raise NotImplementedError(f"{self.__class__.__name__}.filename")
+    filename: Union[bytes, Pattern[bytes]]
 
     @classmethod
     def detect_metadata_files(cls, file_entries: List[DirectoryLsEntry]) -> List[Sha1]:
-        for entry in file_entries:
-            if entry["name"].lower() == cls.filename:
-                return [entry["sha1"]]
+        filename = cls.filename
+        # Check if filename is a regex or bytes:
+        if isinstance(filename, bytes):
+            for entry in file_entries:
+                if entry["name"].lower() == filename:
+                    return [entry["sha1"]]
+        else:
+            for entry in file_entries:
+                if filename.match(entry["name"]):
+                    return [entry["sha1"]]
+
         return []
 
 
 class DictMapping(BaseMapping):
     """Base class for mappings that take as input a file that is mostly
     a key-value store (eg. a shallow JSON dict)."""
 
@@ -384,21 +389,21 @@
 class SafeLoader(yaml.SafeLoader):
     yaml_implicit_resolvers = {
         k: [r for r in v if r[0] != "tag:yaml.org,2002:timestamp"]
         for k, v in yaml.SafeLoader.yaml_implicit_resolvers.items()
     }
 
 
-class YamlMapping(DictMapping, SingleFileIntrinsicMapping):
+class YamlMapping(DictMapping):
     """Base class for all mappings that use Yaml data as input."""
 
     def translate(self, raw_content: bytes) -> Optional[Dict[str, str]]:
         raw_content_string: str = raw_content.decode()
         try:
             content_dict = yaml.load(raw_content_string, Loader=SafeLoader)
-        except yaml.scanner.ScannerError:
+        except (yaml.scanner.ScannerError, yaml.parser.ParserError):
             return None
 
         if isinstance(content_dict, dict):
             return self._translate_dict(content_dict)
 
         return None
```

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/cff.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/cff.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 from rdflib import BNode, Graph, Literal, URIRef
 import rdflib.term
 
 from swh.indexer.codemeta import CROSSWALK_TABLE
 from swh.indexer.namespaces import RDF, SCHEMA
 
-from .base import YamlMapping
+from .base import SingleFileIntrinsicMapping, YamlMapping
 from .utils import add_map
 
 DOI = URIRef("https://doi.org/")
 SPDX = URIRef("https://spdx.org/licenses/")
 
 
-class CffMapping(YamlMapping):
+class CffMapping(YamlMapping, SingleFileIntrinsicMapping):
     """Dedicated class for Citation (CITATION.cff) mapping and translation"""
 
     name = "cff"
     filename = b"CITATION.cff"
     mapping = CROSSWALK_TABLE["Citation File Format Core (CFF-Core) 1.0.2"]
     string_fields = ["keywords", "license", "abstract", "version", "doi"]
     date_fields = ["date-released"]
```

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/codemeta.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/composer.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/composer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/dart.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/dart.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 
 from rdflib import RDF, BNode, Graph, Literal, URIRef
 
 from swh.indexer.codemeta import _DATA_DIR, read_crosstable
 from swh.indexer.namespaces import SCHEMA
 
-from .base import YamlMapping
+from .base import SingleFileIntrinsicMapping, YamlMapping
 from .utils import add_map
 
 SPDX = URIRef("https://spdx.org/licenses/")
 
 PUB_TABLE_PATH = os.path.join(_DATA_DIR, "pubspec.csv")
 
 with open(PUB_TABLE_PATH) as fd:
@@ -25,15 +25,15 @@
 def name_to_person(name):
     return {
         "@type": SCHEMA.Person,
         SCHEMA.name: name,
     }
 
 
-class PubspecMapping(YamlMapping):
+class PubspecMapping(YamlMapping, SingleFileIntrinsicMapping):
 
     name = "pubspec"
     filename = b"pubspec.yaml"
     mapping = PUB_TABLE["Pubspec"]
     string_fields = [
         "repository",
         "keywords",
```

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/gitea.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/gitea.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/github.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/github.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/maven.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/maven.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/npm.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/npm.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/nuget.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/nuget.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Copyright (C) 2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os.path
 import re
-from typing import Any, Dict, List
+from typing import Any, Dict
 
 from rdflib import RDF, BNode, Graph, Literal, URIRef
 
 from swh.indexer.codemeta import _DATA_DIR, read_crosstable
 from swh.indexer.namespaces import SCHEMA
-from swh.indexer.storage.interface import Sha1
 
-from .base import BaseIntrinsicMapping, DirectoryLsEntry, XmlMapping
+from .base import SingleFileIntrinsicMapping, XmlMapping
 from .utils import add_list, add_url_if_valid
 
 NUGET_TABLE_PATH = os.path.join(_DATA_DIR, "nuget.csv")
 
 with open(NUGET_TABLE_PATH) as fd:
     (CODEMETA_TERMS, NUGET_TABLE) = read_crosstable(fd)
 
 SPDX = URIRef("https://spdx.org/licenses/")
 
 
-class NuGetMapping(XmlMapping, BaseIntrinsicMapping):
+class NuGetMapping(XmlMapping, SingleFileIntrinsicMapping):
     """
     dedicated class for NuGet (.nuspec) mapping and translation
     """
 
     name = "nuget"
+    filename = re.compile(rb".*\.nuspec")
     mapping = NUGET_TABLE["NuGet"]
     mapping["copyright"] = URIRef("http://schema.org/copyrightNotice")
     mapping["language"] = URIRef("http://schema.org/inLanguage")
     string_fields = [
         "description",
         "version",
         "name",
@@ -41,21 +41,14 @@
         "license",
         "summary",
         "copyright",
         "language",
     ]
     uri_fields = ["projectUrl", "licenseUrl"]
 
-    @classmethod
-    def detect_metadata_files(cls, file_entries: List[DirectoryLsEntry]) -> List[Sha1]:
-        for entry in file_entries:
-            if entry["name"].endswith(b".nuspec"):
-                return [entry["sha1"]]
-        return []
-
     def _translate_dict(self, d: Dict[str, Any]) -> Dict[str, Any]:
         return super()._translate_dict(d.get("package", {}).get("metadata", {}))
 
     def translate_repository(self, graph, root, v):
         if isinstance(v, dict) and isinstance(v["@url"], str):
             codemeta_key = URIRef(self.mapping["repository.url"])
             add_url_if_valid(graph, root, codemeta_key, v["@url"])
```

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/python.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/python.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/ruby.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/ruby.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,54 +2,45 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import ast
 import itertools
 import re
-from typing import List
 
 from rdflib import RDF, BNode, Graph, Literal, URIRef
 
 from swh.indexer.codemeta import CROSSWALK_TABLE
-from swh.indexer.metadata_dictionary.base import DirectoryLsEntry
 from swh.indexer.namespaces import SCHEMA
-from swh.indexer.storage.interface import Sha1
 
-from .base import BaseIntrinsicMapping, DictMapping
+from .base import DictMapping, SingleFileIntrinsicMapping
 from .utils import add_map
 
 SPDX = URIRef("https://spdx.org/licenses/")
 
 
 def name_to_person(graph: Graph, name):
     if not isinstance(name, str):
         return None
     author = BNode()
     graph.add((author, RDF.type, SCHEMA.Person))
     graph.add((author, SCHEMA.name, Literal(name)))
     return author
 
 
-class GemspecMapping(BaseIntrinsicMapping, DictMapping):
+class GemspecMapping(DictMapping, SingleFileIntrinsicMapping):
     name = "gemspec"
+    filename = re.compile(rb".*\.gemspec")
     mapping = CROSSWALK_TABLE["Ruby Gem"]
     string_fields = ["name", "version", "description", "summary", "email"]
     uri_fields = ["homepage"]
 
     _re_spec_new = re.compile(r".*Gem::Specification.new +(do|\{) +\|.*\|.*")
     _re_spec_entry = re.compile(r"\s*\w+\.(?P<key>\w+)\s*=\s*(?P<expr>.*)")
 
-    @classmethod
-    def detect_metadata_files(cls, file_entries: List[DirectoryLsEntry]) -> List[Sha1]:
-        for entry in file_entries:
-            if entry["name"].endswith(b".gemspec"):
-                return [entry["sha1"]]
-        return []
-
     def translate(self, raw_content):
         try:
             raw_content = raw_content.decode()
         except UnicodeDecodeError:
             self.log.warning("Error unidecoding from %s", self.log_suffix)
             return
```

### Comparing `swh.indexer-2.9.3/swh/indexer/metadata_dictionary/utils.py` & `swh.indexer-2.9.4/swh/indexer/metadata_dictionary/utils.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/mimetype.py` & `swh.indexer-2.9.4/swh/indexer/mimetype.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/namespaces.py` & `swh.indexer-2.9.4/swh/indexer/namespaces.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/origin_head.py` & `swh.indexer-2.9.4/swh/indexer/origin_head.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/rehash.py` & `swh.indexer-2.9.4/swh/indexer/rehash.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/30-schema.sql` & `swh.indexer-2.9.4/swh/indexer/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/50-func.sql` & `swh.indexer-2.9.4/swh/indexer/sql/50-func.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/60-indexes.sql` & `swh.indexer-2.9.4/swh/indexer/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/115.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/115.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/116.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/116.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/117.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/117.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/119.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/119.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/120.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/120.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/123.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/123.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/125.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/125.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/126.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/126.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/127.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/127.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/129.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/129.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/130.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/130.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/131.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/131.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/132.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/132.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/133.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/133.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/134.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/134.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/135.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/135.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/136.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/136.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/sql/upgrades/137.sql` & `swh.indexer-2.9.4/swh/indexer/sql/upgrades/137.sql`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/__init__.py` & `swh.indexer-2.9.4/swh/indexer/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/api/client.py` & `swh.indexer-2.9.4/swh/indexer/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/api/serializers.py` & `swh.indexer-2.9.4/swh/indexer/storage/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/api/server.py` & `swh.indexer-2.9.4/swh/indexer/storage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/converters.py` & `swh.indexer-2.9.4/swh/indexer/storage/converters.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/db.py` & `swh.indexer-2.9.4/swh/indexer/storage/db.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/exc.py` & `swh.indexer-2.9.4/swh/indexer/storage/exc.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/in_memory.py` & `swh.indexer-2.9.4/swh/indexer/storage/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/interface.py` & `swh.indexer-2.9.4/swh/indexer/storage/interface.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/metrics.py` & `swh.indexer-2.9.4/swh/indexer/storage/metrics.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/model.py` & `swh.indexer-2.9.4/swh/indexer/storage/model.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/storage/writer.py` & `swh.indexer-2.9.4/swh/indexer/storage/writer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tasks.py` & `swh.indexer-2.9.4/swh/indexer/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/conftest.py` & `swh.indexer-2.9.4/swh/indexer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_cff.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_cff.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_codemeta.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_composer.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_composer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_dart.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_dart.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pytest
 
 from swh.indexer.metadata_dictionary import MAPPINGS
 
 
 def test_compute_metadata_pubspec():
-    raw_content = """
+    raw_content = b"""
 ---
 name: newtify
 description: >-
   Have you been turned into a newt?  Would you like to be?
   This package can help. It has all of the
   newt-transmogrification functionality you have been looking
   for.
@@ -33,17 +33,15 @@
 
 dependencies:
   efts: ^2.0.4
   transmogrify: ^0.4.0
 
 dev_dependencies:
   test: '>=1.15.0 <2.0.0'
-    """.encode(
-        "utf-8"
-    )
+    """
 
     result = MAPPINGS["PubMapping"]().translate(raw_content)
 
     assert set(result.pop("keywords")) == {
         "polyfill",
         "shim",
         "compatibility",
@@ -62,19 +60,17 @@
         "license": "https://spdx.org/licenses/MIT",
     }
 
     assert result == expected
 
 
 def test_normalize_author_pubspec():
-    raw_content = """
+    raw_content = b"""
     author: Atlee Pine <atlee@example.org>
-    """.encode(
-        "utf-8"
-    )
+    """
 
     result = MAPPINGS["PubMapping"]().translate(raw_content)
 
     expected = {
         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
         "type": "SoftwareSourceCode",
         "author": [
@@ -82,21 +78,19 @@
         ],
     }
 
     assert result == expected
 
 
 def test_normalize_authors_pubspec():
-    raw_content = """
+    raw_content = b"""
     authors:
       - Vicky Merzown <vmz@example.org>
       - Ron Bilius Weasley
-    """.encode(
-        "utf-8"
-    )
+    """
 
     result = MAPPINGS["PubMapping"]().translate(raw_content)
 
     expected = {
         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
         "type": "SoftwareSourceCode",
         "author": [
@@ -109,22 +103,20 @@
     }
 
     assert result == expected
 
 
 @pytest.mark.xfail(reason="https://github.com/w3c/json-ld-api/issues/547")
 def test_normalize_author_authors_pubspec():
-    raw_content = """
+    raw_content = b"""
     authors:
       - Vicky Merzown <vmz@example.org>
       - Ron Bilius Weasley
     author: Hermione Granger
-    """.encode(
-        "utf-8"
-    )
+    """
 
     result = MAPPINGS["PubMapping"]().translate(raw_content)
 
     expected = {
         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
         "type": "SoftwareSourceCode",
         "author": [
@@ -140,21 +132,30 @@
         ],
     }
 
     assert result == expected
 
 
 def test_normalize_empty_authors():
-    raw_content = """
+    raw_content = b"""
     authors:
-    """.encode(
-        "utf-8"
-    )
+    """
 
     result = MAPPINGS["PubMapping"]().translate(raw_content)
 
     expected = {
         "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
         "type": "SoftwareSourceCode",
     }
 
     assert result == expected
+
+
+def test_invalid_yaml():
+    raw_content = b"""
+    name: smartech_push
+    license: { :type => "Commercial", :file => "LICENSE" }
+    """
+
+    result = MAPPINGS["PubMapping"]().translate(raw_content)
+
+    assert result is None
```

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_gitea.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_gitea.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_github.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_github.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_maven.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_maven.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_npm.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_npm.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_nuget.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_nuget.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_python.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_python.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/metadata_dictionary/test_ruby.py` & `swh.indexer-2.9.4/swh/indexer/tests/metadata_dictionary/test_ruby.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/conftest.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/generate_data_test.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/generate_data_test.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_api_client.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_converters.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_in_memory.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_init.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_metrics.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_metrics.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_model.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_model.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_server.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/storage/test_storage.py` & `swh.indexer-2.9.4/swh/indexer/tests/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/tasks.py` & `swh.indexer-2.9.4/swh/indexer/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_cli.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_codemeta.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_codemeta.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_fossology_license.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_fossology_license.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_indexer.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_journal_client.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_metadata.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_mimetype.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_mimetype.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_origin_head.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_origin_head.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/test_origin_metadata.py` & `swh.indexer-2.9.4/swh/indexer/tests/test_origin_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/utils.py` & `swh.indexer-2.9.4/swh/indexer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh/indexer/tests/zz_celery/test_tasks.py` & `swh.indexer-2.9.4/swh/indexer/tests/zz_celery/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.indexer-2.9.3/swh.indexer.egg-info/PKG-INFO` & `swh.indexer-2.9.4/swh.indexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.indexer
-Version: 2.9.3
+Version: 2.9.4
 Summary: Software Heritage Content Indexer
 Home-page: https://forge.softwareheritage.org/diffusion/78/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-indexer
```

### Comparing `swh.indexer-2.9.3/swh.indexer.egg-info/SOURCES.txt` & `swh.indexer-2.9.4/swh.indexer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 docs/Makefile.local
 docs/README.md
 docs/cli.rst
 docs/conf.py
 docs/dev-info.rst
 docs/index.rst
 docs/metadata-workflow.rst
+docs/swhpkg.rst
 docs/_static/.placeholder
 docs/_templates/.placeholder
 docs/images/.gitignore
 docs/images/Makefile
-docs/images/tasks-metadata-indexers.uml
+docs/images/tasks-extrinsic-metadata-indexers.uml
+docs/images/tasks-intrinsic-metadata-indexers.uml
 sql/bin/db-upgrade
 sql/bin/dot_add_content
 sql/doc/json
 sql/doc/json/.gitignore
 sql/doc/json/Makefile
 sql/doc/json/indexer_configuration.tool_configuration.schema.json
 sql/doc/json/revision_metadata.translated_metadata.json
```

### Comparing `swh.indexer-2.9.3/tox.ini` & `swh.indexer-2.9.4/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [tox]
+requires =
+  tox>4
 envlist=black,flake8,mypy,py3
 
 [testenv]
 extras =
   testing
 deps =
   pytest-cov
@@ -33,48 +35,44 @@
 commands =
   {envpython} -m flake8
 
 [testenv:mypy]
 extras =
   testing
 deps =
-  mypy==0.942
+  mypy==1.0
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
-  # fetch and install swh-docs in develop mode
-  -e git+https://forge.softwareheritage.org/source/swh-docs#egg=swh.docs
-
+  -e git+https://gitlab.softwareheritage.org/swh/devel/swh-docs.git\#egg=swh.docs
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
-
 # build documentation only inside swh-environment using local state
 # of swh-docs package
 [testenv:sphinx-dev]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # install swh-docs in develop mode
   -e ../swh-docs
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

