# Comparing `tmp/logprep-6.5.1.tar.gz` & `tmp/logprep-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.5.1.tar", last modified: Wed Jun 14 13:59:11 2023, max compression
+gzip compressed data, was "logprep-6.6.0.tar", last modified: Mon Jul  3 12:51:55 2023, max compression
```

## Comparing `logprep-6.5.1.tar` & `logprep-6.6.0.tar`

### file list

```diff
@@ -1,536 +1,537 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.460579 logprep-6.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-14 13:59:06.000000 logprep-6.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 13:59:06.000000 logprep-6.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-06-14 13:59:11.460579 logprep-6.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-06-14 13:59:06.000000 logprep-6.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.460579 logprep-6.5.1/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 13:59:11.460579 logprep-6.5.1/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/opensearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/connector/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/connector/s3/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.424579 logprep-6.5.1/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/amides/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/amides/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/amides/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/amides/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/amides/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.428579 logprep-6.5.1/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/grokker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/grokker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.432579 logprep-6.5.1/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/timestamp_differ/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/timestamper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/processor/timestamper/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.436579 logprep-6.5.1/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.440579 logprep-6.5.1/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.440579 logprep-6.5.1/logprep/util/grok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/grok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.416579 logprep-6.5.1/logprep/util/grok/patterns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.440579 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/aws
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/bind
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/exim
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/java
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/maven
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/rails
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/redis
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/squid
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/zeek
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/logprep/util/grok/patterns/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/aws
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/bind
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/exim
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/java
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/maven
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/mcollective-patterns
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/rails
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/redis
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok/patterns/legacy/squid
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-14 13:59:06.000000 logprep-6.5.1/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.420579 logprep-6.5.1/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-06-14 13:59:11.000000 logprep-6.5.1/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-14 13:59:11.000000 logprep-6.5.1/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:59:11.000000 logprep-6.5.1/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-14 13:59:11.000000 logprep-6.5.1/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-14 13:59:11.000000 logprep-6.5.1/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 13:59:11.000000 logprep-6.5.1/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 13:59:06.000000 logprep-6.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-14 13:59:11.460579 logprep-6.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-14 13:59:06.000000 logprep-6.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:06.000000 logprep-6.5.1/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.444579 logprep-6.5.1/tests/unit/component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_opensearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/connector/test_s3_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/exceptions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/exceptions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/exceptions/processor/test_processing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22087 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/amides/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/amides/test_amides_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/amides/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/amides/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/amides/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.448579 logprep-6.5.1/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/grokker/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/grokker/test_grokker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/grokker/test_grokker_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.452579 logprep-6.5.1/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.456579 logprep-6.5.1/tests/unit/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/timestamper/test_timestamper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/processor/timestamper/test_timestamper_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.460579 logprep-6.5.1/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:11.460579 logprep-6.5.1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-14 13:59:07.000000 logprep-6.5.1/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-06-14 13:59:07.000000 logprep-6.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-03 12:51:51.000000 logprep-6.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 12:51:51.000000 logprep-6.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-03 12:51:55.490977 logprep-6.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-07-03 12:51:51.000000 logprep-6.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.494977 logprep-6.6.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-03 12:51:55.494977 logprep-6.6.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamp_differ/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/grok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.454977 logprep-6.6.0/logprep/util/grok/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/maven
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/zeek
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/logprep/util/grok/patterns/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/maven
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/mcollective-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 12:51:51.000000 logprep-6.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 12:51:55.494977 logprep-6.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-03 12:51:51.000000 logprep-6.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_grok_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-07-03 12:51:51.000000 logprep-6.6.0/versioneer.py
```

### Comparing `logprep-6.5.1/LICENSE` & `logprep-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/PKG-INFO` & `logprep-6.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.5.1
+Version: 6.6.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.5.1 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.6.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.5.1/README.md` & `logprep-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/abc/component.py` & `logprep-6.6.0/logprep/abc/component.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/abc/connector.py` & `logprep-6.6.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/abc/getter.py` & `logprep-6.6.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/abc/input.py` & `logprep-6.6.0/logprep/abc/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/abc/output.py` & `logprep-6.6.0/logprep/abc/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/abc/processor.py` & `logprep-6.6.0/logprep/abc/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/configuration.py` & `logprep-6.6.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/confluent_kafka/input.py` & `logprep-6.6.0/logprep/connector/confluent_kafka/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/confluent_kafka/output.py` & `logprep-6.6.0/logprep/connector/confluent_kafka/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/console/output.py` & `logprep-6.6.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/dummy/input.py` & `logprep-6.6.0/logprep/connector/dummy/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/dummy/output.py` & `logprep-6.6.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/elasticsearch/output.py` & `logprep-6.6.0/logprep/connector/elasticsearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/file/input.py` & `logprep-6.6.0/logprep/connector/file/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/http/input.py` & `logprep-6.6.0/logprep/connector/http/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/json/input.py` & `logprep-6.6.0/logprep/connector/json/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/jsonl/input.py` & `logprep-6.6.0/logprep/connector/jsonl/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/jsonl/output.py` & `logprep-6.6.0/logprep/connector/jsonl/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/opensearch/output.py` & `logprep-6.6.0/logprep/connector/opensearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/connector/s3/output.py` & `logprep-6.6.0/logprep/connector/s3/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/factory.py` & `logprep-6.6.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/factory_error.py` & `logprep-6.6.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/filter/expression/filter_expression.py` & `logprep-6.6.0/logprep/filter/expression/filter_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,52 +96,38 @@
         -------
         str
             Returns dotted string.
 
         """
         return ".".join([str(i) for i in key_list])
 
-    def get_lucene_filter(self):
-        """Returns a filter string that is partially lucene complete. As lucene does not support
-        regex the corresponding regex field is left as a value inside the lucene filter such that
-        the end user can decide for themselves what they want to do with this information"""
-        return str(self)
-
 
 class Always(FilterExpression):
     """Filter expression that can be set to match always or never."""
 
     def __init__(self, value: Any):
         self._value = value
 
     def __repr__(self):
         if self._value:
-            return "TRUE"
-        return "FALSE"
+            return "*"
+        return ""
 
     def does_match(self, document: dict):
         return self._value
 
-    def get_lucene_filter(self):
-        if self._value:
-            return "*"
-        return ""
-
 
 class Not(FilterExpression):
     """Filter expression that negates a match."""
 
     def __init__(self, expression: FilterExpression):
         self.expression = expression
 
     def __repr__(self) -> str:
-        return f"NOT({str(self.expression)})"
-
-    def get_lucene_filter(self):
-        return f"NOT ({self.expression.get_lucene_filter()})"
+        return f"NOT ({str(self.expression)})"
 
     def does_match(self, document: dict) -> bool:
         return not self.expression.matches(document)
 
 
 class CompoundFilterExpression(FilterExpression):
     """Base class of filter expressions that combine other filter expressions."""
@@ -153,31 +139,25 @@
         raise NotImplementedError
 
 
 class And(CompoundFilterExpression):
     """Compound filter expression that is a logical conjunction."""
 
     def __repr__(self) -> str:
-        return f'AND({", ".join([str(i) for i in self.expressions])})'
-
-    def get_lucene_filter(self):
-        return f'({" AND ".join([exp.get_lucene_filter() for exp in self.expressions])})'
+        return f'({" AND ".join([str(exp) for exp in self.expressions])})'
 
     def does_match(self, document: dict) -> bool:
         return all((expression.matches(document) for expression in self.expressions))
 
 
 class Or(CompoundFilterExpression):
     """Compound filter expression that is a logical disjunction."""
 
     def __repr__(self) -> str:
-        return f'OR({", ".join([str(i) for i in self.expressions])})'
-
-    def get_lucene_filter(self):
-        return f'({" OR ".join([exp.get_lucene_filter() for exp in self.expressions])})'
+        return f'({" OR ".join([str(exp) for exp in self.expressions])})'
 
     def does_match(self, document: dict) -> bool:
         return any((expression.matches(document) for expression in self.expressions))
 
 
 class KeyValueBasedFilterExpression(FilterExpression):
     """Base class of filter expressions that match a certain value on a given key."""
@@ -185,17 +165,14 @@
     def __init__(self, key: List[str], expected_value: Any):
         self.key = key
         self._expected_value = expected_value
 
     def __repr__(self) -> str:
         return f"{self.as_dotted_string(self.key)}:{str(self._expected_value)}"
 
-    def get_lucene_filter(self):
-        return str(self)
-
     def does_match(self, document):
         raise NotImplementedError
 
 
 class StringFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a string."""
 
@@ -205,17 +182,14 @@
         if isinstance(value, list):
             return self._expected_value in value
         return str(value) == self._expected_value
 
     def __repr__(self) -> str:
         return f'{self.as_dotted_string(self.key)}:"{str(self._expected_value)}"'
 
-    def get_lucene_filter(self):
-        return str(self)
-
 
 class WildcardStringFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a string with wildcard support."""
 
     flags = 0
 
     wc = re.compile(r"((?:\\)*\*)")
@@ -330,15 +304,15 @@
 
     def __init__(self, key: List[str], regex: str):
         self.key = key
         self._regex = self._normalize_regex(regex)
         self._matcher = re.compile(self._regex)
 
     def __repr__(self) -> str:
-        return f"{self.as_dotted_string(self.key)}:r/{self._regex}/"
+        return f"{self.as_dotted_string(self.key)}:/{self._regex.strip('^$')}/"
 
     @staticmethod
     def _normalize_regex(regex: str) -> str:
         match = RegExFilterExpression.match_escaping_pattern.match(regex)
         if match and len(match.group("escaping")) % 2 == 0:
             end_token = ""
         else:
@@ -352,29 +326,23 @@
     def does_match(self, document: dict) -> bool:
         value = self._get_value(self.key, document)
 
         if isinstance(value, list):
             return any(filter(self._matcher.match, value))
         return self._matcher.match(str(value)) is not None
 
-    def get_lucene_filter(self):
-        return str(self)
-
 
 class Exists(FilterExpression):
     """Filter expression that returns true if a given field exists."""
 
     def __init__(self, value: list):
         self.split_field = value
 
     def __repr__(self) -> str:
-        return f'"{self.as_dotted_string(self.split_field)}"'
-
-    def get_lucene_filter(self):
-        return f"{self}: *"
+        return f"{self.as_dotted_string(self.split_field)}: *"
 
     def does_match(self, document: dict) -> bool:
         if not self.split_field:
             return False
 
         try:
             current = document
```

### Comparing `logprep-6.5.1/logprep/filter/lucene_filter.py` & `logprep-6.6.0/logprep/filter/lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/framework/pipeline.py` & `logprep-6.6.0/logprep/framework/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,17 +423,20 @@
                     if self._output:
                         self._store_extra_data(extra_data)
                     extra_outputs.append(extra_data)
             except ProcessingWarning as error:
                 self.logger.warning(str(error))
             except ProcessingCriticalError as error:
                 self.logger.error(str(error))
-                for _, output in self._output.items():
-                    if output.default:
-                        output.store_failed(str(error), self._decoder.decode(event_received), event)
+                if self._output:
+                    for _, output in self._output.items():
+                        if output.default:
+                            output.store_failed(
+                                str(error), self._decoder.decode(event_received), event
+                            )
             if not event:
                 break
         if self._processing_counter:
             self._processing_counter.increment()
             self._processing_counter.print_if_ready()
         if self.metrics:
             self.metrics.number_of_processed_events += 1
```

### Comparing `logprep-6.5.1/logprep/framework/pipeline_manager.py` & `logprep-6.6.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/framework/rule_tree/node.py` & `logprep-6.6.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.6.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
                 return priority_dict[expr.as_dotted_string(expr.expression.key)]
             except KeyError:
                 return RuleParser._sort(expr.expression, priority_dict)
         elif isinstance(expr, Exists):
             try:
                 return priority_dict[expr.as_dotted_string(expr.split_field)]
             except KeyError:
-                return repr(expr)[1:-1]
+                return repr(expr)
         else:
             try:
                 return priority_dict[expr.as_dotted_string(expr.key)]
             except KeyError:
                 return repr(expr)
 
     @staticmethod
@@ -488,15 +488,18 @@
                                 RuleParser._add_tag(rule, tag_map[expression.split_field[0]])
                         elif expression.key[0] in tag_map.keys():
                             RuleParser._add_tag(rule, tag_map[expression.key[0]])
                     # Always Expressions do not need tags
                     elif isinstance(segment, Always):
                         continue
                     else:
-                        if segment.key[0] in tag_map.keys():
+                        if (
+                            segment.key[0] in tag_map.keys()
+                            and Exists([tag_map[segment.key[0]]]) not in rule
+                        ):
                             RuleParser._add_tag(rule, tag_map[segment.key[0]])
 
     @staticmethod
     def _add_tag(rule, tag_map_value: str):
         """Add tag helper function.
 
         This function implements the functionality to add a tag for _add_special_tags().
