# Comparing `tmp/sqlfluff-2.1.1.tar.gz` & `tmp/sqlfluff-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-a8ni5akz/sqlfluff-2.1.1.tar", last modified: Thu May 25 16:29:29 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-edjas6jf/sqlfluff-2.1.2.tar", last modified: Mon Jul  3 08:39:57 2023, max compression
```

## Comparing `sqlfluff-2.1.1.tar` & `sqlfluff-2.1.2.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)   387901 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131078 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    23153 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68489 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    95470 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    80767 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   165834 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   200331 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   102326 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   172937 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)   391296 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45672 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25234 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134007 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68489 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94430 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81016 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165314 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36674 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202066 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101197 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173365 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:39:57.000000 sqlfluff-2.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-03 08:39:43.000000 sqlfluff-2.1.2/test/test_testing.py
```

### Comparing `sqlfluff-2.1.1/CHANGELOG.md` & `sqlfluff-2.1.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,54 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.1.2] - 2023-07-03
+
+## Highlights
+
+This release resolves compatibility issues with a set of `dbt-core` versions.
+- `dbt-core` 1.5.2 onwards is now properly supported.
+- support for `dbt-core` 1.1 to 1.4 has now been re-enabled after
+  support had to be abandoned a few releases ago.
+
+NOTE: We cannot guarantee that SQLFluff will always continue to remain
+compatible with all dbt versions, particularly as the folks at dbt-labs
+have often backported breaking changes to their internal APIs to previous
+versions of `dbt-core`. This release does at least bring more extensive
+internal testing to catch when this does occur to allow our community
+to react.
+
+This release fixes also resolves a potential security issue for when
+using external libraries (and the `library_path` config setting),
+and also contains various dialect improvements.
+
+## What’s Changed
+
+* docs(templater): Add documentation for `SQLFLUFF_JINJA_FILTERS` [#4932](https://github.com/sqlfluff/sqlfluff/pull/4932) [@dmohns](https://github.com/dmohns)
+* Re-enable dbt 1.1 & 1.2 [#4944](https://github.com/sqlfluff/sqlfluff/pull/4944) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Re-enable dbt 1.4 & 1.3 [#4941](https://github.com/sqlfluff/sqlfluff/pull/4941) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix compatibility with dbt 1.5.2+ [#4939](https://github.com/sqlfluff/sqlfluff/pull/4939) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Security option for library path [#4925](https://github.com/sqlfluff/sqlfluff/pull/4925) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Remove extra code escapes from release notes docs [#4921](https://github.com/sqlfluff/sqlfluff/pull/4921) [@tunetheweb](https://github.com/tunetheweb)
+* Postgres frame_clause quoted interval [#4915](https://github.com/sqlfluff/sqlfluff/pull/4915) [@greg-finley](https://github.com/greg-finley)
+* Snowflake: CREATE TAG [#4914](https://github.com/sqlfluff/sqlfluff/pull/4914) [@greg-finley](https://github.com/greg-finley)
+* TSQL: support for `DROP EXTERNAL TABLE` [#4919](https://github.com/sqlfluff/sqlfluff/pull/4919) [@keen85](https://github.com/keen85)
+* fix(dialect-clickhouse): Support create database [#4620](https://github.com/sqlfluff/sqlfluff/pull/4620) [@germainlefebvre4](https://github.com/germainlefebvre4)
+* Snowflake: Actualize the CreateProcedureStatementSegment and CreateFunctionStatementSegment [#4908](https://github.com/sqlfluff/sqlfluff/pull/4908) [@moreaupascal56](https://github.com/moreaupascal56)
+* Oracle: Add support for `$` and `#`  in identifier [#4903](https://github.com/sqlfluff/sqlfluff/pull/4903) [@ulixius9](https://github.com/ulixius9)
+* docs(templater): Refactor templater configuration docs [#4835](https://github.com/sqlfluff/sqlfluff/pull/4835) [@dmohns](https://github.com/dmohns)
+* Handle brackets in from clause with joins [#4890](https://github.com/sqlfluff/sqlfluff/pull/4890) [@ulixius9](https://github.com/ulixius9)
+* Postgres: Add support for dollar literal & mark collation as non-reserved [#4883](https://github.com/sqlfluff/sqlfluff/pull/4883) [@ulixius9](https://github.com/ulixius9)
+* MySQL: ON UPDATE NOW [#4898](https://github.com/sqlfluff/sqlfluff/pull/4898) [@greg-finley](https://github.com/greg-finley)
+* Support ROLLUP/CUBE in AM06 [#4892](https://github.com/sqlfluff/sqlfluff/pull/4892) [@tunetheweb](https://github.com/tunetheweb)
+
 ## [2.1.1] - 2023-05-25
 
 ## Highlights
 
 This releases fixes a compatability issue with the latest version of dbt. It also ships various dialect improvements.
 
 ## What’s Changed
```

### Comparing `sqlfluff-2.1.1/LICENSE.md` & `sqlfluff-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/PKG-INFO` & `sqlfluff-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.1
+Version: 2.1.2
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.1/README.md` & `sqlfluff-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/setup.cfg` & `sqlfluff-2.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.1.1
+version = 2.1.2
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -110,13 +110,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.1.1
+stable_version = 2.1.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/api/simple.py` & `sqlfluff-2.1.2/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.1.2/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.1.2/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
             frame = inspect.currentframe()
             try:
                 opt = frame.f_back.f_locals.get("opt")  # type: ignore
             finally:
                 del frame
 
-            if opt in deprecated:  # type: ignore
+            if opt in deprecated:
                 msg = (
                     f"DeprecationWarning: The option {opt!r} is deprecated, "
                     f"use {preferred!r}."
                 )
                 echo(style(msg, fg="red"), err=True)
 
             return orig_process(value, state)
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/cli/commands.py` & `sqlfluff-2.1.2/src/sqlfluff/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,24 @@
     )(f)
     f = click.option(
         "--disable-noqa",
         is_flag=True,
         default=None,
         help="Set this flag to ignore inline noqa comments.",
     )(f)
+    f = click.option(
+        "--library-path",
+        default=None,
+        help=(
+            "Override the `library_path` value from the [sqlfluff:templater:jinja]"
+            " configuration value. Set this to 'none' to disable entirely."
+            " This overrides any values set by users in configuration files or"
+            " inline directives."
+        ),
+    )(f)
     return f
 
 
 def lint_options(f: Callable) -> Callable:
     """Add lint operation options to commands via a decorator.
 
     These are cli commands that do linting, i.e. `lint` and `fix`.
@@ -378,16 +388,23 @@
                     color=Color.red,
                 )
             )
             sys.exit(EXIT_ERROR)
     from_root_kwargs = {}
     if "require_dialect" in kwargs:
         from_root_kwargs["require_dialect"] = kwargs.pop("require_dialect")
+    library_path = kwargs.pop("library_path", None)
     # Instantiate a config object (filtering out the nulls)
     overrides = {k: kwargs[k] for k in kwargs if kwargs[k] is not None}
+    if library_path is not None:
+        # Check for a null value
+        if library_path.lower() == "none":
+            library_path = None  # Set an explicit None value.
+        # Set the global override
+        overrides["library_path"] = library_path
     try:
         return FluffConfig.from_root(
             extra_config_path=extra_config_path,
             ignore_local_config=ignore_local_config,
             overrides=overrides,
             **from_root_kwargs,
         )
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.1.2/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.1.2/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.1.2/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/config.py` & `sqlfluff-2.1.2/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.1.2/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.1.2/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.1.2/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/enums.py` & `sqlfluff-2.1.2/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/errors.py` & `sqlfluff-2.1.2/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.1.2/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.1.2/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.1.2/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.1.2/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.1.2/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.1.2/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.1.2/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.1.2/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.1.2/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.1.2/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.1.2/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.1.2/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.1.2/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.1.2/src/sqlfluff/core/templaters/jinja.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,16 @@
         for value in loaded_context.values():
             macro_ctx.update(
                 self._extract_macros_from_template(value, env=env, ctx=ctx)
             )
         return macro_ctx
 
     def _extract_libraries_from_config(self, config):
-        library_path = config.get_section(
+        # If a more global library_path is set, let that take precedence.
+        library_path = config.get("library_path") or config.get_section(
             (self.templater_selector, self.name, "library_path")
         )
         if not library_path:
             return {}
 
         libraries = JinjaTemplater.Libraries()
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.1.2/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.1.2/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.1.2/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/core/timing.py` & `sqlfluff-2.1.2/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1443,15 +1443,19 @@
     """
 
     type = "frame_clause"
 
     _frame_extent = OneOf(
         Sequence("CURRENT", "ROW"),
         Sequence(
-            OneOf(Ref("NumericLiteralSegment"), "UNBOUNDED"),
+            OneOf(
+                Ref("NumericLiteralSegment"),
+                Sequence("INTERVAL", Ref("QuotedLiteralSegment")),
+                "UNBOUNDED",
+            ),
             OneOf("PRECEDING", "FOLLOWING"),
         ),
     )
 
     match_grammar: Matchable = Sequence(
         Ref("FrameClauseUnitGrammar"),
         OneOf(_frame_extent, Sequence("BETWEEN", _frame_extent, "AND", _frame_extent)),
@@ -1541,31 +1545,35 @@
         )
 
 
 class FromExpressionSegment(BaseSegment):
     """A from expression segment."""
 
     type = "from_expression"
-    match_grammar: Matchable = Sequence(
-        Indent,
-        OneOf(
-            # check first for MLTableExpression, because of possible FunctionSegment in
-            # MainTableExpression
-            Ref("MLTableExpressionSegment"),
-            Ref("FromExpressionElementSegment"),
-        ),
-        Dedent,
-        Conditional(Indent, indented_joins=True),
-        AnyNumberOf(
-            Sequence(
-                OneOf(Ref("JoinClauseSegment"), Ref("JoinLikeClauseGrammar")),
+    match_grammar: Matchable = OptionallyBracketed(
+        Sequence(
+            Indent,
+            OneOf(
+                # check first for MLTableExpression,
+                # because of possible FunctionSegment in
+                # MainTableExpression
+                Ref("MLTableExpressionSegment"),
+                Ref("FromExpressionElementSegment"),
+                Bracketed(Ref("FromExpressionSegment")),
             ),
-            optional=True,
-        ),
-        Conditional(Dedent, indented_joins=True),
+            Dedent,
+            Conditional(Indent, indented_joins=True),
+            AnyNumberOf(
+                Sequence(
+                    OneOf(Ref("JoinClauseSegment"), Ref("JoinLikeClauseGrammar")),
+                ),
+                optional=True,
+            ),
+            Conditional(Dedent, indented_joins=True),
+        )
     )
 
 
 class TableExpressionSegment(BaseSegment):
     """The main table expression e.g. within a FROM clause."""
 
     type = "table_expression"
@@ -2296,37 +2304,127 @@
             ),
             terminator=OneOf(Ref.keyword("LIMIT"), Ref("FrameClauseUnitGrammar")),
         ),
         Dedent,
     )
 
 
-class GroupByClauseSegment(BaseSegment):
-    """A `GROUP BY` clause like in `SELECT`."""
+class RollupFunctionNameSegment(BaseSegment):
+    """ROLLUP function name segment.
 
-    type = "groupby_clause"
+    Need to be able to specify this as type `function_name_identifier`
+    within a `function_name` so that linting rules identify it properly.
+    """
+
+    type = "function_name"
+    match_grammar: Matchable = StringParser(
+        "ROLLUP",
+        CodeSegment,
+        type="function_name_identifier",
+    )
+
+
+class CubeFunctionNameSegment(BaseSegment):
+    """ROLLUP function name segment.
+
+    Need to be able to specify this as type `function_name_identifier`
+    within a `function_name` so that linting rules identify it properly.
+    """
+
+    type = "function_name"
+    match_grammar: Matchable = StringParser(
+        "CUBE",
+        CodeSegment,
+        type="function_name_identifier",
+    )
+
+
+class GroupingSetsClauseSegment(BaseSegment):
+    """`GROUPING SETS` clause within the `GROUP BY` clause."""
+
+    type = "grouping_sets_clause"
+
+    match_grammar = Sequence(
+        "GROUPING",
+        "SETS",
+        Bracketed(
+            Delimited(
+                Ref("CubeRollupClauseSegment"),
+                Ref("GroupingExpressionList"),
+            )
+        ),
+    )
+
+
+class GroupingExpressionList(BaseSegment):
+    """A `GROUP BY` clause expression list like in `ROLLUP`."""
+
+    type = "grouping_expression_list"
 
     match_grammar: Matchable = Sequence(
-        "GROUP",
-        "BY",
         Indent,
         Delimited(
             OneOf(
                 Ref("ColumnReferenceSegment"),
-                # Can `GROUP BY 1`
+                # Can `GROUP BY ROLLUP(1)`
                 Ref("NumericLiteralSegment"),
-                # Can `GROUP BY coalesce(col, 1)`
+                # Can `GROUP BY ROLLUP(coalesce(col, 1))`
                 Ref("ExpressionSegment"),
+                Bracketed(),  # Allows empty parentheses
             ),
             terminator=Ref("GroupByClauseTerminatorGrammar"),
         ),
         Dedent,
     )
 
 
+class CubeRollupClauseSegment(BaseSegment):
+    """`CUBE` / `ROLLUP` clause within the `GROUP BY` clause."""
+
+    type = "cube_rollup_clause"
+    match_grammar = Sequence(
+        OneOf(Ref("CubeFunctionNameSegment"), Ref("RollupFunctionNameSegment")),
+        Bracketed(
+            Ref("GroupingExpressionList"),
+        ),
+    )
+
+
+class GroupByClauseSegment(BaseSegment):
+    """A `GROUP BY` clause like in `SELECT`."""
+
+    type = "groupby_clause"
+
+    match_grammar: Matchable = Sequence(
+        "GROUP",
+        "BY",
+        OneOf(
+            Ref("CubeRollupClauseSegment"),
+            # We could replace this next bit with a GroupingExpressionList
+            # reference (renaming that to a more generic name), to avoid
+            # repeating this bit of code, but I would rather keep it flat
+            # to avoid changing regular `GROUP BY` clauses.
+            Sequence(
+                Indent,
+                Delimited(
+                    OneOf(
+                        Ref("ColumnReferenceSegment"),
+                        # Can `GROUP BY 1`
+                        Ref("NumericLiteralSegment"),
+                        # Can `GROUP BY coalesce(col, 1)`
+                        Ref("ExpressionSegment"),
+                    ),
+                    terminator=Ref("GroupByClauseTerminatorGrammar"),
+                ),
+                Dedent,
+            ),
+        ),
+    )
+
+
 class HavingClauseSegment(BaseSegment):
     """A `HAVING` clause like in `SELECT`."""
 
     type = "having_clause"
     match_grammar: Matchable = Sequence(
         "HAVING",
         ImplicitIndent,
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_athena.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,42 +675,14 @@
                 Ref("SetOperatorSegment"),
             ),
         ),
         Dedent,
     )
 
 
-class CubeRollupClauseSegment(BaseSegment):
-    """`[CUBE | ROLLUP]` clause within the `GROUP BY` clause."""
-
-    type = "cube_rollup_clause"
-
-    match_grammar = Sequence(
-        OneOf("CUBE", "ROLLUP"),
-        Bracketed(Delimited(Ref("ColumnReferenceSegment"))),
-    )
-
-
-class GroupingSetsClauseSegment(BaseSegment):
-    """`GROUPING SETS` clause within the `GROUP BY` clause."""
-
-    type = "grouping_sets_clause"
-
-    match_grammar = Sequence(
-        "GROUPING",
-        "SETS",
-        Bracketed(
-            Delimited(
-                Ref("ColumnReferenceSegment"),
-                Bracketed(Delimited(Ref("ColumnReferenceSegment"), optional=True)),
-            ),
-        ),
-    )
-
-
 class ShowStatementSegment(BaseSegment):
     """A `show` execute statement.
 
     Full Apache Hive `SHOW` reference:
     https://cwiki.apache.org/confluence/display/Hive/LanguageManual+DDL#LanguageManualDDL-Show
 
     Athena supported subset:
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,21 +293,21 @@
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/arrays#flattening_arrays
         Sequence("WITH", "OFFSET", Ref("AliasExpressionSegment"), optional=True),
         Ref("SamplingExpressionSegment", optional=True),
         Ref("PostTableExpressionGrammar", optional=True),
     )
 
 
-class EngineFunctionSegment(BaseSegment):
+class TableEngineFunctionSegment(BaseSegment):
     """A ClickHouse `ENGINE` clause function.
 
     With this segment we attempt to match all possible engines.
     """
 
-    type = "engine_function"
+    type = "table_engine_function"
     match_grammar: Matchable = Sequence(
         Sequence(
             Ref(
                 "FunctionNameSegment",
                 exclude=OneOf(
                     Ref("DatePartFunctionNameSegment"),
                     Ref("ValuesClauseSegment"),
@@ -326,32 +326,117 @@
         ),
     )
 
 
 class OnClusterClauseSegment(BaseSegment):
     """A `ON CLUSTER` clause."""
 
-    type = "on_cluster"
+    type = "on_cluster_clause"
     match_grammar = Sequence(
         "ON",
         "CLUSTER",
         Ref("SingleIdentifierGrammar"),
     )
 
 
-class EngineSegment(BaseSegment):
+class TableEngineSegment(BaseSegment):
     """An `ENGINE` used in `CREATE TABLE`."""
 
     type = "engine"
+    match_grammar = Sequence(
+        "ENGINE",
+        Ref("EqualsSegment"),
+        Sequence(
+            Ref("TableEngineFunctionSegment"),
+            AnySetOf(
+                Sequence(
+                    "ORDER",
+                    "BY",
+                    OneOf(
+                        Ref("BracketedColumnReferenceListGrammar"),
+                        Ref("ColumnReferenceSegment"),
+                    ),
+                ),
+                Sequence(
+                    "PARTITION",
+                    "BY",
+                    Ref("ExpressionSegment"),
+                ),
+                Sequence(
+                    "PRIMARY",
+                    "KEY",
+                    Ref("ExpressionSegment"),
+                ),
+                Sequence(
+                    "SAMPLE",
+                    "BY",
+                    Ref("ExpressionSegment"),
+                ),
+                Sequence(
+                    "SETTINGS",
+                    Delimited(
+                        Sequence(
+                            Ref("NakedIdentifierSegment"),
+                            Ref("EqualsSegment"),
+                            OneOf(
+                                Ref("NumericLiteralSegment"),
+                                Ref("QuotedLiteralSegment"),
+                            ),
+                            optional=True,
+                        ),
+                    ),
+                ),
+            ),
+        ),
+    )
+
+
+class DatabaseEngineFunctionSegment(BaseSegment):
+    """A ClickHouse `ENGINE` clause function.
+
+    With this segment we attempt to match all possible engines.
+    """
+
+    type = "engine_function"
+    match_grammar: Matchable = Sequence(
+        Sequence(
+            OneOf(
+                "ATOMIC",
+                "MYSQL",
+                "MATERIALIZEDMYSQL",
+                "LAZY",
+                "POSTGRESQL",
+                "MATERIALIZEDPOSTGRESQL",
+                "REPLICATED",
+                "SQLITE",
+            ),
+            Bracketed(
+                Ref(
+                    "FunctionContentsGrammar",
+                    # The brackets might be empty for some functions...
+                    optional=True,
+                    ephemeral_name="FunctionContentsGrammar",
+                ),
+                # Engine functions may omit brackets.
+                optional=True,
+            ),
+        ),
+    )
+
+
+class DatabaseEngineSegment(BaseSegment):
+    """An `ENGINE` used in `CREATE TABLE`."""
+
+    type = "database_engine"
 
     match_grammar = Sequence(
         "ENGINE",
         Ref("EqualsSegment"),
         Sequence(
-            Ref("EngineFunctionSegment"),
+            Ref("DatabaseEngineFunctionSegment"),
             AnySetOf(
                 Sequence(
                     "ORDER",
                     "BY",
                     OneOf(
                         Ref("BracketedColumnReferenceListGrammar"),
                         Ref("ColumnReferenceSegment"),
@@ -496,14 +581,71 @@
                 ),
                 Ref("ColumnTTLSegment"),
             ),
         )
     )
 
 
+class CreateDatabaseStatementSegment(ansi.CreateDatabaseStatementSegment):
+    """A `CREATE DATABASE` statement.
+
+    As specified in
+    https://clickhouse.com/docs/en/sql-reference/statements/create/database
+    """
+
+    type = "create_database_statement"
+
+    match_grammar = Sequence(
+        "CREATE",
+        "DATABASE",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("DatabaseReferenceSegment"),
+        AnySetOf(
+            Ref("OnClusterClauseSegment", optional=True),
+            Ref("DatabaseEngineSegment", optional=True),
+            Sequence(
+                "COMMENT",
+                Ref("SingleIdentifierGrammar"),
+                optional=True,
+            ),
+            Sequence(
+                "SETTINGS",
+                Delimited(
+                    Sequence(
+                        Ref("NakedIdentifierSegment"),
+                        Ref("EqualsSegment"),
+                        OneOf(
+                            Ref("NakedIdentifierSegment"),
+                            Ref("NumericLiteralSegment"),
+                            Ref("QuotedLiteralSegment"),
+                            Ref("BooleanLiteralGrammar"),
+                        ),
+                        optional=True,
+                    ),
+                ),
+                optional=True,
+            ),
+        ),
+        AnyNumberOf(
+            "TABLE",
+            "OVERRIDE",
+            Ref("TableReferenceSegment"),
+            Bracketed(
+                Delimited(
+                    Ref("TableConstraintSegment"),
+                    Ref("ColumnDefinitionSegment"),
+                    Ref("ColumnConstraintSegment"),
+                ),
+                optional=True,
+            ),
+            optional=True,
+        ),
+    )
+
+
 class CreateTableStatementSegment(ansi.CreateTableStatementSegment):
     """A `CREATE TABLE` statement.
 
     As specified in
     https://clickhouse.com/docs/en/sql-reference/statements/create/table/
     """
 
@@ -530,38 +672,41 @@
                             Ref("ColumnDefinitionSegment"),
                             Ref("ColumnConstraintSegment"),
                         ),
                     ),
                     # Column definition may be missing if using AS SELECT
                     optional=True,
                 ),
-                Ref("EngineSegment"),
+                Ref("TableEngineSegment"),
                 # CREATE TABLE (...) AS SELECT:
                 Sequence(
                     "AS",
                     Ref("SelectableGrammar"),
                     optional=True,
                 ),
             ),
             # CREATE TABLE AS other_table:
             Sequence(
                 "AS",
                 Ref("TableReferenceSegment"),
-                Ref("EngineSegment", optional=True),
+                Ref("TableEngineSegment", optional=True),
             ),
             # CREATE TABLE AS table_function():
             Sequence(
                 "AS",
                 Ref("FunctionSegment"),
             ),
         ),
         AnySetOf(
             Sequence(
                 "COMMENT",
-                Ref("SingleQuotedIdentifierSegment"),
+                OneOf(
+                    Ref("SingleIdentifierGrammar"),
+                    Ref("QuotedIdentifierSegment"),
+                ),
             ),
             Ref("TableTTLSegment"),
             optional=True,
         ),
         Ref("TableEndClauseSegment", optional=True),
     )
 
@@ -581,18 +726,18 @@
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         Ref("OnClusterClauseSegment", optional=True),
         OneOf(
             Sequence(
                 "TO",
                 Ref("TableReferenceSegment"),
-                Ref("EngineSegment", optional=True),
+                Ref("TableEngineSegment", optional=True),
             ),
             Sequence(
-                Ref("EngineSegment", optional=True),
+                Ref("TableEngineSegment", optional=True),
                 Sequence("POPULATE", optional=True),
             ),
         ),
         "AS",
         Ref("SelectableGrammar"),
         Ref("TableEndClauseSegment", optional=True),
     )
@@ -1069,15 +1214,14 @@
 
 class StatementSegment(ansi.StatementSegment):
     """Overriding StatementSegment to allow for additional segment parsing."""
 
     match_grammar = ansi.StatementSegment.match_grammar
     parse_grammar = ansi.StatementSegment.parse_grammar.copy(
         insert=[
-            Ref("CreateTableStatementSegment"),
             Ref("CreateMaterializedViewStatementSegment"),
             Ref("DropDictionaryStatementSegment"),
             Ref("DropQuotaStatementSegment"),
             Ref("DropSettingProfileStatementSegment"),
             Ref("SystemStatementSegment"),
         ]
     )
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "ANY",
     "ARRAY",
     "AS",
     "ASCENDING",
     "ASOF",
     "AST",
     "ASYNC",
+    "ATOMIC",
     "ATTACH",
     "BETWEEN",
     "BOTH",
     "BY",
     "CHECK",
     "CLEAR",
     "CLUSTER",
@@ -89,44 +90,50 @@
     "INTO",
     "IS",
     "IS_OBJECT_ID",
     "KEY",
     "KILL",
     "LAST",
     "LAYOUT",
+    "LAZY",
     "LEADING",
     "LIFETIME",
     "LIKE",
     "LIMIT",
     "LIVE",
     "LOCAL",
     "LOGS",
     "MATERIALIZE",
     "MATERIALIZED",
+    "MATERIALIZEDMYSQL",
+    "MATERIALIZEDPOSTGRESQL",
     "MAX",
     "MERGES",
     "MIN",
     "MINUTE",
     "MODEL",
     "MODELS",
     "MODIFY",
     "MONTH",
     "MOVE",
     "MOVES",
     "MUTATION",
+    "MYSQL",
     "NAN_SQL",
     "NO",
     "NOT",
-    "NULL_SQL",
     "NULLS",
+    "NULL_SQL",
     "OFFSET",
     "OPTIMIZE",
     "OR",
     "OUTFILE",
+    "OVERRIDE",
     "POPULATE",
+    "POSTGRESQL",
     "PREWHERE",
     "PRIMARY",
     "PROFILE",
     "PROJECTION",
     "QUARTER",
     "QUOTA",
     "QUEUES",
@@ -143,14 +150,15 @@
     "SECOND",
     "SEMI",
     "SEND",
     "SENDS",
     "SETTINGS",
     "SHOW",
     "SOURCE",
+    "SQLITE",
     "START",
     "STOP",
     "SUBSTRING",
     "SYNC",
     "SYNTAX",
     "SYSTEM",
     "TABLE",
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,72 +538,31 @@
         Indent,
         Delimited(
             OneOf(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
                 Ref("NumericLiteralSegment"),
                 # Can `GROUP BY coalesce(col, 1)`
-                Ref("ExpressionSegment"),
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingSetsClauseSegment"),
+                Ref("ExpressionSegment"),
                 Bracketed(),  # Allows empty parentheses
             ),
             terminator=OneOf(
                 Sequence("ORDER", "BY"),
                 "LIMIT",
                 "HAVING",
                 "QUALIFY",
                 Ref("SetOperatorSegment"),
             ),
         ),
         Dedent,
     )
 
 
-class CubeRollupClauseSegment(BaseSegment):
-    """`CUBE` / `ROLLUP` clause within the `GROUP BY` clause."""
-
-    type = "cube_rollup_clause"
-    match_grammar = Sequence(
-        OneOf("CUBE", "ROLLUP"),
-        Bracketed(
-            Ref("GroupingExpressionList"),
-        ),
-    )
-
-
-class GroupingSetsClauseSegment(BaseSegment):
-    """`GROUPING SETS` clause within the `GROUP BY` clause."""
-
-    type = "grouping_sets_clause"
-    match_grammar = Sequence(
-        "GROUPING",
-        "SETS",
-        Bracketed(
-            Delimited(
-                Ref("CubeRollupClauseSegment"),
-                Ref("GroupingExpressionList"),
-            )
-        ),
-    )
-
-
-class GroupingExpressionList(BaseSegment):
-    """Grouping expression list within `CUBE` / `ROLLUP` `GROUPING SETS`."""
-
-    type = "grouping_expression_list"
-    match_grammar = Delimited(
-        OneOf(
-            Bracketed(Delimited(Ref("ExpressionSegment"))),
-            Ref("ExpressionSegment"),
-            Bracketed(),  # Allows empty parentheses
-        )
-    )
-
-
 class QualifyClauseSegment(BaseSegment):
     """`QUALIFY` clause within `SELECT`."""
 
     type = "qualify_clause"
     match_grammar = Sequence("QUALIFY", Ref("ExpressionSegment"))
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,21 @@
                         Ref("QuotedLiteralSegment"),
                         optional=True,
                     ),
                     optional=True,
                 ),
                 Sequence(
                     Sequence("ON", "UPDATE", optional=True),
-                    "CURRENT_TIMESTAMP",
+                    Sequence(
+                        OneOf("CURRENT_TIMESTAMP", "NOW"),
+                        Bracketed(
+                            Ref("NumericLiteralSegment", optional=True),
+                            optional=True,
+                        ),
+                    ),
                     Sequence(
                         Bracketed(Ref("NumericLiteralSegment")),
                         optional=True,
                     ),
                     optional=True,
                 ),
             ),
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     CodeSegment,
     CommentSegment,
     Delimited,
     GreedyUntil,
     Matchable,
     Ref,
     RegexLexer,
+    RegexParser,
+    SegmentGenerator,
     Sequence,
     StringLexer,
     StringParser,
     SymbolSegment,
     OneOf,
 )
 
@@ -46,14 +48,26 @@
         "localtimestamp",
         "sessiontimestamp",
         "sysdate",
         "systimestamp",
     ]
 )
 
+
+oracle_dialect.patch_lexer_matchers(
+    [
+        RegexLexer(
+            "code",
+            r"[a-zA-Z][0-9a-zA-Z_$#]*",
+            CodeSegment,
+            segment_kwargs={"type": "code"},
+        ),
+    ]
+)
+
 oracle_dialect.insert_lexer_matchers(
     [
         RegexLexer(
             "prompt_command",
             r"PROMPT([^(\r\n)])*((?=\n)|(?=\r\n))?",
             CommentSegment,
         ),
@@ -73,14 +87,22 @@
             "CASCADE",
             "CONSTRAINTS",
             optional=True,
         ),
         Ref.keyword("PURGE", optional=True),
         optional=True,
     ),
+    NakedIdentifierSegment=SegmentGenerator(
+        lambda dialect: RegexParser(
+            r"[A-Z0-9_]*[A-Z][A-Z0-9_#$]*",
+            ansi.IdentifierSegment,
+            type="naked_identifier",
+            anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+        )
+    ),
 )
 
 
 class AlterTableStatementSegment(ansi.AlterTableStatementSegment):
     """An `ALTER TABLE` statement.
 
     https://docs.oracle.com/en/database/oracle/oracle-database/21/sqlrf/ALTER-TABLE.html
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,26 @@
         RegexLexer(
             # For now we'll just treat meta syntax like comments and so just ignore
             # them. In future we may want to enhance this to actually parse them to
             # ensure they are valid meta commands.
             "meta_command",
             r"\\([^\\\r\n])+((\\\\)|(?=\n)|(?=\r\n))?",
             CommentSegment,
-        )
+        ),
+        RegexLexer(
+            # pg_stat_statements which is an official postgres extension used for
+            # storing the query logs replaces the actual literals used in the
+            # query with $n where n is integer value. This grammar is for parsing
+            # those literals.
+            # ref: https://www.postgresql.org/docs/current/pgstatstatements.html
+            "dollar_numeric_literal",
+            r"\$\d+",
+            ansi.LiteralSegment,
+            segment_kwargs={"type": "dollar_numeric_literal"},
+        ),
     ],
     before="code",  # Final thing to search for - as psql specific
 )
 
 postgres_dialect.patch_lexer_matchers(
     [
         # Patching comments to remove hash comments
@@ -281,14 +292,17 @@
         Sequence("ONLY", OptionallyBracketed(Ref("TableReferenceSegment"))),
         Sequence(Ref("TableReferenceSegment"), Ref("StarSegment")),
     ),
     RightArrowSegment=StringParser("=>", SymbolSegment, type="right_arrow"),
     OnKeywordAsIdentifierSegment=StringParser(
         "ON", ansi.IdentifierSegment, type="naked_identifier"
     ),
+    DollarNumericLiteralSegment=TypedParser(
+        "dollar_numeric_literal", ansi.LiteralSegment, type="dollar_numeric_literal"
+    ),
 )
 
 postgres_dialect.replace(
     LikeGrammar=OneOf("LIKE", "ILIKE", Sequence("SIMILAR", "TO")),
     StringBinaryOperatorGrammar=OneOf(Ref("ConcatSegment"), "COLLATE"),
     ComparisonOperatorGrammar=OneOf(
         Ref("EqualsSegment"),
@@ -467,14 +481,15 @@
         ),
         # NB: The Dedent for the indent above lives in the
         # SelectStatementSegment so that it sits in the right
         # place corresponding to the whitespace.
     ),
     LiteralGrammar=ansi_dialect.get_grammar("LiteralGrammar").copy(
         insert=[
+            Ref("DollarNumericLiteralSegment"),
             Ref("PsqlVariableGrammar"),
         ],
         before=Ref("ArrayLiteralSegment"),
     ),
     FromClauseTerminatorGrammar=ansi_dialect.get_grammar(
         "FromClauseTerminatorGrammar"
     ).copy(
@@ -1459,78 +1474,31 @@
     match_grammar = Sequence(
         "WITHIN",
         "GROUP",
         Bracketed(Ref("OrderByClauseSegment", optional=True)),
     )
 
 
-class CubeRollupClauseSegment(BaseSegment):
-    """`CUBE` / `ROLLUP` clause within the `GROUP BY` clause.
-
-    https://www.postgresql.org/docs/current/queries-table-expressions.html#QUERIES-GROUPING-SETS
-    """
-
-    type = "cube_rollup_clause"
-    match_grammar = Sequence(
-        OneOf("CUBE", "ROLLUP"),
-        Bracketed(
-            Ref("GroupingExpressionList"),
-        ),
-    )
-
-
-class GroupingSetsClauseSegment(BaseSegment):
-    """`GROUPING SETS` clause within the `GROUP BY` clause.
-
-    https://www.postgresql.org/docs/current/queries-table-expressions.html#QUERIES-GROUPING-SETS
-    """
-
-    type = "grouping_sets_clause"
-    match_grammar = Sequence(
-        "GROUPING",
-        "SETS",
-        Bracketed(
-            Delimited(
-                Ref("CubeRollupClauseSegment"),
-                Ref("GroupingExpressionList"),
-            )
-        ),
-    )
-
-
-class GroupingExpressionList(BaseSegment):
-    """Grouping expression list within `CUBE` / `ROLLUP` `GROUPING SETS`."""
-
-    type = "grouping_expression_list"
-    match_grammar = Delimited(
-        OneOf(
-            Bracketed(Delimited(Ref("ExpressionSegment"))),
-            Ref("ExpressionSegment"),
-            Bracketed(),  # Allows empty parentheses
-        )
-    )
-
-
 class GroupByClauseSegment(BaseSegment):
     """A `GROUP BY` clause like in `SELECT`."""
 
     type = "groupby_clause"
     match_grammar = Sequence(
         "GROUP",
         "BY",
         Indent,
         Delimited(
             OneOf(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
                 Ref("NumericLiteralSegment"),
-                # Can `GROUP BY coalesce(col, 1)`
-                Ref("ExpressionSegment"),
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingSetsClauseSegment"),
+                # Can `GROUP BY coalesce(col, 1)`
+                Ref("ExpressionSegment"),
                 Bracketed(),  # Allows empty parentheses
             ),
             terminator=OneOf(
                 Sequence("ORDER", "BY"),
                 "LIMIT",
                 "HAVING",
                 "QUALIFY",
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     ("CLASS_ORIGIN", "not-keyword"),
     ("CLOB", "not-keyword"),
     ("CLOSE", "non-reserved"),
     ("CLUSTER", "non-reserved"),
     ("COALESCE", "non-reserved-(cannot-be-function-or-type)"),
     ("COBOL", "not-keyword"),
     ("COLLATE", "reserved"),
-    ("COLLATION", "reserved-(can-be-function-or-type)"),
+    ("COLLATION", "non-reserved"),
     ("COLLATION_CATALOG", "not-keyword"),
     ("COLLATION_NAME", "not-keyword"),
     ("COLLATION_SCHEMA", "not-keyword"),
     ("COLLECT", "not-keyword"),
     ("COLUMN", "reserved"),
     ("COLUMNS", "non-reserved"),
     ("COLUMN_NAME", "not-keyword"),
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -2491,31 +2491,81 @@
     https://docs.snowflake.com/en/sql-reference/sql/create-procedure.html
     """
 
     type = "create_procedure_statement"
     match_grammar = Sequence(
         "CREATE",
         Sequence("OR", "REPLACE", optional=True),
+        Sequence("SECURE", optional=True),
         "PROCEDURE",
         Ref("FunctionNameSegment"),
         Ref("FunctionParameterListGrammar"),
+        Sequence("COPY", "GRANTS", optional=True),
         "RETURNS",
-        Ref("DatatypeSegment"),
-        Sequence("NOT", "NULL", optional=True),
-        "LANGUAGE",
-        OneOf("JAVASCRIPT", "SQL"),
         OneOf(
-            Sequence("CALLED", "ON", "NULL", "INPUT"),
-            Sequence("RETURNS", "NULL", "ON", "NULL", "INPUT"),
-            "STRICT",
+            Ref("DatatypeSegment"),
+            Sequence(
+                "TABLE",
+                Bracketed(Delimited(Ref("ColumnDefinitionSegment"), optional=True)),
+            ),
+        ),
+        AnySetOf(
+            Sequence("NOT", "NULL", optional=True),
+            Sequence(
+                "LANGUAGE",
+                OneOf(
+                    "JAVA",
+                    "JAVASCRIPT",
+                    "PYTHON",
+                    "SCALA",
+                    "SQL",
+                ),
+                optional=True,
+            ),
+            OneOf(
+                Sequence("CALLED", "ON", "NULL", "INPUT"),
+                Sequence("RETURNS", "NULL", "ON", "NULL", "INPUT"),
+                "STRICT",
+                optional=True,
+            ),
+            OneOf("VOLATILE", "IMMUTABLE", optional=True),
+            Sequence(
+                "RUNTIME_VERSION",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+                optional=True,
+            ),
+            Ref("CommentEqualsClauseSegment", optional=True),
+            Sequence(
+                "IMPORTS",
+                Ref("EqualsSegment"),
+                Bracketed(Delimited(Ref("QuotedLiteralSegment"))),
+                optional=True,
+            ),
+            Sequence(
+                "PACKAGES",
+                Ref("EqualsSegment"),
+                Bracketed(Delimited(Ref("QuotedLiteralSegment"))),
+                optional=True,
+            ),
+            Sequence(
+                "HANDLER",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+                optional=True,
+            ),
+            Sequence(
+                "TARGET_PATH",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+                optional=True,
+            ),
+            Sequence("EXECUTE", "AS", OneOf("CALLER", "OWNER"), optional=True),
             optional=True,
         ),
-        OneOf("VOLATILE", "IMMUTABLE", optional=True),
-        Ref("CommentEqualsClauseSegment", optional=True),
-        Sequence("EXECUTE", "AS", OneOf("CALLER", "OWNER"), optional=True),
         "AS",
         OneOf(
             Ref("DoubleQuotedUDFBody"),
             Ref("SingleQuotedUDFBody"),
             Ref("DollarQuotedUDFBody"),
         ),
     )
@@ -2540,17 +2590,18 @@
         OneOf(
             Ref("DatatypeSegment"),
             Sequence("TABLE", Bracketed(Delimited(Ref("ColumnDefinitionSegment")))),
         ),
         AnySetOf(
             Sequence("NOT", "NULL", optional=True),
             Sequence(
-                "LANGUAGE", OneOf("JAVASCRIPT", "SQL", "PYTHON", "JAVA"), optional=True
+                "LANGUAGE",
+                OneOf("JAVASCRIPT", "SQL", "PYTHON", "JAVA", "SCALA"),
+                optional=True,
             ),
-            OneOf("VOLATILE", "IMMUTABLE", optional=True),
             OneOf(
                 Sequence("CALLED", "ON", "NULL", "INPUT"),
                 Sequence("RETURNS", "NULL", "ON", "NULL", "INPUT"),
                 "STRICT",
                 optional=True,
             ),
             OneOf("VOLATILE", "IMMUTABLE", optional=True),
@@ -3391,14 +3442,15 @@
         Ref("OrReplaceGrammar", optional=True),
         OneOf(
             Sequence("NETWORK", "POLICY"),
             Sequence("RESOURCE", "MONITOR"),
             "SHARE",
             "ROLE",
             "USER",
+            "TAG",
             "WAREHOUSE",
             Sequence("NOTIFICATION", "INTEGRATION"),
             Sequence("SECURITY", "INTEGRATION"),
             Sequence("STORAGE", "INTEGRATION"),
             Sequence("MATERIALIZED", "VIEW"),
             Sequence("MASKING", "POLICY"),
             "PIPE",
@@ -3466,14 +3518,21 @@
                 optional=True,
             ),
             Sequence(
                 "COMMENT",
                 Ref("EqualsSegment"),
                 Ref("QuotedLiteralSegment"),
             ),
+            # For tags
+            Sequence(
+                "ALLOWED_VALUES",
+                Delimited(
+                    Ref("QuotedLiteralSegment"),
+                ),
+            ),
             # For network policy
             Sequence(
                 "ALLOWED_IP_LIST",
                 Ref("EqualsSegment"),
                 Bracketed(
                     Delimited(
                         Ref("QuotedLiteralSegment"),
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 ACCESS
 ACCOUNT
 ACCOUNTS
 ADD
 ADMIN
 AFTER
 ALLOWED_IP_LIST
+ALLOWED_VALUES
 ALLOW_DUPLICATE
 ALLOW_OVERLAPPING_EXECUTION
 API
 API_INTEGRATION
 APPEND_ONLY
 APPLY
 ARRAY
@@ -461,14 +462,15 @@
 ROUTINES
 ROW
 RSA_PUBLIC_KEY
 RSA_PUBLIC_KEY_2
 RUNNING
 RUNTIME_VERSION
 S3
+SCALA
 SCALING_POLICY
 SCHEDULE
 SCHEMA
 SCHEMAS
 SEARCH
 SECONDARY
 SECURE
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1799,17 +1799,17 @@
         Indent,
         OneOf(
             Delimited(
                 Ref("ColumnReferenceSegment"),
                 # Can `GROUP BY 1`
                 Ref("NumericLiteralSegment"),
                 # Can `GROUP BY coalesce(col, 1)`
-                Ref("ExpressionSegment"),
                 Ref("CubeRollupClauseSegment"),
                 Ref("GroupingSetsClauseSegment"),
+                Ref("ExpressionSegment"),
             ),
             Sequence(
                 Delimited(
                     Ref("ColumnReferenceSegment"),
                     # Can `GROUP BY 1`
                     Ref("NumericLiteralSegment"),
                     # Can `GROUP BY coalesce(col, 1)`
@@ -1853,61 +1853,14 @@
 
     match_grammar = Sequence(
         "WITH",
         OneOf("CUBE", "ROLLUP"),
     )
 
 
-class CubeRollupClauseSegment(BaseSegment):
-    """`[CUBE | ROLLUP]` clause within the `GROUP BY` clause.
-
-    https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-groupby.html
-    """
-
-    type = "cube_rollup_clause"
-
-    match_grammar = Sequence(
-        OneOf("CUBE", "ROLLUP"),
-        Bracketed(
-            Ref("GroupingExpressionList"),
-        ),
-    )
-
-
-class GroupingSetsClauseSegment(BaseSegment):
-    """`GROUPING SETS` clause within the `GROUP BY` clause."""
-
-    type = "grouping_sets_clause"
-
-    match_grammar = Sequence(
-        "GROUPING",
-        "SETS",
-        Bracketed(
-            Delimited(
-                Ref("CubeRollupClauseSegment"),
-                Ref("GroupingExpressionList"),
-            )
-        ),
-    )
-
-
-class GroupingExpressionList(BaseSegment):
-    """Grouping expression list within `CUBE` / `ROLLUP` `GROUPING SETS`."""
-
-    type = "grouping_expression_list"
-
-    match_grammar = Delimited(
-        OneOf(
-            Bracketed(Delimited(Ref("ExpressionSegment"))),
-            Ref("ExpressionSegment"),
-            Bracketed(),  # Allows empty parentheses
-        )
-    )
-
-
 class SortByClauseSegment(BaseSegment):
     """A `SORT BY` clause like in `SELECT`.
 
     This clause is mutually exclusive with SORT BY, ORDER BY and DISTRIBUTE BY.
     https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-sortby.html
     """
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,14 +591,15 @@
             Ref("BulkInsertStatementSegment"),
             Ref("AlterIndexStatementSegment"),
             Ref("CreateDatabaseScopedCredentialStatementSegment"),
             Ref("CreateExternalDataSourceStatementSegment"),
             Ref("SqlcmdCommandSegment"),
             Ref("CreateExternalFileFormat"),
             Ref("CreateExternalTableStatementSegment"),
+            Ref("DropExternalTableStatementSegment"),
         ],
         remove=[
             Ref("CreateModelStatementSegment"),
             Ref("DropModelStatementSegment"),
             Ref("DescribeStatementSegment"),
         ],
     )
@@ -5593,7 +5594,22 @@
         Ref("RoleReferenceSegment"),
         Sequence(
             "AUTHORIZATION",
             Ref("RoleReferenceSegment"),
             optional=True,
         ),
     )
+
+
+class DropExternalTableStatementSegment(BaseSegment):
+    """A `DROP EXTERNAL TABLE ...` statement.
+
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/drop-external-table-transact-sql
+    """
+
+    type = "drop_external_table_statement"
+    match_grammar = Sequence(
+        "DROP",
+        "EXTERNAL",
+        "TABLE",
+        Ref("TableReferenceSegment"),
+    )
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.1.2/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.1.2/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,24 +80,28 @@
             1, 2;
     """
 
     name = "ambiguous.column_references"
     aliases = ("L054",)
     groups: Tuple[str, ...] = ("all", "core", "ambiguous")
     config_keywords = ["group_by_and_order_by_style"]
-    crawl_behaviour = SegmentSeekerCrawler({"groupby_clause", "orderby_clause"})
+    crawl_behaviour = SegmentSeekerCrawler(
+        {"groupby_clause", "orderby_clause", "grouping_expression_list"}
+    )
     _ignore_types: List[str] = ["withingroup_clause", "window_specification"]
 
     def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """Inconsistent column references in GROUP BY/ORDER BY clauses."""
         # Config type hints
         self.group_by_and_order_by_style: str
 
         # We only care about GROUP BY/ORDER BY clauses.
-        assert context.segment.is_type("groupby_clause", "orderby_clause")
+        assert context.segment.is_type(
+            "groupby_clause", "orderby_clause", "grouping_expression_list"
+        )
 
         # Ignore Windowing clauses
         if FunctionalContext(context).parent_stack.any(sp.is_type(*self._ignore_types)):
             return LintResult(memory=context.memory)
 
         # Look at child segments and map column references to either the implicit or
         # explicit category.
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.1.2/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.1.2/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.1.2/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.1
+Version: 2.1.2
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.1/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.1.2/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.1.2/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.1/test/test_testing.py` & `sqlfluff-2.1.2/test/test_testing.py`

 * *Files identical despite different names*