```

### Comparing `logprep-6.5.1/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.6.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/metrics/metric.py` & `logprep-6.6.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/metrics/metric_exposer.py` & `logprep-6.6.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/metrics/metric_targets.py` & `logprep-6.6.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/amides/detection.py` & `logprep-6.6.0/logprep/processor/amides/detection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module contains classes for misuse detection and rule attribution
 as used by AMIDES."""
 
-from typing import List, Tuple, Dict
+from typing import Dict, List, Tuple
 
 from sklearn.base import BaseEstimator
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.preprocessing import MinMaxScaler
 
 from logprep.processor.amides.features import CommaSeparation
 
@@ -40,25 +40,25 @@
             self._vectorizer = model["vectorizer"]
             self._vectorizer.tokenizer = CommaSeparation()
             self._scaler = model["scaler"]
         except KeyError as err:
             raise MissingModelComponentError(err.args[0]) from err
 
     def detect(self, sample: str) -> float:
-        """Detect malicious data sample. Return probability value that estimates how likely
+        """Detect malicious data sample. Returns confidence value that estimates how likely
         given sample is malicious.
 
         Parameters
         ----------
         sample: str
             Sample string to evaluate.
 
         Returns
         -------
-        positive_probability: float
+        confidence_value: float
             Value between 0.0 and 1.0 that serves as confidence value.
         """
         feature_vector = self._vectorizer.transform([sample])
         df_value = self._clf.decision_function(feature_vector)
         scaled_df_value = self._scaler.transform(df_value.reshape(-1, 1)).flatten()[0]
 
         return scaled_df_value.item()
@@ -73,33 +73,33 @@
 
     _decision_threshold: float
 
     def __init__(self, misuse_model: dict, decision_threshold: float):
         super().__init__(misuse_model)
         self._decision_threshold = decision_threshold
 
-    def detect(self, sample: str) -> int:
+    def detect(self, sample: str) -> Tuple[bool, float]:
         """Detect if given sample is malicious. Returns 0 or 1 if sample's detection
         result is below or above the configured decision threshold.
 
         Parameters
         ----------
         sample: str
             Sample string to evaluate.
 
         Returns
         -------
-        predict: int.
-            0 or 1 if classified as benign or malicious.
+        predict: Tuple[boolean, float].
+            Detection result as boolean value and the corresponding confidence.
         """
         confidence_value = super().detect(sample)
 
         if confidence_value >= self._decision_threshold:
-            return 1
-        return 0
+            return True, round(confidence_value, 3)
+        return False, round(confidence_value, 3)
 
 
 class RuleAttributorError(BaseException):
     """Base class for all RuleAttributor-related Errors."""
 
 
 class RuleAttributor:
@@ -124,39 +124,37 @@
         for rule_name, rule_model in models.items():
             try:
                 rule_model = DetectionModel(rule_model)
                 self._rule_models[rule_name] = rule_model
             except DetectionModelError as err:
                 raise RuleAttributorError from err
 
-    def attribute(self, sample: str) -> Dict[str, float]:
+    def attribute(self, sample: str) -> List[dict]:
         """Attribute given sample to rules of which the attributor holds rule models.
 
         Parameters
         ----------
         sample: str
             Malicious sample to attribute.
 
         Returns
         -------
-        attributions: Dict[str, float]
+        attributions: List[dict]
             List of rule attributions, containing rule model names and confidence values.
         """
         conf_values = self._calculate_rule_confidence_values(sample)
 
         return self._get_rules_with_highest_confidence_values(conf_values)
 
-    def _calculate_rule_confidence_values(self, cmdline: str) -> List[Tuple[str, float]]:
+    def _calculate_rule_confidence_values(self, cmdline: str) -> List[dict]:
         conf_values = []
 
         for name, rule_model in self._rule_models.items():
             rule_confidence_value = rule_model.detect(cmdline)
-            conf_values.append((name, round(rule_confidence_value, 3)))
+            conf_values.append({"rule": name, "confidence": round(rule_confidence_value, 3)})
 
         return conf_values
 
-    def _get_rules_with_highest_confidence_values(
-        self, conf_values: List[Tuple[str, float]]
-    ) -> Dict[str, float]:
-        conf_values.sort(key=lambda item: item[1], reverse=True)
+    def _get_rules_with_highest_confidence_values(self, conf_values: List[dict]) -> List[dict]:
+        conf_values.sort(key=lambda item: item["confidence"], reverse=True)
 
-        return dict(conf_values[: self._num_rule_attributions])
+        return conf_values[: self._num_rule_attributions]
```

### Comparing `logprep-6.5.1/logprep/processor/amides/features.py` & `logprep-6.6.0/logprep/processor/amides/features.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/amides/normalize.py` & `logprep-6.6.0/logprep/processor/amides/normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/amides/processor.py` & `logprep-6.6.0/logprep/processor/amides/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
    :members:
    :undoc-members:
    :inherited-members:
    :noindex:
 
 .. automodule:: logprep.processor.amides.rule
 """
-from functools import lru_cache, cached_property
+from functools import cached_property, lru_cache
 from multiprocessing import current_process
 from pathlib import Path
 from time import time
 from typing import List, Tuple
 from zipfile import ZipFile
 
 import joblib
@@ -214,34 +214,35 @@
         normalized = self._normalizer.normalize(cmdline)
         if not normalized:
             return
 
         result = self._evaluate_cmdline_cached(normalized)
         self._update_cache_metrics()
 
-        if result:
-            self._write_target_field(event=event, rule=rule, result=result)
+        self._write_target_field(event=event, rule=rule, result=result)
 
     def _evaluate_cmdline(self, cmdline: str):
-        result = self._perform_misuse_detection(cmdline)
-        if result == 0:
-            return []
+        result = {}
 
-        return self._calculate_rule_attributions(cmdline)
+        malicious, result["confidence"] = self._perform_misuse_detection(cmdline)
+        if malicious:
+            result["attributions"] = self._calculate_rule_attributions(cmdline)
 
-    def _perform_misuse_detection(self, cmdline: str) -> int:
+        return result
+
+    def _perform_misuse_detection(self, cmdline: str) -> Tuple[bool, float]:
         begin = time()
         result = self._misuse_detector.detect(cmdline)
         processing_time = time() - begin
 
         self.metrics.update_mean_misuse_detection_time(processing_time)
 
         return result
 
-    def _calculate_rule_attributions(self, cmdline: str) -> List[Tuple[str, int]]:
+    def _calculate_rule_attributions(self, cmdline: str) -> List[dict]:
         begin = time()
         attributions = self._rule_attributor.attribute(cmdline)
         processing_time = time() - begin
 
         self.metrics.update_mean_rule_attribution_time(processing_time)
 
         return attributions
```

### Comparing `logprep-6.5.1/logprep/processor/amides/rule.py` & `logprep-6.6.0/logprep/processor/amides/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,11 +48,9 @@
             validator=[
                 validators.instance_of(list),
                 validators.deep_iterable(member_validator=validators.instance_of(str)),
                 validators.min_len(1),
                 validators.max_len(1),
             ]
         )
-        target_field: str = field(
-            validator=validators.instance_of(str), default="rule_attributions"
-        )
+        target_field: str = field(validator=validators.instance_of(str), default="amides")
         mapping: dict = field(default="", init=False, repr=False, eq=False)
```

### Comparing `logprep-6.5.1/logprep/processor/base/exceptions.py` & `logprep-6.6.0/logprep/processor/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/base/rule.py` & `logprep-6.6.0/logprep/processor/base/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         return all([other.filter == self._filter, other._config == self._config])
 
     def __hash__(self) -> int:  # pylint: disable=function-redefined
         return id(self)
 
     def __repr__(self) -> str:
         if hasattr(self, "_config"):
-            return f"filename={self.file_name}, filter={self.filter}, {self._config}"
+            return f"filename={self.file_name}, filter='{self.filter}', {self._config}"
         return super().__repr__()
 
     # pylint: disable=C0111
     @property
     def filter(self):
         return self._filter
```

### Comparing `logprep-6.5.1/logprep/processor/calculator/fourFn.py` & `logprep-6.6.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/calculator/processor.py` & `logprep-6.6.0/logprep/processor/calculator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/calculator/rule.py` & `logprep-6.6.0/logprep/processor/calculator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/clusterer/processor.py` & `logprep-6.6.0/logprep/processor/clusterer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/clusterer/rule.py` & `logprep-6.6.0/logprep/processor/clusterer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.6.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/concatenator/processor.py` & `logprep-6.6.0/logprep/processor/concatenator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/concatenator/rule.py` & `logprep-6.6.0/logprep/processor/concatenator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/datetime_extractor/processor.py` & `logprep-6.6.0/logprep/processor/datetime_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/datetime_extractor/rule.py` & `logprep-6.6.0/logprep/processor/datetime_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/deleter/processor.py` & `logprep-6.6.0/logprep/processor/deleter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/deleter/rule.py` & `logprep-6.6.0/logprep/processor/deleter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/dissector/processor.py` & `logprep-6.6.0/logprep/processor/dissector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/dissector/rule.py` & `logprep-6.6.0/logprep/processor/dissector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.6.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,18 @@
         if self._config.tld_lists:
             downloaded_tld_lists_paths = []
             self._logger.debug("start tldlists download...")
             for index, tld_list in enumerate(self._config.tld_lists):
                 logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
                 os.makedirs(logprep_tmp_dir, exist_ok=True)
                 list_path = logprep_tmp_dir / f"{self.name}-tldlist-{index}.dat"
-                with FileLock(list_path):
-                    list_path.touch()
-                    list_path.write_bytes(GetterFactory.from_string(tld_list).get_raw())
+                if not os.path.isfile(list_path):
+                    with FileLock(list_path):
+                        list_path.touch()
+                        list_path.write_bytes(GetterFactory.from_string(tld_list).get_raw())
                 downloaded_tld_lists_paths.append(f"file://{str(list_path.absolute())}")
             self._config.tld_lists = downloaded_tld_lists_paths
             self._logger.debug("finished tldlists download...")
 
     def _apply_rules(self, event, rule: DomainLabelExtractorRule):
         """
         Apply matching rule to given log event. Such that a given domain,
```

### Comparing `logprep-6.5.1/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.6.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/domain_resolver/processor.py` & `logprep-6.6.0/logprep/processor/domain_resolver/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,18 @@
         if self._config.tld_lists:
             downloaded_tld_lists_paths = []
             self._logger.debug("start tldlists download...")
             for index, tld_list in enumerate(self._config.tld_lists):
                 logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
                 os.makedirs(logprep_tmp_dir, exist_ok=True)
                 list_path = logprep_tmp_dir / f"{self.name}-tldlist-{index}.dat"
-                with FileLock(list_path):
-                    list_path.touch()
-                    list_path.write_bytes(GetterFactory.from_string(tld_list).get_raw())
+                if not os.path.isfile(list_path):
+                    with FileLock(list_path):
+                        list_path.touch()
+                        list_path.write_bytes(GetterFactory.from_string(tld_list).get_raw())
                 downloaded_tld_lists_paths.append(f"file://{str(list_path.absolute())}")
             self._config.tld_lists = downloaded_tld_lists_paths
             self._logger.debug("finished tldlists download...")
 
     def _apply_rules(self, event, rule):
         source_field = rule.source_fields[0]
         domain_or_url_str = get_dotted_field_value(event, source_field)
```

### Comparing `logprep-6.5.1/logprep/processor/domain_resolver/rule.py` & `logprep-6.6.0/logprep/processor/domain_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/dropper/processor.py` & `logprep-6.6.0/logprep/processor/dropper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/dropper/rule.py` & `logprep-6.6.0/logprep/processor/dropper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/field_manager/processor.py` & `logprep-6.6.0/logprep/processor/field_manager/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/field_manager/rule.py` & `logprep-6.6.0/logprep/processor/field_manager/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.6.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/generic_adder/processor.py` & `logprep-6.6.0/logprep/processor/generic_adder/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/generic_adder/rule.py` & `logprep-6.6.0/logprep/processor/generic_adder/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/generic_resolver/processor.py` & `logprep-6.6.0/logprep/processor/generic_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/generic_resolver/rule.py` & `logprep-6.6.0/logprep/processor/generic_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/geoip_enricher/processor.py` & `logprep-6.6.0/logprep/processor/geoip_enricher/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,19 +70,20 @@
         super().setup()
         db_path = Path(self._config.db_path)
         if not db_path.exists():
             self._logger.debug("start geoip database download...")
             logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
             os.makedirs(logprep_tmp_dir, exist_ok=True)
             db_path_file = logprep_tmp_dir / f"{self.name}.mmdb"
-            with FileLock(db_path_file):
-                db_path_file.touch()
-                db_path_file.write_bytes(
-                    GetterFactory.from_string(str(self._config.db_path)).get_raw()
-                )
+            if not os.path.isfile(db_path_file):
+                with FileLock(db_path_file):
+                    db_path_file.touch()
+                    db_path_file.write_bytes(
+                        GetterFactory.from_string(str(self._config.db_path)).get_raw()
+                    )
             self._logger.debug("finished geoip database download.")
             self._config.db_path = str(db_path_file.absolute())
 
     def _try_getting_geoip_data(self, ip_string):
         try:
             ip_addr = str(ip_address(ip_string))
             ip_data = self._city_db.city(ip_addr)
```

### Comparing `logprep-6.5.1/logprep/processor/geoip_enricher/rule.py` & `logprep-6.6.0/logprep/processor/geoip_enricher/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/grokker/processor.py` & `logprep-6.6.0/logprep/processor/grokker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/grokker/rule.py` & `logprep-6.6.0/logprep/processor/grokker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.6.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.6.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/ip_informer/processor.py` & `logprep-6.6.0/logprep/processor/ip_informer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/ip_informer/rule.py` & `logprep-6.6.0/logprep/processor/ip_informer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/key_checker/processor.py` & `logprep-6.6.0/logprep/processor/key_checker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/key_checker/rule.py` & `logprep-6.6.0/logprep/processor/key_checker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/labeler/labeling_schema.py` & `logprep-6.6.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/labeler/processor.py` & `logprep-6.6.0/logprep/processor/labeler/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/labeler/rule.py` & `logprep-6.6.0/logprep/processor/labeler/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/list_comparison/processor.py` & `logprep-6.6.0/logprep/processor/list_comparison/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/list_comparison/rule.py` & `logprep-6.6.0/logprep/processor/list_comparison/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/normalizer/processor.py` & `logprep-6.6.0/logprep/processor/normalizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/normalizer/rule.py` & `logprep-6.6.0/logprep/processor/normalizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.6.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/pre_detector/processor.py` & `logprep-6.6.0/logprep/processor/pre_detector/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,13 @@
             self._event["pre_detection_id"] = str(uuid4())
 
         detection_results.append(self._generate_detection_result(rule))
 
     def _generate_detection_result(self, rule: PreDetectorRule):
         detection_result = rule.detection_data
         detection_result["rule_filter"] = rule.filter_str
-        detection_result["lucene_filter"] = rule.lucene_filter
         detection_result["description"] = rule.description
         detection_result["pre_detection_id"] = self._event["pre_detection_id"]
         if "host" in self._event and "name" in self._event["host"]:
             detection_result["host"] = {"name": self._event["host"]["name"]}
 
         return detection_result
```

### Comparing `logprep-6.5.1/logprep/processor/processor_strategy.py` & `logprep-6.6.0/logprep/processor/processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.6.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/pseudonymizer/processor.py` & `logprep-6.6.0/logprep/processor/pseudonymizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/pseudonymizer/rule.py` & `logprep-6.6.0/logprep/processor/pseudonymizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/requester/processor.py` & `logprep-6.6.0/logprep/processor/requester/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/requester/rule.py` & `logprep-6.6.0/logprep/processor/requester/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/selective_extractor/processor.py` & `logprep-6.6.0/logprep/processor/selective_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/selective_extractor/rule.py` & `logprep-6.6.0/logprep/processor/selective_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/string_splitter/processor.py` & `logprep-6.6.0/logprep/processor/string_splitter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/string_splitter/rule.py` & `logprep-6.6.0/logprep/processor/string_splitter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/template_replacer/processor.py` & `logprep-6.6.0/logprep/processor/template_replacer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/template_replacer/rule.py` & `logprep-6.6.0/logprep/processor/template_replacer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/timestamp_differ/processor.py` & `logprep-6.6.0/logprep/processor/timestamp_differ/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/timestamp_differ/rule.py` & `logprep-6.6.0/logprep/processor/timestamp_differ/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/timestamper/processor.py` & `logprep-6.6.0/logprep/processor/timestamper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/processor/timestamper/rule.py` & `logprep-6.6.0/logprep/processor/timestamper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/registry.py` & `logprep-6.6.0/logprep/registry.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/run_logprep.py` & `logprep-6.6.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/runner.py` & `logprep-6.6.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/aggregating_logger.py` & `logprep-6.6.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,31 @@
 
 from logprep.framework.pipeline import Pipeline
 from logprep.util.configuration import Configuration
 from logprep.util.helper import get_dotted_field_value
 from logprep.util.json_handling import parse_json
 
 
+def align_extra_output_formats(extra_outputs):
+    """
+    Aligns the different output formats into one common format of the selective_extractor,
+    predetector and pseudonymizer.
+    """
+    reformatted_extra_outputs = []
+    for extra_output in extra_outputs:
+        if isinstance(extra_output, tuple):
+            documents, target = extra_output
+            for document in documents:
+                reformatted_extra_outputs.append({str(target): document})
+        else:
+            for output in extra_output:
+                reformatted_extra_outputs.append({str(output[1]): output[0][0]})
+    return reformatted_extra_outputs
+
+
 class RuleCorpusTester:
     """This class can test a rule corpus against expected outputs"""
 
     _tmp_dir: str
     """ Temporary directory where test files will be saved temporarily """
 
     _original_config_path: str
@@ -185,33 +202,21 @@
         For each test case the logprep connector files are rewritten (only the current test case
         will be added to the input file), the pipline is run and the outputs are compared.
         """
         print(Style.BRIGHT + "# Test Cases Summary:" + Style.RESET_ALL)
         for test_case_id, test_case in self._test_cases.items():
             _ = [processor.setup() for processor in self._pipeline._pipeline]
             parsed_event, extra_outputs = self._pipeline.process_pipeline()
-            extra_outputs = self._align_extra_output_formats(extra_outputs)
+            extra_outputs = align_extra_output_formats(extra_outputs)
             test_case.generated_output = parsed_event
             test_case.generated_extra_output = extra_outputs
             self._compare_logprep_outputs(test_case_id, parsed_event)
             self._compare_extra_data_output(test_case_id, extra_outputs)
             self._print_pass_fail_statements(test_case_id)
 
-    def _align_extra_output_formats(self, extra_outputs):
-        reformatted_extra_outputs = []
-        for extra_output in extra_outputs:
-            if isinstance(extra_output, tuple):
-                documents, target = extra_output
-                for document in documents:
-                    reformatted_extra_outputs.append({str(target): document})
-            else:
-                for output in extra_output:
-                    reformatted_extra_outputs.append({str(output[1]): output[0][0]})
-        return reformatted_extra_outputs
-
     def _compare_logprep_outputs(self, test_case_id, logprep_output):
         test_case = self._test_cases.get(test_case_id, {})
         if test_case.expected_output:
             diff = self._compare_events(logprep_output, test_case.expected_output)
             self._extract_print_statements_from_diff(test_case_id, diff)
 
     def _compare_extra_data_output(self, test_case_id, logprep_extra_outputs):
```

### Comparing `logprep-6.5.1/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.6.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/cache.py` & `logprep-6.6.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/configuration.py` & `logprep-6.6.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/decorators.py` & `logprep-6.6.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/getter.py` & `logprep-6.6.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/grok.py` & `logprep-6.6.0/logprep/util/grok/grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/aws` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/bacula` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/bind` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bind`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/bro` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/exim` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/firewalls` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/grok-patterns` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/haproxy` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/httpd` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/java` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/java`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/junos` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/linux-syslog` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/mongodb` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/nagios` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/rails` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/squid` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/squid`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/ecs-v1/zeek` & `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/zeek`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/aws` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/bacula` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/bro` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/exim` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/firewalls` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/grok-patterns` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/haproxy` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/httpd` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/java` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/java`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/junos` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/linux-syslog` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/mongodb` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/nagios` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok/patterns/legacy/rails` & `logprep-6.6.0/logprep/util/grok/patterns/legacy/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/grok_pattern_loader.py` & `logprep-6.6.0/logprep/util/grok_pattern_loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """This module contains a loader for grok patterns."""
 
-from typing import Optional
 from os import walk, path
+from typing import Optional
+
+PATTERN_CONVERSION = [("[[:alnum:]]", r"\w")]
 
 
 class GrokPatternLoaderError(BaseException):
     """Base class for GrokPatternLoader related exceptions."""
 
     def __init__(self, message: str):
         super().__init__(f"GrokPatternLoader: {message}")
@@ -46,28 +48,28 @@
 
         Returns
         -------
         grok_pattern_dict: dict
             Dictionary with grok patterns.
 
         """
-        grok_pattern_dict = dict()
+        grok_pattern_dict = {}
         with open(pattern_path, "r", encoding="utf8") as pattern_file:
             lines = pattern_file.readlines()
             lines = [line for line in lines if line.strip() and not line.startswith("#")]
             for idx, line in enumerate(lines):
                 line = line.rstrip("\n") if idx != len(lines) - 1 else line
                 identifier, pattern = line.split(" ", 1)
 
                 if identifier in grok_pattern_dict:
                     raise GrokPatternLoaderError(
                         f"Duplicate pattern definition - Pattern: " f'"{identifier}"'
                     )
                 grok_pattern_dict[identifier] = pattern
-        return grok_pattern_dict
+        return GrokPatternLoader._update_pattern(grok_pattern_dict)
 
     @staticmethod
     def load_from_dir(pattern_dir_path: str) -> dict:
         """Load grok patterns from path to file.
 
         Parameters
         ----------
@@ -76,18 +78,28 @@
 
         Returns
         -------
         grok_pattern_dict: dict
             Dictionary with grok patterns.
 
         """
-        grok_pattern_dict = dict()
+        grok_pattern_dict = {}
         for root, _, files in walk(pattern_dir_path):
             for file in files:
                 new_patterns = GrokPatternLoader.load_from_file(path.join(root, file))
                 intersection = set(grok_pattern_dict).intersection(new_patterns)
                 if intersection:
                     raise GrokPatternLoaderError(
                         f'Duplicate pattern definition across files - Patterns: "{intersection}"'
                     )
                 grok_pattern_dict.update(new_patterns)
         return grok_pattern_dict
+
+    @staticmethod
+    def _update_pattern(grok_pattern_dict) -> dict:
+        return {
+            grok: pattern.replace(non_supported_regex, supported_regex)
+            if non_supported_regex in pattern
+            else pattern
+            for grok, pattern in grok_pattern_dict.items()
+            for non_supported_regex, supported_regex in PATTERN_CONVERSION
+        }
```

### Comparing `logprep-6.5.1/logprep/util/hasher.py` & `logprep-6.6.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/helper.py` & `logprep-6.6.0/logprep/util/helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/json_handling.py` & `logprep-6.6.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/log_aggregator.py` & `logprep-6.6.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/multiprocessing_log_handler.py` & `logprep-6.6.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/pipeline_profiler.py` & `logprep-6.6.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.6.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/processor_generator.py` & `logprep-6.6.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/prometheus_exporter.py` & `logprep-6.6.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/rule_dry_runner.py` & `logprep-6.6.0/logprep/util/rule_dry_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from difflib import ndiff
 from functools import cached_property
 
 from colorama import Back, Fore
 from ruamel.yaml import YAML
 
 from logprep.framework.pipeline import Pipeline
+from logprep.util.auto_rule_tester.auto_rule_corpus_tester import align_extra_output_formats
 from logprep.util.configuration import Configuration
 from logprep.util.getter import GetterFactory
 from logprep.util.helper import color_print_line, color_print_title, recursive_compare
 
 yaml = YAML(typ="safe", pure=True)
 
 
@@ -74,15 +75,18 @@
         config = Configuration.create_from_yaml(patched_config_path)
         config.verify_pipeline_without_processor_outputs(self._logger)
         del config["output"]
         return Pipeline(config=config)
 
     @cached_property
     def _input_documents(self):
-        return GetterFactory.from_string(self._input_file_path).get_jsonl()
+        document_getter = GetterFactory.from_string(self._input_file_path)
+        if self._use_json:
+            return [document_getter.get_json()]
+        return document_getter.get_jsonl()
 
     def __init__(
         self, input_file_path: str, config_path: str, full_output: bool, use_json: bool, logger
     ):
         self._input_file_path = input_file_path
         self._config_path = config_path
         self._full_output = full_output
@@ -91,14 +95,15 @@
 
     def run(self):
         """Run the dry runner."""
         transformed_cnt = 0
         output_count = 0
         for input_document in self._input_documents:
             test_output, test_output_custom = self._pipeline.process_pipeline()
+            test_output_custom = align_extra_output_formats(test_output_custom)
             if test_output:
                 output_count += 1
             diff = self._print_output_results(input_document, test_output, test_output_custom)
             if diff:
                 transformed_cnt += 1
         color_print_title(Back.WHITE, f"TRANSFORMED EVENTS: {transformed_cnt}/{output_count}")
         shutil.rmtree(self._tmp_path)
@@ -129,12 +134,12 @@
             elif item.startswith("? "):
                 color_print_line(Back.BLACK, Fore.WHITE, item)
             else:
                 color_print_line(Back.BLACK, Fore.CYAN, item)
 
     def _print_custom_outputs(self, test_output_custom):
         color_print_title(Back.MAGENTA, "CUSTOM OUTPUTS")
-        for output, output_target in test_output_custom:
-            color_print_title(Back.YELLOW, f"Output Target: {str(output_target[0])}")
-            for out in output:
-                test_json = json.dumps(out, sort_keys=True, indent=4)
-                color_print_line(Back.BLACK, Fore.YELLOW, test_json)
+        for custom_output in test_output_custom:
+            output_target, output = list(custom_output.items())[0]
+            color_print_title(Back.YELLOW, f"Output Target: {output_target}")
+            test_json = json.dumps(output, sort_keys=True, indent=4)
+            color_print_line(Back.BLACK, Fore.YELLOW, test_json)
```

### Comparing `logprep-6.5.1/logprep/util/schema_and_rule_checker.py` & `logprep-6.6.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/time.py` & `logprep-6.6.0/logprep/util/time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/time_measurement.py` & `logprep-6.6.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep/util/validators.py` & `logprep-6.6.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/logprep.egg-info/PKG-INFO` & `logprep-6.6.0/logprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.5.1
+Version: 6.6.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.5.1 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.6.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.5.1/logprep.egg-info/SOURCES.txt` & `logprep-6.6.0/logprep.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,15 @@
 tests/unit/processor/timestamper/test_timestamper_rule.py
 tests/unit/util/__init__.py
 tests/unit/util/test_auto_rule_corpus_tester.py
 tests/unit/util/test_auto_rule_tester.py
 tests/unit/util/test_cache.py
 tests/unit/util/test_configuration.py
 tests/unit/util/test_getter.py
+tests/unit/util/test_grok_pattern.py
 tests/unit/util/test_grok_pattern_loader.py
 tests/unit/util/test_hasher.py
 tests/unit/util/test_helper.py
 tests/unit/util/test_helper_add_field.py
 tests/unit/util/test_log_aggregator.py
 tests/unit/util/test_processor_generator.py
 tests/unit/util/test_prometheus_exporter.py
```

### Comparing `logprep-6.5.1/setup.py` & `logprep-6.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_amides.py` & `logprep-6.6.0/tests/acceptance/test_amides.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python3
 # pylint: disable=not-an-iterable
 # pylint: disable=missing-docstring
 
-from logging import getLogger, DEBUG, basicConfig
+from logging import DEBUG, basicConfig, getLogger
 
 import pytest
 
 from logprep.util.json_handling import dump_config_as_file
 from tests.acceptance.util import get_test_output
 
-
 basicConfig(level=DEBUG, format="%(asctime)-15s %(name)-5s %(levelname)-8s: %(message)s")
 logger = getLogger("Logprep-Test")
 
 
 @pytest.fixture
 def config():
     config_yml = {
@@ -51,11 +50,13 @@
 
 
 def test_amides(tmp_path, config):
     config_path = str(tmp_path / "generated_config.yml")
     dump_config_as_file(config_path, config)
 
     test_output = get_test_output(config_path)
-    test_output_documents = [
-        event for event in test_output[0] if event.get("rule_attributions", None)
+    test_output_documents = [event for event in test_output[0] if event.get("amides")]
+    attributed_documents = [
+        event for event in test_output_documents if event.get("amides").get("attributions")
     ]
-    assert len(test_output_documents) == 8
+    assert len(test_output_documents) == 20
+    assert len(attributed_documents) == 8
```

### Comparing `logprep-6.5.1/tests/acceptance/test_config_refresh.py` & `logprep-6.6.0/tests/acceptance/test_config_refresh.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_file_input.py` & `logprep-6.6.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_full_configuration.py` & `logprep-6.6.0/tests/acceptance/test_full_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_http_input.py` & `logprep-6.6.0/tests/acceptance/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_multiple_outputs.py` & `logprep-6.6.0/tests/acceptance/test_multiple_outputs.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_pre_detection.py` & `logprep-6.6.0/tests/acceptance/test_pre_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,36 @@
             {"@timestamp":"2019-08-02T09:46:20.000Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"kind":"event","code":6005,"created":"2019-08-02T09:55:11.996Z"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86","os":{"version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows"},"name":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"},"log":{"level":"information"},"message":"The Event log service was started.","winlog":{"provider_name":"EventLog","task":"","channel":"System","event_data":{"Binary":"E30708000500020009002E00140057010000000000000000"},"event_id":6005,"computer_name":"abcdefg1234","keywords":["Classic"],"record_id":11571,"api":"wineventlog"}},
             {"@timestamp":"2019-08-02T09:46:20.000Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"kind":"event","code":6005,"created":"2019-08-02T09:55:11.996Z"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86","os":{"version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows"},"name":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"},"log":{"level":"information"},"message":"The Event log service was started.","winlog":{"provider_name":"EventLog","task":"","channel":"System","event_data":{"Binary":"E30708000500020009002E00140057010000000000000000"},"event_id":6005,"computer_name":"abcdefg1234","keywords":["Classic"],"record_id":11571,"api":"wineventlog"}},
             None
         ),
         (
             {"@timestamp":"2019-07-30T14:38:16.352Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"code":7036,"created":"2019-08-02T09:55:11.996Z","kind":"event"},"agent":{"version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0"},"ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4"},"log":{"level":"information"},"message":"The Software Protection service entered the stopped state.","winlog":{"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_id":1234,"task":"","api":"wineventlog","event_data":{"Binary":"7300700070007300760063002F0031000000","param1":"Software Protection","param2":"stopped"},"keywords":["Classic"],"provider_name":"Service Control Manager","record_id":11580,"channel":"System","computer_name":"abcdefg1234","process":{"thread":{"id":2808},"pid":436}}},
             {"@timestamp":"2019-07-30T14:38:16.352Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"event":{"code":7036,"created":"2019-08-02T09:55:11.996Z","kind":"event"},"agent":{"version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0"},"ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4"},"log":{"level":"information"},"message":"The Software Protection service entered the stopped state.","winlog":{"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_id":1234,"task":"","api":"wineventlog","event_data":{"Binary":"7300700070007300760063002F0031000000","param1":"Software Protection","param2":"stopped"},"keywords":["Classic"],"provider_name":"Service Control Manager","record_id":11580,"channel":"System","computer_name":"abcdefg1234","process":{"thread":{"id":2808},"pid":436}}},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "1cf39644-a632-4c42-a7b4-2896c4efffb5", "host": {"name": "CLIENT1"}, "@timestamp": "2019-07-30T14:38:16.352Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "1cf39644-a632-4c42-a7b4-2896c4efffb5", "host": {"name": "CLIENT1"}, "@timestamp": "2019-07-30T14:38:16.352Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:46:41.906Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"host":{"name":"CLIENT1","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86"},"agent":{"hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9"},"ecs":{"version":"1.0.0"},"winlog":{"channel":"System","provider_name":"Service Control Manager","record_id":11627,"event_id":1234,"api":"wineventlog","keywords":["Classic"],"computer_name":"abcdefg1234","process":{"pid":440,"thread":{"id":524}},"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_data":{"param1":"Wazuh","param2":"running","Binary":"4F0073007300650063005300760063002F0034000000"},"task":""},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:11.998Z"},"log":{"level":"information"},"message":"The Wazuh service entered the running state."},
             {"@timestamp":"2019-08-02T09:46:41.906Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"host":{"name":"CLIENT1","os":{"name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1","architecture":"x86"},"agent":{"hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9"},"ecs":{"version":"1.0.0"},"winlog":{"channel":"System","provider_name":"Service Control Manager","record_id":11627,"event_id":1234,"api":"wineventlog","keywords":["Classic"],"computer_name":"abcdefg1234","process":{"pid":440,"thread":{"id":524}},"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","event_data":{"param1":"Wazuh","param2":"running","Binary":"4F0073007300650063005300760063002F0034000000"},"task":""},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:11.998Z"},"log":{"level":"information"},"message":"The Wazuh service entered the running state."},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "08d1aa6f-f508-464e-a13d-0b5da46b5bcc", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:41.906Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "08d1aa6f-f508-464e-a13d-0b5da46b5bcc", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:41.906Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:46:54.583Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"provider_name":"Service Control Manager","computer_name":"abcdefg1234","provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","process":{"pid":440,"thread":{"id":1792}},"event_data":{"param1":"Portable Device Enumerator Service","param2":"running","Binary":"57005000440042007500730045006E0075006D002F0034000000"},"channel":"System","record_id":11638,"task":"","api":"wineventlog","event_id":1234,"keywords":["Classic"]},"event":{"code":7036,"created":"2019-08-02T09:55:11.999Z","kind":"event"},"agent":{"ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0"}},"log":{"level":"information"},"message":"The Portable Device Enumerator Service service entered the running state."},
             {"@timestamp":"2019-08-02T09:46:54.583Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"provider_name":"Service Control Manager","computer_name":"abcdefg1234","provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","process":{"pid":440,"thread":{"id":1792}},"event_data":{"param1":"Portable Device Enumerator Service","param2":"running","Binary":"57005000440042007500730045006E0075006D002F0034000000"},"channel":"System","record_id":11638,"task":"","api":"wineventlog","event_id":1234,"keywords":["Classic"]},"event":{"code":7036,"created":"2019-08-02T09:55:11.999Z","kind":"event"},"agent":{"ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1","id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat"},"ecs":{"version":"1.0.0"},"host":{"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","name":"CLIENT1","hostname":"CLIENT1","architecture":"x86","os":{"platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional","kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0"}},"log":{"level":"information"},"message":"The Portable Device Enumerator Service service entered the running state."},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "06d12743-01f0-4793-8a31-3815cfa31fc3", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:54.583Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "06d12743-01f0-4793-8a31-3815cfa31fc3", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:46:54.583Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager 2","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager 2","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', 'lucene_filter': 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
         ),
         (
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
             {"@timestamp":"2019-08-02T09:54:57.125Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"7.2.0","topic":"wineventlog_raw"},"winlog":{"computer_name":"abcdefg1234","event_id":123,"record_id":11714,"provider_guid":"{555908d1-a6d7-4695-8e1e-26931d2012f4}","channel":"System","task":"","api":"wineventlog","event_data":{"param2":"running","Binary":"41007500640069006F007300720076002F0034000000","param1":"Windows Audio"},"provider_name":"Service Control Manager","keywords":["Classic"],"process":{"pid":440,"thread":{"id":528}}},"event":{"kind":"event","code":7036,"created":"2019-08-02T09:55:12.091Z"},"log":{"level":"information"},"message":"The Windows Audio service entered the running state.","ecs":{"version":"1.0.0"},"host":{"name":"CLIENT1","architecture":"x86","os":{"kernel":"6.1.7601.18741 (win7sp1_gdr.150202-1526)","build":"7601.0","platform":"windows","version":"6.1","family":"windows","name":"Windows 7 Professional"},"id":"19fc45ac-5890-4f96-81b1-50ed111c0ce4","hostname":"CLIENT1"},"agent":{"id":"0b755aca-0a9a-454a-9800-1979901962a0","version":"7.2.0","type":"winlogbeat","ephemeral_id":"de845cd9-5141-4c92-ad32-27a4518307e9","hostname":"CLIENT1"}},
-            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', 'lucene_filter': 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}},
-             {"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', 'lucene_filter': 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
+            [{"pre_detector_topic": {"description": "", "id": "RULE_ONE_ID", "title": "RULE_ONE", "severity": "critical", "mitre": ["mitre1", "mitre2"], "case_condition": "directly", "rule_filter": 'winlog.provider_name:"Service Control Manager"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}},
+             {"pre_detector_topic": {"description": "", "id": "RULE_TWO_ID", "title": "RULE_TWO", "severity": "critical", "mitre": ["mitre2", "mitre3"], "case_condition": "directly", "rule_filter": 'winlog.event_id:"123"', "pre_detection_id": "638cc0b3-b912-4220-8551-defea8ea139d", "host": {"name": "CLIENT1"}, "@timestamp": "2019-08-02T09:54:57.125Z"}}]
         ),
     ],
 )
 # fmt: on
 def test_events_pre_detected_correctly(
     tmp_path, input_event, expected_output_event, expected_extra_output
 ):
```

### Comparing `logprep-6.5.1/tests/acceptance/test_preprocessing.py` & `logprep-6.6.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.6.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.6.0/tests/acceptance/test_wineventlog_normalization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_wineventlog_processing.py` & `logprep-6.6.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.6.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/acceptance/util.py` & `logprep-6.6.0/tests/acceptance/util.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.6.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/testdata/ConfigurationForTest.py` & `logprep-6.6.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/testdata/FilledTempFile.py` & `logprep-6.6.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/testdata/metadata.py` & `logprep-6.6.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/testdata/ruledata.py` & `logprep-6.6.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.6.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/component/base.py` & `logprep-6.6.0/tests/unit/component/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/base.py` & `logprep-6.6.0/tests/unit/connector/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.6.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.6.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.6.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_console_output.py` & `logprep-6.6.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_dummy_input.py` & `logprep-6.6.0/tests/unit/connector/test_dummy_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_dummy_output.py` & `logprep-6.6.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.6.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.6.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.6.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.6.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_http_input.py` & `logprep-6.6.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_json_input.py` & `logprep-6.6.0/tests/unit/connector/test_json_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_jsonl_input.py` & `logprep-6.6.0/tests/unit/connector/test_jsonl_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_jsonl_output.py` & `logprep-6.6.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_opensearch_output.py` & `logprep-6.6.0/tests/unit/connector/test_opensearch_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/connector/test_s3_output.py` & `logprep-6.6.0/tests/unit/connector/test_s3_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/exceptions/processor/test_processing_warning.py` & `logprep-6.6.0/tests/unit/exceptions/processor/test_processing_warning.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from logprep.processor.base.rule import Rule
 
 
 class TestProcessingWarning:
     exception = ProcessingWarning
 
     error_message = """ProcessingWarning in Dissector (my_dissector): the error message
-Rule: filename=None, filter="message", Rule.Config(description='', regex_fields=[], tests=[], tag_on_failure=['_rule_failure']),
+Rule: filename=None, filter='message: *', Rule.Config(description='', regex_fields=[], tests=[], tag_on_failure=['_rule_failure']),
 Event: {'message': 'test_event'}
 """
 
     def setup_method(self):
         self.processor = Factory.create(
             {"my_dissector": {"type": "dissector", "specific_rules": [], "generic_rules": []}},
             getLogger(),
@@ -39,14 +39,14 @@
             raise self.exception(*self.exception_args)
         assert self.processor.metrics.number_of_warnings == 1
 
 
 class TestFieldExsitsWarning(TestProcessingWarning):
     exception = FieldExistsWarning
     error_message = """FieldExistsWarning in Dissector (my_dissector): The following fields could not be written, because one or more subfields existed and could not be extended: my_field
-Rule: filename=None, filter="message", Rule.Config(description='', regex_fields=[], tests=[], tag_on_failure=[\'_rule_failure\']),
+Rule: filename=None, filter='message: *', Rule.Config(description='', regex_fields=[], tests=[], tag_on_failure=[\'_rule_failure\']),
 Event: {'message': 'test_event'}
 """
 
     def setup_method(self):
         super().setup_method()
         self.exception_args = (self.processor, self.rule, self.event, ["my_field"])
```

### Comparing `logprep-6.5.1/tests/unit/filter/test_filter_expression.py` & `logprep-6.6.0/tests/unit/filter/test_filter_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
 
 class TestAlways:
     def setup_class(self):
         self.documents = [{}, {"key": "value"}, {"integer": 42}]
 
     def test_string_representation(self):
-        assert str(Always(True)) == "TRUE"
-        assert str(Always(False)) == "FALSE"
+        assert str(Always(True)) == "*"
+        assert str(Always(False)) == ""
 
     def test_different_objects_with_same_payload_are_equal(self):
         filter1 = Always(False)
         filter2 = Always(False)
 
         assert filter1 == filter2
 
@@ -63,15 +63,15 @@
     def test_true_is_true_regardless_of_document(self):
         for document in self.documents:
             assert Always(True).matches(document)
 
 
 class TestNot:
     def test_string_representation(self):
-        assert str(Not(Always(True))) == "NOT(TRUE)"
+        assert str(Not(Always(True))) == "NOT (*)"
 
     def test_different_objects_with_same_payload_are_equal(self):
         not_filter1 = Not(Always(True))
         not_filter2 = Not(Always(True))
 
         assert not_filter1 == not_filter2
 
@@ -82,15 +82,16 @@
     def test_a_false_becomes_true(self):
         not_filter = Not(Always(False))
         assert not_filter.matches({})
 
 
 class TestAnd:
     def test_string_representation(self):
-        assert str(And(Always(True))) == "AND(TRUE)"
+        assert str(And(Exists(["foo"]))) == "(foo: *)"
+        assert str(And(Exists(["foo"]), Exists(["bar"]))) == "(foo: * AND bar: *)"
 
     def test_different_objects_with_same_payload_are_equal(self):
         and_filter1 = And(Always(False))
         and_filter2 = And(Always(False))
 
         assert and_filter1 == and_filter2
 
@@ -120,15 +121,16 @@
                         assert and_filter.matches({})
                     else:
                         assert not and_filter.matches({})
 
 
 class TestOr:
     def test_string_representation(self):
-        assert str(Or(Always(True))) == "OR(TRUE)"
+        assert str(Or(Exists(["foo"]))) == "(foo: *)"
+        assert str(Or(Exists(["foo"]), Exists(["bar"]))) == "(foo: * OR bar: *)"
 
     def test_different_objects_with_same_payload_are_equal(self):
         or_filter1 = Or(Always(False))
         or_filter2 = Or(Always(False))
 
         assert or_filter1 == or_filter2
 
@@ -278,15 +280,15 @@
 class TestRegExFilterExpression(ValueBasedFilterExpressionTest):
     def setup_method(self, _):
         self.regex = "start.*end"
         self.filter = RegExFilterExpression(["key1", "key2"], self.regex)
         self.filter_identical = RegExFilterExpression(["key1", "key2"], self.regex)
 
     def test_string_representation(self):
-        assert str(self.filter) == "key1.key2:r/^start.*end$/"
+        assert str(self.filter) == "key1.key2:/start.*end/"
 
     def test_does_not_match_if_key_is_missing(self):
         assert not self.filter.matches({"not": {"the": {"key": "to match"}}})
 
     def test_empty_regex_matches_nothing(self):
         filter = RegExFilterExpression(["key1", "key2"], "")
         for length in range(1, 20):
@@ -336,15 +338,15 @@
 class TestExistsFilterExpression(ValueBasedFilterExpressionTest):
     def setup_method(self, _):
         self.split_field = ["key1", "key2"]
         self.filter = Exists(["key1", "key2"])
         self.filter_identical = Exists(["key1", "key2"])
 
     def test_string_representation(self):
-        assert str(self.filter) == '"key1.key2"'
+        assert str(self.filter) == "key1.key2: *"
 
     def test_matches_any_value(self):
         filter = Exists(["key1", "key2"])
         assert filter.matches({"key1": {"key2": ""}})
         assert filter.matches({"key1": {"key2": "foo"}})
         assert filter.matches({"key1": {"key2": "bar"}})
 
@@ -524,19 +526,19 @@
         assert _filter.escaped_expected == expected_expression
 
 
 class TestLuceneRepresentation:
     @pytest.mark.parametrize(
         "logprep_filter_language, special_fields, expected_lucene_filter_query",
         [
-            ("exist_field", None, '"exist_field": *'),
+            ("exist_field", None, "exist_field: *"),
             ("key: value", None, 'key:"value"'),
             ("dotted.key: value", None, 'dotted.key:"value"'),
             ("*", None, "*"),
-            ("NOT key", None, 'NOT ("key": *)'),
+            ("NOT key", None, "NOT (key: *)"),
             ("NOT key: value", None, 'NOT (key:"value")'),
             ("key: value1 AND keyy: value2", None, '(key:"value1" AND keyy:"value2")'),
             (
                 "key: value1 AND keyy: value2 AND keyyy: value3",
                 None,
                 '(key:"value1" AND keyy:"value2" AND keyyy:"value3")',
             ),
@@ -555,25 +557,24 @@
                 "key: value1 AND (keyy: value2 OR NOT keyyy: value3)",
                 None,
                 '(key:"value1" AND (keyy:"value2" OR NOT (keyyy:"value3")))',
             ),
             ("key: val*", None, 'key:"val*"'),
             ("key: 1", None, 'key:"1"'),
             ("key: 1.0", None, 'key:"1.0"'),
-            (r"key: field\[\d\].*", {"regex_fields": ["key"]}, r"key:r/^field\[\d\].*$/"),
+            (r"key: field\[\d\].*", {"regex_fields": ["key"]}, r"key:/field\[\d\].*/"),
             (
                 r"nonRegexKey: something AND key: field\[\d\].*",
                 {"regex_fields": ["key"]},
-                r'(nonRegexKey:"something" AND key:r/^field\[\d\].*$/)',
+                r'(nonRegexKey:"something" AND key:/field\[\d\].*/)',
             ),
         ],
     )
     def test_convert_filter_to_best_closest_lucene_language(
         self, logprep_filter_language, special_fields, expected_lucene_filter_query
     ):
         filter_expression = LuceneFilter.create(
             logprep_filter_language, special_fields=special_fields
         )
-        lucene_filter = filter_expression.get_lucene_filter()
         assert (
-            lucene_filter == expected_lucene_filter_query
-        ), f"Expected: '{expected_lucene_filter_query}', but got: '{lucene_filter}'"
+            str(filter_expression) == expected_lucene_filter_query
+        ), f"Expected: '{expected_lucene_filter_query}', but got: '{filter_expression}'"
```

### Comparing `logprep-6.5.1/tests/unit/filter/test_lucene_filter.py` & `logprep-6.6.0/tests/unit/filter/test_lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.6.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,501 +18,541 @@
 str5 = StringFilterExpression(["key5", "subkey5"], "value5")
 
 ex1 = Exists(["ABC.def"])
 ex2 = Exists(["xyz"])
 
 
 class TestRuleParser:
-    def test_parse_rule(self):
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "foo: bar",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [[Exists(["foo"]), StringFilterExpression(["foo"], "bar")]]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "foo: bar AND bar: foo",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["bar"]),
-                StringFilterExpression(["bar"], "foo"),
-                Exists(["foo"]),
-                StringFilterExpression(["foo"], "bar"),
-            ]
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "foo: bar OR bar: foo",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [Exists(["foo"]), StringFilterExpression(["foo"], "bar")],
-            [Exists(["bar"]), StringFilterExpression(["bar"], "foo")],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "winlog: 123 AND test: (Good OR Okay OR Bad) OR foo: bar",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["test"]),
-                StringFilterExpression(["test"], "Good"),
-                Exists(["winlog"]),
-                StringFilterExpression(["winlog"], "123"),
-            ],
-            [
-                Exists(["test"]),
-                StringFilterExpression(["test"], "Okay"),
-                Exists(["winlog"]),
-                StringFilterExpression(["winlog"], "123"),
-            ],
-            [
-                Exists(["test"]),
-                StringFilterExpression(["test"], "Bad"),
-                Exists(["winlog"]),
-                StringFilterExpression(["winlog"], "123"),
-            ],
-            [Exists(["foo"]), StringFilterExpression(["foo"], "bar")],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "(EventID: 1 AND ABC AND foo: bar)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["ABC"]),
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "1"),
-                Exists(["foo"]),
-                StringFilterExpression(["foo"], "bar"),
-            ]
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "(EventID: 17 AND PipeName: \\PSHost*) AND NOT (Image: *\\powershell.exe)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "17"),
-                Not(StringFilterExpression(["Image"], "*\\powershell.exe")),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "\\PSHost*"),
-            ]
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "EventID: (17 OR 18) AND PipeName: (atctl OR userpipe OR iehelper)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "17"),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "atctl"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "17"),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "userpipe"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "17"),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "iehelper"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "18"),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "atctl"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "18"),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "userpipe"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "18"),
-                Exists(["PipeName"]),
-                StringFilterExpression(["PipeName"], "iehelper"),
-            ],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "EventID: 8 AND "
-                "SourceImage: (*System32cscript.exe OR *System32wscript.exe OR *System32mshta.exe) AND "
-                "TargetImage: *SysWOW64\\* AND NOT StartModule",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "8"),
-                Exists(["SourceImage"]),
-                StringFilterExpression(["SourceImage"], "*System32cscript.exe"),
-                Not(Exists(["StartModule"])),
-                Exists(["TargetImage"]),
-                StringFilterExpression(["TargetImage"], "*SysWOW64\\*"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "8"),
-                Exists(["SourceImage"]),
-                StringFilterExpression(["SourceImage"], "*System32wscript.exe"),
-                Not(Exists(["StartModule"])),
-                Exists(["TargetImage"]),
-                StringFilterExpression(["TargetImage"], "*SysWOW64\\*"),
-            ],
-            [
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "8"),
-                Exists(["SourceImage"]),
-                StringFilterExpression(["SourceImage"], "*System32mshta.exe"),
-                Not(Exists(["StartModule"])),
-                Exists(["TargetImage"]),
-                StringFilterExpression(["TargetImage"], "*SysWOW64\\*"),
-            ],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "(EventID: 12 AND TargetObject: *cmmgr32.exe*) "
-                "OR (EventID: 13 AND TargetObject: *cmmgr32.exe*) "
-                "OR (EventID: 10 AND CallTrace: *cmlua.dll*)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(
-            rule, {"EventID": "1"}, {"TargetObject": "TAG", "CallTrace": "Key.subkey:Value"}
-        )
-        assert parsed_rule == [
-            [
-                Exists(["TAG"]),
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "12"),
-                Exists(["TargetObject"]),
-                StringFilterExpression(["TargetObject"], "*cmmgr32.exe*"),
-            ],
-            [
-                Exists(["TAG"]),
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "13"),
-                Exists(["TargetObject"]),
-                StringFilterExpression(["TargetObject"], "*cmmgr32.exe*"),
-            ],
-            [
-                StringFilterExpression(["Key", "subkey"], "Value"),
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "10"),
-                Exists(["CallTrace"]),
-                StringFilterExpression(["CallTrace"], "*cmlua.dll*"),
-            ],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "bar: foo AND NOT foo: bar",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["bar"]),
-                StringFilterExpression(["bar"], "foo"),
-                Not(StringFilterExpression(["foo"], "bar")),
-            ]
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "NOT bar",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        tag_map = {"bar": "tag"}
-        parsed_rule = RP.parse_rule(rule, {}, tag_map)
-        assert parsed_rule == [[Exists(["tag"]), Not(Exists(["bar"]))]]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "winlog.event_id: 7036 AND NOT Something",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Not(Exists(["Something"])),
-                Exists(["winlog", "event_id"]),
-                StringFilterExpression(["winlog", "event_id"], "7036"),
-            ]
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "NOT (foo: bar AND (test: ok OR msg: (123 OR 456)))",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [Not(StringFilterExpression(["foo"], "bar"))],
-            [
-                Not(StringFilterExpression(["msg"], "123")),
-                Not(StringFilterExpression(["msg"], "456")),
-                Not(StringFilterExpression(["test"], "ok")),
-            ],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "winlog.channel: Security AND "
-                "winlog.event_id: 4625 AND "
-                "NOT ((winlog.channel: Security AND "
-                "(winlog.event_data.IpAddress: *-* OR winlog.event_data.IpAddress: (10.* OR 192.168.*) "
-                "OR "
-                "winlog.event_data.IpAddress: 1 "
-                "OR "
-                "winlog.event_data.IpAddress: (fe80* OR fc00*))))",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "process.parent: (foo OR bar) AND process.executable: cmd.exe AND process.command_line: (perl OR python)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Exists(["process", "command_line"]),
-                StringFilterExpression(["process", "command_line"], "perl"),
-                Exists(["process", "executable"]),
-                StringFilterExpression(["process", "executable"], "cmd.exe"),
-                Exists(["process", "parent"]),
-                StringFilterExpression(["process", "parent"], "foo"),
-            ],
-            [
-                Exists(["process", "command_line"]),
-                StringFilterExpression(["process", "command_line"], "python"),
-                Exists(["process", "executable"]),
-                StringFilterExpression(["process", "executable"], "cmd.exe"),
-                Exists(["process", "parent"]),
-                StringFilterExpression(["process", "parent"], "foo"),
-            ],
-            [
-                Exists(["process", "command_line"]),
-                StringFilterExpression(["process", "command_line"], "perl"),
-                Exists(["process", "executable"]),
-                StringFilterExpression(["process", "executable"], "cmd.exe"),
-                Exists(["process", "parent"]),
-                StringFilterExpression(["process", "parent"], "bar"),
-            ],
-            [
-                Exists(["process", "command_line"]),
-                StringFilterExpression(["process", "command_line"], "python"),
-                Exists(["process", "executable"]),
-                StringFilterExpression(["process", "executable"], "cmd.exe"),
-                Exists(["process", "parent"]),
-                StringFilterExpression(["process", "parent"], "bar"),
-            ],
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "EventID: 15 AND NOT (Imphash: 000 OR NOT AImphash)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [
-                Not(Not(Exists(["AImphash"]))),
-                Exists(["EventID"]),
-                StringFilterExpression(["EventID"], "15"),
-                Not(StringFilterExpression(["Imphash"], "000")),
-            ]
-        ]
-
-        rule = PreDetectorRule._create_from_dict(
-            {
-                "filter": "(A1 OR A2) AND (B1 OR B2) AND (C1 OR C2) AND (D1 OR D2)",
-                "pre_detector": {
-                    "id": 1,
-                    "title": "1",
-                    "severity": "0",
-                    "case_condition": "directly",
-                    "mitre": [],
-                },
-            }
-        )
-
-        parsed_rule = RP.parse_rule(rule, {}, {})
-        assert parsed_rule == [
-            [Exists(["A1"]), Exists(["B1"]), Exists(["C1"]), Exists(["D1"])],
-            [Exists(["A1"]), Exists(["B1"]), Exists(["C1"]), Exists(["D2"])],
-            [Exists(["A1"]), Exists(["B1"]), Exists(["C2"]), Exists(["D1"])],
-            [Exists(["A1"]), Exists(["B1"]), Exists(["C2"]), Exists(["D2"])],
-            [Exists(["A1"]), Exists(["B2"]), Exists(["C1"]), Exists(["D1"])],
-            [Exists(["A1"]), Exists(["B2"]), Exists(["C1"]), Exists(["D2"])],
-            [Exists(["A1"]), Exists(["B2"]), Exists(["C2"]), Exists(["D1"])],
-            [Exists(["A1"]), Exists(["B2"]), Exists(["C2"]), Exists(["D2"])],
-            [Exists(["A1"]), Exists(["C1"]), Exists(["D1"])],
-            [Exists(["A1"]), Exists(["C1"]), Exists(["D2"])],
-            [Exists(["A1"]), Exists(["C2"]), Exists(["D1"])],
-            [Exists(["A1"]), Exists(["C2"]), Exists(["D2"])],
-            [Exists(["A2"]), Exists(["B1"]), Exists(["C1"]), Exists(["D1"])],
-            [Exists(["A2"]), Exists(["B1"]), Exists(["C1"]), Exists(["D2"])],
-            [Exists(["A2"]), Exists(["B1"]), Exists(["C2"]), Exists(["D1"])],
-            [Exists(["A2"]), Exists(["B1"]), Exists(["C2"]), Exists(["D2"])],
-            [Exists(["A2"]), Exists(["B2"]), Exists(["C1"]), Exists(["D1"])],
-            [Exists(["A2"]), Exists(["B2"]), Exists(["C1"]), Exists(["D2"])],
-            [Exists(["A2"]), Exists(["B2"]), Exists(["C2"]), Exists(["D1"])],
-            [Exists(["A2"]), Exists(["B2"]), Exists(["C2"]), Exists(["D2"])],
-            [Exists(["A2"]), Exists(["C1"]), Exists(["D1"])],
-            [Exists(["A2"]), Exists(["C1"]), Exists(["D2"])],
-            [Exists(["A2"]), Exists(["C2"]), Exists(["D1"])],
-            [Exists(["A2"]), Exists(["C2"]), Exists(["D2"])],
-        ]
+    @pytest.mark.parametrize(
+        "rule, priority_dict, tag_map, expected_expressions",
+        [
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "foo: bar",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [[Exists(["foo"]), StringFilterExpression(["foo"], "bar")]],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "foo: bar AND bar: foo",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["bar"]),
+                        StringFilterExpression(["bar"], "foo"),
+                        Exists(["foo"]),
+                        StringFilterExpression(["foo"], "bar"),
+                    ]
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "foo: bar OR bar: foo",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [Exists(["foo"]), StringFilterExpression(["foo"], "bar")],
+                    [Exists(["bar"]), StringFilterExpression(["bar"], "foo")],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "winlog: 123 AND test: (Good OR Okay OR Bad) OR foo: bar",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["test"]),
+                        StringFilterExpression(["test"], "Good"),
+                        Exists(["winlog"]),
+                        StringFilterExpression(["winlog"], "123"),
+                    ],
+                    [
+                        Exists(["test"]),
+                        StringFilterExpression(["test"], "Okay"),
+                        Exists(["winlog"]),
+                        StringFilterExpression(["winlog"], "123"),
+                    ],
+                    [
+                        Exists(["test"]),
+                        StringFilterExpression(["test"], "Bad"),
+                        Exists(["winlog"]),
+                        StringFilterExpression(["winlog"], "123"),
+                    ],
+                    [Exists(["foo"]), StringFilterExpression(["foo"], "bar")],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "(EventID: 1 AND ABC AND foo: bar)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["ABC"]),
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "1"),
+                        Exists(["foo"]),
+                        StringFilterExpression(["foo"], "bar"),
+                    ]
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "(EventID: 17 AND PipeName: \\PSHost*) AND NOT (Image: *\\powershell.exe)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "17"),
+                        Not(StringFilterExpression(["Image"], "*\\powershell.exe")),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "\\PSHost*"),
+                    ]
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "EventID: (17 OR 18) AND PipeName: (atctl OR userpipe OR iehelper)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "17"),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "atctl"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "17"),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "userpipe"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "17"),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "iehelper"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "18"),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "atctl"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "18"),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "userpipe"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "18"),
+                        Exists(["PipeName"]),
+                        StringFilterExpression(["PipeName"], "iehelper"),
+                    ],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "EventID: 8 AND "
+                        "SourceImage: (*System32cscript.exe OR *System32wscript.exe OR *System32mshta.exe) AND "
+                        "TargetImage: *SysWOW64\\* AND NOT StartModule",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "8"),
+                        Exists(["SourceImage"]),
+                        StringFilterExpression(["SourceImage"], "*System32cscript.exe"),
+                        Not(Exists(["StartModule"])),
+                        Exists(["TargetImage"]),
+                        StringFilterExpression(["TargetImage"], "*SysWOW64\\*"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "8"),
+                        Exists(["SourceImage"]),
+                        StringFilterExpression(["SourceImage"], "*System32wscript.exe"),
+                        Not(Exists(["StartModule"])),
+                        Exists(["TargetImage"]),
+                        StringFilterExpression(["TargetImage"], "*SysWOW64\\*"),
+                    ],
+                    [
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "8"),
+                        Exists(["SourceImage"]),
+                        StringFilterExpression(["SourceImage"], "*System32mshta.exe"),
+                        Not(Exists(["StartModule"])),
+                        Exists(["TargetImage"]),
+                        StringFilterExpression(["TargetImage"], "*SysWOW64\\*"),
+                    ],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "bar: foo AND NOT foo: bar",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["bar"]),
+                        StringFilterExpression(["bar"], "foo"),
+                        Not(StringFilterExpression(["foo"], "bar")),
+                    ]
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "winlog.event_id: 7036 AND NOT Something",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Not(Exists(["Something"])),
+                        Exists(["winlog", "event_id"]),
+                        StringFilterExpression(["winlog", "event_id"], "7036"),
+                    ]
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "NOT (foo: bar AND (test: ok OR msg: (123 OR 456)))",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [Not(StringFilterExpression(["foo"], "bar"))],
+                    [
+                        Not(StringFilterExpression(["msg"], "123")),
+                        Not(StringFilterExpression(["msg"], "456")),
+                        Not(StringFilterExpression(["test"], "ok")),
+                    ],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "process.parent: (foo OR bar) AND process.executable: cmd.exe AND process.command_line: (perl OR python)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Exists(["process", "command_line"]),
+                        StringFilterExpression(["process", "command_line"], "perl"),
+                        Exists(["process", "executable"]),
+                        StringFilterExpression(["process", "executable"], "cmd.exe"),
+                        Exists(["process", "parent"]),
+                        StringFilterExpression(["process", "parent"], "foo"),
+                    ],
+                    [
+                        Exists(["process", "command_line"]),
+                        StringFilterExpression(["process", "command_line"], "python"),
+                        Exists(["process", "executable"]),
+                        StringFilterExpression(["process", "executable"], "cmd.exe"),
+                        Exists(["process", "parent"]),
+                        StringFilterExpression(["process", "parent"], "foo"),
+                    ],
+                    [
+                        Exists(["process", "command_line"]),
+                        StringFilterExpression(["process", "command_line"], "perl"),
+                        Exists(["process", "executable"]),
+                        StringFilterExpression(["process", "executable"], "cmd.exe"),
+                        Exists(["process", "parent"]),
+                        StringFilterExpression(["process", "parent"], "bar"),
+                    ],
+                    [
+                        Exists(["process", "command_line"]),
+                        StringFilterExpression(["process", "command_line"], "python"),
+                        Exists(["process", "executable"]),
+                        StringFilterExpression(["process", "executable"], "cmd.exe"),
+                        Exists(["process", "parent"]),
+                        StringFilterExpression(["process", "parent"], "bar"),
+                    ],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "EventID: 15 AND NOT (Imphash: 000 OR NOT AImphash)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [
+                        Not(Not(Exists(["AImphash"]))),
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "15"),
+                        Not(StringFilterExpression(["Imphash"], "000")),
+                    ]
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "(A1 OR A2) AND (B1 OR B2) AND (C1 OR C2) AND (D1 OR D2)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                [
+                    [Exists(["A1"]), Exists(["B1"]), Exists(["C1"]), Exists(["D1"])],
+                    [Exists(["A1"]), Exists(["B1"]), Exists(["C1"]), Exists(["D2"])],
+                    [Exists(["A1"]), Exists(["B1"]), Exists(["C2"]), Exists(["D1"])],
+                    [Exists(["A1"]), Exists(["B1"]), Exists(["C2"]), Exists(["D2"])],
+                    [Exists(["A1"]), Exists(["B2"]), Exists(["C1"]), Exists(["D1"])],
+                    [Exists(["A1"]), Exists(["B2"]), Exists(["C1"]), Exists(["D2"])],
+                    [Exists(["A1"]), Exists(["B2"]), Exists(["C2"]), Exists(["D1"])],
+                    [Exists(["A1"]), Exists(["B2"]), Exists(["C2"]), Exists(["D2"])],
+                    [Exists(["A1"]), Exists(["C1"]), Exists(["D1"])],
+                    [Exists(["A1"]), Exists(["C1"]), Exists(["D2"])],
+                    [Exists(["A1"]), Exists(["C2"]), Exists(["D1"])],
+                    [Exists(["A1"]), Exists(["C2"]), Exists(["D2"])],
+                    [Exists(["A2"]), Exists(["B1"]), Exists(["C1"]), Exists(["D1"])],
+                    [Exists(["A2"]), Exists(["B1"]), Exists(["C1"]), Exists(["D2"])],
+                    [Exists(["A2"]), Exists(["B1"]), Exists(["C2"]), Exists(["D1"])],
+                    [Exists(["A2"]), Exists(["B1"]), Exists(["C2"]), Exists(["D2"])],
+                    [Exists(["A2"]), Exists(["B2"]), Exists(["C1"]), Exists(["D1"])],
+                    [Exists(["A2"]), Exists(["B2"]), Exists(["C1"]), Exists(["D2"])],
+                    [Exists(["A2"]), Exists(["B2"]), Exists(["C2"]), Exists(["D1"])],
+                    [Exists(["A2"]), Exists(["B2"]), Exists(["C2"]), Exists(["D2"])],
+                    [Exists(["A2"]), Exists(["C1"]), Exists(["D1"])],
+                    [Exists(["A2"]), Exists(["C1"]), Exists(["D2"])],
+                    [Exists(["A2"]), Exists(["C2"]), Exists(["D1"])],
+                    [Exists(["A2"]), Exists(["C2"]), Exists(["D2"])],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "winlog.channel: Security AND "
+                        "winlog.event_id: 4625 AND "
+                        "NOT ((winlog.channel: Security AND "
+                        "(winlog.event_data.IpAddress: *-* OR winlog.event_data.IpAddress: (10.* OR 192.168.*) "
+                        "OR "
+                        "winlog.event_data.IpAddress: 1 "
+                        "OR "
+                        "winlog.event_data.IpAddress: (fe80* OR fc00*))))",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {},
+                None,
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "(EventID: 12 AND TargetObject: *cmmgr32.exe*) "
+                        "OR (EventID: 13 AND TargetObject: *cmmgr32.exe*) "
+                        "OR (EventID: 10 AND CallTrace: *cmlua.dll*)",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {"EventID": "1"},
+                {"TargetObject": "TAG", "CallTrace": "Key.subkey:Value"},
+                [
+                    [
+                        Exists(["TAG"]),
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "12"),
+                        Exists(["TargetObject"]),
+                        StringFilterExpression(["TargetObject"], "*cmmgr32.exe*"),
+                    ],
+                    [
+                        Exists(["TAG"]),
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "13"),
+                        Exists(["TargetObject"]),
+                        StringFilterExpression(["TargetObject"], "*cmmgr32.exe*"),
+                    ],
+                    [
+                        StringFilterExpression(["Key", "subkey"], "Value"),
+                        Exists(["EventID"]),
+                        StringFilterExpression(["EventID"], "10"),
+                        Exists(["CallTrace"]),
+                        StringFilterExpression(["CallTrace"], "*cmlua.dll*"),
+                    ],
+                ],
+            ),
+            (
+                PreDetectorRule._create_from_dict(
+                    {
+                        "filter": "NOT bar",
+                        "pre_detector": {
+                            "id": 1,
+                            "title": "1",
+                            "severity": "0",
+                            "case_condition": "directly",
+                            "mitre": [],
+                        },
+                    }
+                ),
+                {},
+                {"bar": "tag"},
+                [[Exists(["tag"]), Not(Exists(["bar"]))]],
+            ),
+        ],
+    )
+    def test_parse_rule_param(self, rule, priority_dict, tag_map, expected_expressions):
+        if expected_expressions is not None:
+            assert RP.parse_rule(rule, priority_dict, tag_map) == expected_expressions
+        else:
+            assert RP.parse_rule(rule, priority_dict, tag_map)
 
     def test_has_unresolved_not_expression(self):
         exp = And(str1, str2)
         assert not RP._has_unresolved_not_expression(exp)
 
         exp = Not(str1)
         assert not RP._has_unresolved_not_expression(exp)
```

### Comparing `logprep-6.5.1/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/framework/test_pipeline.py` & `logprep-6.6.0/tests/unit/framework/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.6.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.6.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/metrics/test_metric_targets.py` & `logprep-6.6.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/metrics/test_metrics.py` & `logprep-6.6.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/amides/test_amides.py` & `logprep-6.6.0/tests/unit/processor/amides/test_amides.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,17 +34,20 @@
                 "event_data": {"CommandLine": "cmd.exe /c taskkill.exe /im cmd.exe"},
             },
         }
 
         self.object.process(document)
         assert self.object.metrics.number_of_processed_events == 1
 
-        rule_attributions = document.get("rule_attributions", None)
-        assert rule_attributions
-        assert len(rule_attributions) == 10
+        result = document.get("amides")
+        assert result
+        assert result["confidence"] >= self.CONFIG.get("decision_threshold") and result.get(
+            "attributions"
+        )
+        assert len(result["attributions"]) == 10
         assert self.object.metrics.total_cmdlines == 1
         assert self.object.metrics.new_results == 1
         assert self.object.metrics.num_cache_entries == 1
         assert self.object.metrics.cache_load == 0.2
         assert self.object.metrics.mean_misuse_detection_time != 0.0
         assert self.object.metrics.mean_rule_attribution_time != 0.0
 
@@ -56,15 +59,19 @@
                 "event_id": 1,
                 "provider_name": "Microsoft-Windows-Sysmon",
                 "event_data": {"CommandLine": "C:\\Windows\\system32\\svchost.exe -k DcomLaunch"},
             },
         }
         self.object.process(document)
         assert self.object.metrics.number_of_processed_events == 1
-        assert not document.get("rule_attributions")
+        result = document.get("amides")
+        assert result
+        assert result["confidence"] < self.CONFIG.get("decision_threshold") and not result.get(
+            "attributions"
+        )
         assert self.object.metrics.total_cmdlines == 1
         assert self.object.metrics.new_results == 1
         assert self.object.metrics.num_cache_entries == 1
         assert self.object.metrics.cache_load == 0.2
         assert self.object.metrics.mean_misuse_detection_time != 0.0
         assert self.object.metrics.mean_rule_attribution_time == 0.0
 
@@ -78,15 +85,15 @@
     @pytest.mark.parametrize("document", no_pc_events)
     def test_process_event_no_process_creation_events(self, document):
         self.object.setup()
         assert self.object.metrics.number_of_processed_events == 0
 
         self.object.process(document)
         assert self.object.metrics.number_of_processed_events == 1
-        assert not document.get("rule_attributions")
+        assert not document.get("amides")
         assert self.object.metrics.total_cmdlines == 0
         assert self.object.metrics.new_results == 0
         assert self.object.metrics.num_cache_entries == 0
         assert self.object.metrics.cache_load == 0.0
         assert self.object.metrics.mean_misuse_detection_time == 0.0
         assert self.object.metrics.mean_rule_attribution_time == 0.0
 
@@ -96,15 +103,15 @@
         document = {
             "winlog": {"event_id": 1, "provider_name": "Microsoft-Windows-Sysmon"},
             "some": {"random": "data"},
         }
 
         self.object.process(document)
         assert self.object.metrics.number_of_processed_events == 1
-        assert not document.get("rule_attributions")
+        assert not document.get("amides")
         assert self.object.metrics.total_cmdlines == 0
         assert self.object.metrics.new_results == 0
         assert self.object.metrics.num_cache_entries == 0
         assert self.object.metrics.cache_load == 0.0
         assert self.object.metrics.mean_misuse_detection_time == 0.0
         assert self.object.metrics.mean_rule_attribution_time == 0.0
 
@@ -120,15 +127,15 @@
         }
         other_document = deepcopy(document)
 
         self.object.process(document)
         self.object.process(other_document)
         assert self.object.metrics.number_of_processed_events == 2
 
-        assert other_document.get("rule_attributions") == document.get("rule_attributions")
+        assert other_document.get("amides") == document.get("amides")
         assert self.object.metrics.total_cmdlines == 2
         assert self.object.metrics.new_results == 1
         assert self.object.metrics.cached_results == 1
         assert self.object.metrics.num_cache_entries == 1
         assert self.object.metrics.cache_load == 0.2
         assert self.object.metrics.mean_misuse_detection_time != 0.0
         assert self.object.metrics.mean_rule_attribution_time != 0.0
@@ -140,15 +147,15 @@
             "winlog": {
                 "event_id": 1,
                 "provider_name": "Microsoft-Windows-Sysmon",
                 "event_data": {"CommandLine": "cmd.exe /c taskkill.exe /im cmd.exe"},
             }
         }
         self.object.process(document)
-        assert document.get("rule_attributions")
+        assert document.get("amides")
         with caplog.at_level(logging.WARNING):
             self.object.process(document)
         assert re.match(".*FieldExistsWarning.*", caplog.text)
 
     def test_setup_get_model_via_file_getter(self, tmp_path, monkeypatch):
         model_uri = "file://tests/testdata/unit/amides/model.zip"
         model_original = Path(self.CONFIG["models_path"])
```

### Comparing `logprep-6.5.1/tests/unit/processor/amides/test_amides_rule.py` & `logprep-6.6.0/tests/unit/processor/amides/test_amides_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # pylint: disable=protected-access
 # pylint: disable=line-too-long
 # pylint: disable=missing-docstring
 import pytest
 
-
 from logprep.processor.amides.rule import AmidesRule
 
 
 @pytest.fixture(name="default_rule_definition")
 def fixture_default_rule_definition():
     return {
         "filter": "winlog.event_id: 1 AND winlog.provider_name: Microsoft-Windows-Sysmon",
         "amides": {
             "source_fields": ["process.command_line"],
-            "target_field": "rule_attributions",
+            "target_field": "amides",
         },
         "description": "Description for Amides",
     }
 
 
 class TestAmidesRule:
     @pytest.mark.parametrize(
@@ -25,39 +24,39 @@
         [
             (
                 "Should equal as they are the same",
                 {
                     "filter": "winlog.event_id: 1 AND winlog.provider_name: Microsoft-Windows-Sysmon",
                     "amides": {
                         "source_fields": ["process.command_line"],
-                        "target_field": "rule_attributions",
+                        "target_field": "amides",
                     },
                     "description": "Description for Amides",
                 },
                 True,
             ),
             (
                 "Should not equal due to different filter values",
                 {
                     "filter": "winlog.event_id: 12",
                     "amides": {
                         "source_fields": ["process.command_line"],
-                        "target_field": "rule_attributions",
+                        "target_field": "amides",
                     },
                     "description": "Description for Amides",
                 },
                 False,
             ),
             (
                 "Should not equal due to different source fields",
                 {
                     "filter": "winlog.event_id: 1 AND winlog.provider_name: Microsoft-Windows-Sysmon",
                     "amides": {
                         "source_fields": ["winlog.event_data.CommandLine"],
-                        "target_field": "rule_attributions",
+                        "target_field": "amides",
                     },
                     "description": "Description for Amides",
                 },
                 False,
             ),
             (
                 "Should not equal because of different target fields",
```

### Comparing `logprep-6.5.1/tests/unit/processor/amides/test_detection.py` & `logprep-6.6.0/tests/unit/processor/amides/test_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=missing-docstring
-import pytest
 import numpy as np
-
+import pytest
 from sklearn.preprocessing import MinMaxScaler
+
 from logprep.processor.amides.detection import (
     MissingModelComponentError,
     MisuseDetector,
     RuleAttributor,
     RuleAttributorError,
 )
 
@@ -47,15 +47,15 @@
 
 
 @pytest.fixture(name="misuse_model")
 def fixture_misuse_model():
     return {
         "clf": MockClassifier(malicious_predict=0.8),
         "vectorizer": MockVectorizer(),
-        "scaler": MockScaler(minimum=-0.5, maximum=0.5),
+        "scaler": MockScaler(minimum=-0.5, maximum=0.8),
     }
 
 
 class TestMisuseDetector:
     def test_init(self, misuse_model):
         assert MisuseDetector(misuse_model, decision_threshold=0.5)
 
@@ -75,16 +75,16 @@
         del misuse_model["clf"]
 
         with pytest.raises(MissingModelComponentError):
             _ = MisuseDetector(misuse_model, decision_threshold=0.5)
 
     def test_detect(self, misuse_model):
         detector = MisuseDetector(misuse_model, 0.5)
-        assert detector.detect("benign") == 0
-        assert detector.detect("malicious") == 1
+        assert detector.detect("benign") == (False, 0.0)
+        assert detector.detect("malicious") == (True, 1.0)
 
 
 class TestRuleAttributor:
     @pytest.fixture
     def rule_models(self):
         return {
             "rule_a": {
@@ -116,25 +116,29 @@
         with pytest.raises(RuleAttributorError):
             _ = RuleAttributor(
                 rule_models,
                 num_rule_attributions=10,
             )
 
     def test_attribute_malicious_sample_sufficient_number_of_confidence_values(self, rule_models):
-        expected = {"rule_c": 0.9, "rule_a": 0.8}
+        expected = [{"rule": "rule_c", "confidence": 0.9}, {"rule": "rule_a", "confidence": 0.8}]
         attributor = RuleAttributor(
             rule_models,
             num_rule_attributions=2,
         )
 
         results = attributor.attribute("malicious")
         assert results == expected
 
     def test_attribute_malicious_sample_too_few_sufficient_confidence_values(self, rule_models):
-        expected = {"rule_c": 0.9, "rule_a": 0.8, "rule_b": 0.7}
+        expected = [
+            {"rule": "rule_c", "confidence": 0.9},
+            {"rule": "rule_a", "confidence": 0.8},
+            {"rule": "rule_b", "confidence": 0.7},
+        ]
 
         attributor = RuleAttributor(
             rule_models,
             num_rule_attributions=4,
         )
 
         results = attributor.attribute("malicious")
```

### Comparing `logprep-6.5.1/tests/unit/processor/amides/test_normalize.py` & `logprep-6.6.0/tests/unit/processor/amides/test_normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/amides/test_tokenizer.py` & `logprep-6.6.0/tests/unit/processor/amides/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/base.py` & `logprep-6.6.0/tests/unit/processor/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.6.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.6.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.6.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.6.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.6.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.6.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=protected-access
 # pylint: disable=missing-docstring
 
 import hashlib
 import logging
+import os
 import re
 import shutil
 import tempfile
 from pathlib import Path
 
 import responses
 
@@ -361,7 +362,27 @@
         logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
         downloaded_file = logprep_tmp_dir / f"{self.object.name}-tldlist-0.dat"
         assert downloaded_file.exists()
         downloaded_checksum = hashlib.md5(downloaded_file.read_bytes()).hexdigest()  # nosemgrep
         assert expected_checksum == downloaded_checksum
         # delete testfile
         shutil.rmtree(logprep_tmp_dir)
+
+    @responses.activate
+    def test_setup_doesnt_overwrite_already_existing_tld_list_file(self):
+        tld_list = "http://db-path-target/list.dat"
+        tld_list_content = "some content"
+        responses.add(responses.GET, tld_list, tld_list_content.encode("utf8"))
+
+        logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
+        os.makedirs(logprep_tmp_dir, exist_ok=True)
+        tld_temp_file = logprep_tmp_dir / f"{self.object.name}-tldlist-0.dat"
+
+        pre_existing_content = "file exists already"
+        tld_temp_file.touch()
+        tld_temp_file.write_bytes(pre_existing_content.encode("utf8"))
+        self.object._config.tld_lists = [tld_list]
+        self.object.setup()
+        assert tld_temp_file.exists()
+        assert tld_temp_file.read_bytes().decode("utf8") == pre_existing_content
+        assert tld_temp_file.read_bytes().decode("utf8") != tld_list_content
+        shutil.rmtree(logprep_tmp_dir)  # delete testfile
```

### Comparing `logprep-6.5.1/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 import hashlib
 import logging
+import os
 import re
 import shutil
 import tempfile
 from copy import deepcopy
 from os.path import exists
 from pathlib import Path
 from unittest import mock
@@ -285,7 +286,27 @@
         logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
         downloaded_file = logprep_tmp_dir / f"{self.object.name}-tldlist-0.dat"
         assert downloaded_file.exists()
         downloaded_checksum = hashlib.md5(downloaded_file.read_bytes()).hexdigest()  # nosemgrep
         assert expected_checksum == downloaded_checksum
         # delete testfile
         shutil.rmtree(logprep_tmp_dir)
+
+    @responses.activate
+    def test_setup_doesnt_overwrite_already_existing_tld_list_file(self):
+        tld_list = "http://db-path-target/list.dat"
+        tld_list_content = "some content"
+        responses.add(responses.GET, tld_list, tld_list_content.encode("utf8"))
+
+        logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
+        os.makedirs(logprep_tmp_dir, exist_ok=True)
+        tld_temp_file = logprep_tmp_dir / f"{self.object.name}-tldlist-0.dat"
+
+        pre_existing_content = "file exists already"
+        tld_temp_file.touch()
+        tld_temp_file.write_bytes(pre_existing_content.encode("utf8"))
+        self.object._config.tld_lists = [tld_list]
+        self.object.setup()
+        assert tld_temp_file.exists()
+        assert tld_temp_file.read_bytes().decode("utf8") == pre_existing_content
+        assert tld_temp_file.read_bytes().decode("utf8") != tld_list_content
+        shutil.rmtree(logprep_tmp_dir)  # delete testfile
```

### Comparing `logprep-6.5.1/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.6.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.6.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=missing-docstring
 # pylint: disable=no-member
 # pylint: disable=protected-access
 # pylint: disable=too-many-statements
 import hashlib
 import logging
+import os
 import re
 import shutil
 import tempfile
 from pathlib import Path
 from unittest import mock
 
 import pytest
@@ -381,7 +382,27 @@
         logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
         downloaded_file = logprep_tmp_dir / f"{self.object.name}.mmdb"
         assert downloaded_file.exists()
         downloaded_checksum = hashlib.md5(downloaded_file.read_bytes()).hexdigest()  # nosemgrep
         assert expected_checksum == downloaded_checksum
         # delete testfile
         shutil.rmtree(logprep_tmp_dir)
+
+    @responses.activate
+    def test_setup_doesnt_overwrite_already_existing_geomap_file(self):
+        tld_list = "http://db-path-target/db_file.mmdb"
+        tld_list_content = "some content"
+        responses.add(responses.GET, tld_list, tld_list_content.encode("utf8"))
+
+        logprep_tmp_dir = Path(tempfile.gettempdir()) / "logprep"
+        os.makedirs(logprep_tmp_dir, exist_ok=True)
+        tld_temp_file = logprep_tmp_dir / f"{self.object.name}.mmdb"
+
+        pre_existing_content = "file exists already"
+        tld_temp_file.touch()
+        tld_temp_file.write_bytes(pre_existing_content.encode("utf8"))
+        self.object._config.tld_lists = [tld_list]
+        self.object.setup()
+        assert tld_temp_file.exists()
+        assert tld_temp_file.read_bytes().decode("utf8") == pre_existing_content
+        assert tld_temp_file.read_bytes().decode("utf8") != tld_list_content
+        shutil.rmtree(logprep_tmp_dir)  # delete testfile
```

### Comparing `logprep-6.5.1/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/grokker/test_grok.py` & `logprep-6.6.0/tests/unit/processor/grokker/test_grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/grokker/test_grokker.py` & `logprep-6.6.0/tests/unit/processor/grokker/test_grokker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/grokker/test_grokker_rule.py` & `logprep-6.6.0/tests/unit/processor/grokker/test_grokker_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.6.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.6.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.6.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/normalizer/test_normalizer_rule.py` & `logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.6.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,16 +26,15 @@
                 {
                     "id": "RULE_ONE_ID",
                     "title": "RULE_ONE",
                     "severity": "critical",
                     "mitre": ["attack.test1", "attack.test2"],
                     "case_condition": "directly",
                     "description": "Test rule one",
-                    "rule_filter": 'AND(winlog.event_id:"123", winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
-                    "lucene_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
+                    "rule_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -54,16 +53,15 @@
                     "id": "RULE_ONE_ID",
                     "title": "RULE_ONE",
                     "severity": "critical",
                     "mitre": ["attack.test1", "attack.test2"],
                     "case_condition": "directly",
                     "host": {"name": "Test hostname"},
                     "description": "Test rule one",
-                    "rule_filter": 'AND(winlog.event_id:"123", winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
-                    "lucene_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
+                    "rule_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -78,16 +76,15 @@
                 {
                     "id": "RULE_ONE_ID",
                     "title": "RULE_ONE",
                     "severity": "critical",
                     "mitre": ["attack.test1", "attack.test2"],
                     "case_condition": "directly",
                     "description": "Test rule one",
-                    "rule_filter": 'AND(winlog.event_id:"123", winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
-                    "lucene_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
+                    "rule_filter": '(winlog.event_id:"123" AND winlog.event_data.ServiceName:"VERY BAD")',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
 
         document["pre_detection_id"] = "11fdfc1f-8e00-476e-b88f-753d92af989c"
         detection_results = self.object.process(document)
@@ -104,19 +101,15 @@
                 {
                     "id": "RULE_TWO_ID",
                     "title": "RULE_TWO",
                     "severity": "critical",
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule two",
-                    "rule_filter": 'AND(tags:"test", '
-                    'process.program:"test", '
-                    'OR(message:"test1*xyz", '
-                    'message:"test2*xyz"))',
-                    "lucene_filter": '(tags:"test" AND process.program:"test" AND '
+                    "rule_filter": '(tags:"test" AND process.program:"test" AND '
                     '(message:"test1*xyz" OR message:"test2*xyz"))',
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
@@ -132,19 +125,15 @@
                 {
                     "id": "RULE_THREE_ID",
                     "title": "RULE_THREE",
                     "severity": "critical",
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule three",
-                    "rule_filter": 'AND(tags:"test2", '
-                    'process.program:"test", '
-                    'OR(message:"test1*xyz", '
-                    'message:"test2?xyz"))',
-                    "lucene_filter": '(tags:"test2" AND process.program:"test" AND '
+                    "rule_filter": '(tags:"test2" AND process.program:"test" AND '
                     '(message:"test1*xyz" OR message:"test2?xyz"))',
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
@@ -158,26 +147,24 @@
         expected_detection_results = (
             [
                 {
                     "case_condition": "directly",
                     "id": "RULE_ONE_ID",
                     "mitre": ["attack.test1", "attack.test2"],
                     "description": "Test two rules one",
-                    "rule_filter": '"first_match"',
-                    "lucene_filter": '"first_match": *',
+                    "rule_filter": '"first_match": *',
                     "severity": "critical",
                     "title": "RULE_ONE",
                 },
                 {
                     "case_condition": "directly",
                     "id": "RULE_TWO_ID",
                     "mitre": ["attack.test2", "attack.test4"],
                     "description": "Test two rules two",
-                    "rule_filter": '"second_match"',
-                    "lucene_filter": '"second_match": *',
+                    "rule_filter": '"second_match": *',
                     "severity": "suspicious",
                     "title": "RULE_TWO",
                 },
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
@@ -260,16 +247,15 @@
                 {
                     "id": "RULE_TWO_ID",
                     "title": "RULE_TWO",
                     "severity": "critical",
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule two",
-                    "rule_filter": 'AND(tags:"test", process.program:"test", OR(message:"test1*xyz", message:"test2*xyz"))',  # pylint: disable=line-too-long
-                    "lucene_filter": '(tags:"test" AND process.program:"test" AND (message:"test1*xyz" OR message:"test2*xyz"))',  # pylint: disable=line-too-long
+                    "rule_filter": '(tags:"test" AND process.program:"test" AND (message:"test1*xyz" OR message:"test2*xyz"))',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
@@ -284,16 +270,15 @@
                 {
                     "id": "RULE_TWO_ID",
                     "title": "RULE_TWO",
                     "severity": "critical",
                     "mitre": [],
                     "case_condition": "directly",
                     "description": "Test rule two",
-                    "rule_filter": 'AND(tags:"test", process.program:"test", OR(message:"test1*xyz", message:"test2*xyz"))',  # pylint: disable=line-too-long
-                    "lucene_filter": '(tags:"test" AND process.program:"test" AND (message:"test1*xyz" OR message:"test2*xyz"))',  # pylint: disable=line-too-long
+                    "rule_filter": '(tags:"test" AND process.program:"test" AND (message:"test1*xyz" OR message:"test2*xyz"))',  # pylint: disable=line-too-long
                 }
             ],
             ({"kafka": "pre_detector_alerts"},),
         )
         detection_results = self.object.process(document)
         self._assert_equality_of_results(
             document, expected, detection_results, expected_detection_results
```

### Comparing `logprep-6.5.1/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.6.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/requester/test_requester.py` & `logprep-6.6.0/tests/unit/processor/requester/test_requester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.6.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.6.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/test_processor_rule.py` & `logprep-6.6.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/test_processor_strategy.py` & `logprep-6.6.0/tests/unit/processor/test_processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/timestamper/test_timestamper.py` & `logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/processor/timestamper/test_timestamper_rule.py` & `logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/test_configuration.py` & `logprep-6.6.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/test_factory.py` & `logprep-6.6.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/test_run_logprep.py` & `logprep-6.6.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/test_runner.py` & `logprep-6.6.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.6.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.6.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_cache.py` & `logprep-6.6.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_configuration.py` & `logprep-6.6.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_getter.py` & `logprep-6.6.0/tests/unit/util/test_getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_helper.py` & `logprep-6.6.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_helper_add_field.py` & `logprep-6.6.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_log_aggregator.py` & `logprep-6.6.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_processor_generator.py` & `logprep-6.6.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.6.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.6.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,20 @@
               type: pre_detector
               specific_rules:
                 - tests/testdata/unit/pre_detector/rules/specific/
               generic_rules:
                 - tests/testdata/unit/pre_detector/rules/generic/
               outputs:
                 - patched_output: sre_topic
+          - selective_extractor:
+              type: selective_extractor
+              specific_rules:
+                - tests/testdata/unit/selective_extractor/rules/specific/
+              generic_rules:
+                - tests/testdata/unit/selective_extractor/rules/generic/
         """
         self.config_path = os.path.join(tempfile.gettempdir(), "dry-run-config.yml")
         with open(self.config_path, "w", encoding="utf8") as config_file:
             config_file.write(config)
 
     def teardown_method(self):
         os.remove(self.config_path)
@@ -71,14 +77,15 @@
             full_output=True,
             use_json=True,
             logger=logging.getLogger("test-logger"),
         )
         dry_runner.run()
 
         captured = capsys.readouterr()
+        assert captured.err == ""
         assert "------ PROCESSED EVENT ------" in captured.out
         assert "------ TRANSFORMED EVENTS: 1/1 ------" in captured.out
 
     def test_dry_run_accepts_json_in_list_as_input(self, tmp_path, capsys):
         test_json = [{"winlog": {"event_id": 1111, "event_data": {"test2": "fancy data"}}}]
         input_json_file = os.path.join(tmp_path, "test_input.json")
         with open(input_json_file, "w", encoding="utf8") as input_file:
@@ -90,14 +97,15 @@
             full_output=True,
             use_json=True,
             logger=logging.getLogger("test-logger"),
         )
         dry_runner.run()
 
         captured = capsys.readouterr()
+        assert captured.err == ""
         assert "------ PROCESSED EVENT ------" in captured.out
         assert "------ TRANSFORMED EVENTS: 1/1 ------" in captured.out
 
     def test_dry_run_accepts_jsonl_as_input(self, tmp_path, capsys):
         test_jsonl = [
             '{"winlog": {"event_id": 1111, "event_data": {"test2": "fancy data"}}}\n',
             '{"winlog": {"event_id": 1111, "event_data": {"test2": "more fancy data"}}}',
@@ -112,25 +120,28 @@
             full_output=True,
             use_json=False,
             logger=logging.getLogger("test-logger"),
         )
         dry_runner.run()
 
         captured = capsys.readouterr()
+        assert captured.err == ""
         assert "------ PROCESSED EVENT ------" in captured.out
         assert captured.out.count("------ PROCESSED EVENT ------") == 2
         assert "------ TRANSFORMED EVENTS: 2/2 ------" in captured.out
 
     def test_dry_run_print_custom_output(self, tmp_path, capsys):
         test_json = {
             "winlog": {
                 "event_id": 1234,
                 "provider_name": "Test456",
                 "event_data": {"param1": "username"},
-            }
+            },
+            "message": "some message",
+            "field1": "field for the selective extractor",
         }
         input_json_file = os.path.join(tmp_path, "test_input.json")
         with open(input_json_file, "w", encoding="utf8") as input_file:
             json.dump(test_json, input_file)
 
         dry_runner = DryRunner(
             input_file_path=input_json_file,
@@ -138,14 +149,15 @@
             full_output=True,
             use_json=True,
             logger=logging.getLogger("test-logger"),
         )
         dry_runner.run()
 
         captured = capsys.readouterr()
+        assert captured.err == ""
         assert "------ PROCESSED EVENT ------" in captured.out
         assert "------ TRANSFORMED EVENTS: 1/1 ------" in captured.out
         assert "------ CUSTOM OUTPUTS ------" in captured.out
 
     def test_dry_run_prints_predetection(self, tmp_path, capsys):
         test_json = {
             "winlog": {
@@ -163,10 +175,11 @@
             full_output=True,
             use_json=True,
             logger=logging.getLogger("test-logger"),
         )
         dry_runner.run()
 
         captured = capsys.readouterr()
+        assert captured.err == ""
         assert "------ PROCESSED EVENT ------" in captured.out
         assert "------ TRANSFORMED EVENTS: 1/1 ------" in captured.out
         assert "------ CUSTOM OUTPUTS ------" in captured.out
```

### Comparing `logprep-6.5.1/tests/unit/util/test_time.py` & `logprep-6.6.0/tests/unit/util/test_time.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_time_measurement.py` & `logprep-6.6.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/test_validators.py` & `logprep-6.6.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/unit/util/tests_json_handling.py` & `logprep-6.6.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/tests/util/testhelpers.py` & `logprep-6.6.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.5.1/versioneer.py` & `logprep-6.6.0/versioneer.py`

 * *Files identical despite different names*

