# Comparing `tmp/summa_embed-0.17.5.tar.gz` & `tmp/summa_embed-0.17.6.tar.gz`

## Comparing `summa_embed-0.17.5.tar` & `summa_embed-0.17.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.5/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2381 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10598 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7789 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2523 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      394 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.5/local_dependencies/summa-server/Cargo.toml
--rw-r--r--   0      501       20       43 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/.cargo/config.toml
--rw-r--r--   0      501       20     1050 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/LICENSE
--rw-r--r--   0      501       20     2832 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/consumer.rs
--rw-r--r--   0      501       20    13268 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/index.rs
--rw-r--r--   0      501       20      105 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/mod.rs
--rw-r--r--   0      501       20     2909 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/reflection.rs
--rw-r--r--   0      501       20     1278 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/apis/search.rs
--rw-r--r--   0      501       20      783 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/bin/main.rs
--rw-r--r--   0      501       20     5305 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumer_manager.rs
--rw-r--r--   0      501       20      813 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
--rw-r--r--   0      501       20     1082 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/dummy.rs
--rw-r--r--   0      501       20    11633 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
--rw-r--r--   0      501       20      270 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
--rw-r--r--   0      501       20      532 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
--rw-r--r--   0      501       20      155 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/mod.rs
--rw-r--r--   0      501       20     3811 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/index_meter.rs
--rw-r--r--   0      501       20      258 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/components/mod.rs
--rw-r--r--   0      501       20      943 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/api.rs
--rw-r--r--   0      501       20      919 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/consumer.rs
--rw-r--r--   0      501       20      434 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/metrics.rs
--rw-r--r--   0      501       20      116 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/mod.rs
--rw-r--r--   0      501       20     4268 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/server.rs
--rw-r--r--   0      501       20      991 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/configs/store.rs
--rw-r--r--   0      501       20     3459 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/errors.rs
--rw-r--r--   0      501       20     1427 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/lib.rs
--rw-r--r--   0      501       20     3681 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/logging.rs
--rw-r--r--   0      501       20    15704 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/server.rs
--rw-r--r--   0      501       20     8110 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/api.rs
--rw-r--r--   0      501       20    40154 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/index.rs
--rw-r--r--   0      501       20     5174 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/metrics.rs
--rw-r--r--   0      501       20      287 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/services/mod.rs
--rw-r--r--   0      501       20     2108 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/utils/mod.rs
--rw-r--r--   0      501       20      923 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-server/src/utils/thread_handler.rs
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.5/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20   370551 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/dictionaries/drugs.csv
--rw-r--r--   0      501       20       92 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7233 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5492 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20    13820 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    31266 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13903 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    20309 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5962 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     6539 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      250 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20     1193 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
--rw-r--r--   0      501       20      693 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
--rw-r--r--   0      501       20     2092 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
--rw-r--r--   0      501       20    13740 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1899 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    67578 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     5812 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
--rw-r--r--   0      501       20     2498 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/utils.rs
--rw-r--r--   0      501       20     2216 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11998 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7462 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     4680 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8015 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5474 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      559 2023-06-27 09:46:43.000000 summa_embed-0.17.5/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.5/Cargo.toml
--rw-r--r--   0      501       20      685 2023-06-27 09:46:43.000000 summa_embed-0.17.5/.gitignore
--rw-r--r--   0      501       20      400 2023-06-27 09:46:43.000000 summa_embed-0.17.5/pyproject.toml
--rw-r--r--   0      501       20     2199 2023-06-27 09:46:43.000000 summa_embed-0.17.5/src/lib.rs
--rw-r--r--   0      501       20   102250 2023-06-27 09:47:05.000000 summa_embed-0.17.5/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.5/PKG-INFO
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 summa_embed-0.17.6/local_dependencies/summa-server/Cargo.toml
+-rw-r--r--   0      501       20       43 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/.cargo/config.toml
+-rw-r--r--   0      501       20     1050 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/LICENSE
+-rw-r--r--   0      501       20     2832 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/consumer.rs
+-rw-r--r--   0      501       20    13268 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/index.rs
+-rw-r--r--   0      501       20      105 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/mod.rs
+-rw-r--r--   0      501       20     2909 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/reflection.rs
+-rw-r--r--   0      501       20     1278 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/apis/search.rs
+-rw-r--r--   0      501       20      783 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/bin/main.rs
+-rw-r--r--   0      501       20     5305 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumer_manager.rs
+-rw-r--r--   0      501       20      813 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs
+-rw-r--r--   0      501       20     1082 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/dummy.rs
+-rw-r--r--   0      501       20    11633 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs
+-rw-r--r--   0      501       20      270 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/mod.rs
+-rw-r--r--   0      501       20      532 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/status.rs
+-rw-r--r--   0      501       20      155 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/mod.rs
+-rw-r--r--   0      501       20     3811 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/index_meter.rs
+-rw-r--r--   0      501       20      258 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/components/mod.rs
+-rw-r--r--   0      501       20      943 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/api.rs
+-rw-r--r--   0      501       20      919 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/consumer.rs
+-rw-r--r--   0      501       20      434 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/metrics.rs
+-rw-r--r--   0      501       20      116 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/mod.rs
+-rw-r--r--   0      501       20     4268 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/server.rs
+-rw-r--r--   0      501       20      991 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/configs/store.rs
+-rw-r--r--   0      501       20     3459 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/errors.rs
+-rw-r--r--   0      501       20     1427 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/lib.rs
+-rw-r--r--   0      501       20     3681 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/logging.rs
+-rw-r--r--   0      501       20    15704 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/server.rs
+-rw-r--r--   0      501       20     8110 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/api.rs
+-rw-r--r--   0      501       20    40154 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/index.rs
+-rw-r--r--   0      501       20     5174 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/metrics.rs
+-rw-r--r--   0      501       20      287 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/services/mod.rs
+-rw-r--r--   0      501       20     2108 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/utils/mod.rs
+-rw-r--r--   0      501       20      923 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-server/src/utils/thread_handler.rs
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 summa_embed-0.17.6/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20   370551 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/dictionaries/drugs.csv
+-rw-r--r--   0      501       20       92 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7233 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5492 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20    13820 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    31266 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13903 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    20309 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5962 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     6539 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      250 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20     1193 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs
+-rw-r--r--   0      501       20      693 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs
+-rw-r--r--   0      501       20     2092 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs
+-rw-r--r--   0      501       20    13740 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1899 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    63781 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     5812 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2498 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/utils.rs
+-rw-r--r--   0      501       20     2216 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11998 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7462 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     4526 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8015 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      559 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.17.6/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2381 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10598 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7741 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-07-03 15:18:18.000000 summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 summa_embed-0.17.6/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-07-03 15:18:18.000000 summa_embed-0.17.6/.gitignore
+-rw-r--r--   0      501       20      400 2023-07-03 15:18:18.000000 summa_embed-0.17.6/pyproject.toml
+-rw-r--r--   0      501       20     2199 2023-07-03 15:18:18.000000 summa_embed-0.17.6/src/lib.rs
+-rw-r--r--   0      501       20   101640 2023-07-03 15:18:31.000000 summa_embed-0.17.6/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.17.6/PKG-INFO
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.17.6/local_dependencies/summa-proto/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-proto"
-version = "0.29.0"
+version = "0.29.1"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa search server proto files"
 
 [lib]
 name = "summa_proto"
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.17.6/local_dependencies/summa-server/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/build.rs` & `summa_embed-0.17.6/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.17.6/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.17.6/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.17.6/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.17.6/local_dependencies/summa-proto/proto/query.proto`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     MatchQueryBooleanShouldMode boolean_should_mode = 6;
     MatchQueryDisjuctionMaxMode disjuction_max_mode = 7;
   }
   ExactMatchesPromoter exact_matches_promoter = 8;
   repeated string removed_fields = 9;
   map<string, MorphologyConfig> morphology_configs = 10;
   optional string query_language = 11;
-  NerMatchesPromoter ner_matches_promoter = 12;
 }
 
 message SearchResponse {
   // Time spent inside of `search` handler
   double elapsed_secs = 1;
   // An array of collector outputs
   repeated CollectorOutput collector_outputs = 2;
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.17.6/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.17.6/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.17.6/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/Cargo.toml` & `summa_embed-0.17.6/local_dependencies/summa-server/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "summa-server"
-version = "0.17.5"
+version = "0.17.6"
 license-file = "LICENSE"
 description = "Fast full-text search server"
 homepage = "https://github.com/izihawa/summa"
 repository = "https://github.com/izihawa/summa"
 keywords = ["async", "search", "server", "grpc"]
 
 [lib]
@@ -51,15 +51,15 @@
 rand = { version = "0.8", features = ["small_rng"] }
 rdkafka = { version = "0.29", optional = true }
 rlimit = "0.9"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_derive = "1.0"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
-summa-core = { version = "0.17.5", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.17.6", path = "../summa-core", features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { features = ["grpc"] , path = "../summa-proto" }
 take_mut = "0.2"
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tantivy-fst = "0.4.0"
 time = { version = "0.3", features = ["serde-well-known", "wasm-bindgen"] }
 thiserror = "1.0"
 tokio = { version = "1.25", default_features = false , features = ["full", "time"] }
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/LICENSE` & `summa_embed-0.17.6/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/consumer.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/index.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/reflection.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/reflection.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/apis/search.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/apis/search.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/bin/main.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumer_manager.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumer_manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/consumer_thread.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/dummy.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/dummy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/components/consumers/kafka/status.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/components/consumers/kafka/status.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/components/index_meter.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/components/index_meter.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/api.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/consumer.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/consumer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/server.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/configs/store.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/configs/store.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/errors.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/lib.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/logging.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/logging.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/server.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/server.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/services/api.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/services/api.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/services/index.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/services/index.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/services/metrics.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/services/metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/utils/mod.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-server/src/utils/thread_handler.rs` & `summa_embed-0.17.6/local_dependencies/summa-server/src/utils/thread_handler.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.17.6/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.17.5"
+version = "0.17.6"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/LICENSE` & `summa_embed-0.17.6/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/dictionaries/drugs.csv` & `summa_embed-0.17.6/local_dependencies/summa-core/dictionaries/drugs.csv`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/english.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/manager.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/morphology/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 2% similar despite different names*

```diff
@@ -690,53 +690,14 @@
 
         for pair in pairs.clone() {
             let parsed_queries = self.parse_statement(pair)?;
             subqueries.push((Occur::Should, parsed_queries));
         }
 
         if let Some(top_level_phrase) = self.extract_top_level_phrase(pairs) {
-            if let Some(ner_matches_promoter) = &self.query_parser_config.0.ner_matches_promoter {
-                if let Some(morphology) = self.morphology_manager.get(self.query_parser_config.0.query_language()) {
-                    let fields = if ner_matches_promoter.fields.is_empty() {
-                        self.query_parser_config.0.default_fields.iter()
-                    } else {
-                        ner_matches_promoter.fields.iter()
-                    };
-                    let entities = morphology.detect_ners(&top_level_phrase);
-                    subqueries.extend(
-                        fields
-                            .map(|field| {
-                                let mut subsubqueries = vec![];
-                                for entity in &entities {
-                                    let (field, full_path) = self.schema.find_field(self.resolve_field_name(field)).expect("no field");
-                                    let field_entry = self.schema.get_field_entry(field);
-                                    let field_boost = self.query_parser_config.0.field_boosts.get(field_entry.name()).copied();
-                                    if let FieldType::Str(ref str_option) = field_entry.field_type() {
-                                        let Some(option) = str_option.get_indexing_options() else {
-                                        continue
-                                    };
-                                        let terms = match self.parse_words(field, full_path, option, entity) {
-                                            Ok(terms) => terms,
-                                            Err(err) => return Err(err),
-                                        };
-                                        if terms.len() > 1 && option.index_option().has_positions() {
-                                            let query = Box::new(PhraseQuery::new_with_offset(terms)) as Box<dyn Query>;
-                                            subsubqueries.push(boost_query(query, multiply_boosts(ner_matches_promoter.boost, field_boost)))
-                                        }
-                                    }
-                                }
-                                Ok(subsubqueries)
-                            })
-                            .collect::<Result<Vec<Vec<_>>, _>>()?
-                            .into_iter()
-                            .flatten()
-                            .map(|q| (Occur::Should, q)),
-                    )
-                }
-            }
             if let Some(exact_matches_promoter) = &self.query_parser_config.0.exact_matches_promoter {
                 let fields = if exact_matches_promoter.fields.is_empty() {
                     self.query_parser_config.0.default_fields.iter()
                 } else {
                     exact_matches_promoter.fields.iter()
                 };
                 subqueries.extend(
@@ -1187,28 +1148,8 @@
         query_parser.query_parser_config.0.morphology_configs = morphology_configs;
         query_parser.query_parser_config.0.query_language = Some("en".to_string());
         let query = query_parser.parse_query("red1 search engine going");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"red1\"))), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.3 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.3 }), (Should, TermQuery(Term(field=0, type=Str, \"going\")))] })");
         let query = query_parser.parse_query("iso 34-1:2022");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"iso\")), TermQuery(Term(field=0, type=Str, \"isos\"))], tie_breaker: 0.3 }), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"1\")))] })");
     }
-
-    #[test]
-    pub fn test_ner() {
-        let mut query_parser = create_query_parser();
-        let mut morphology_configs = HashMap::new();
-        morphology_configs.insert(
-            "en".to_string(),
-            proto::MorphologyConfig {
-                derive_tenses_coefficient: Some(0.3),
-            },
-        );
-        query_parser.query_parser_config.0.morphology_configs = morphology_configs;
-        query_parser.query_parser_config.0.ner_matches_promoter = Some(proto::NerMatchesPromoter {
-            boost: Some(1.3),
-            fields: vec!["title".to_string()],
-        });
-        query_parser.query_parser_config.0.query_language = Some("en".to_string());
-        let query = query_parser.parse_query("london is the capital of Great Britain");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"london\"))), (Should, TermQuery(Term(field=0, type=Str, \"is\"))), (Should, TermQuery(Term(field=0, type=Str, \"the\"))), (Should, TermQuery(Term(field=0, type=Str, \"capital\"))), (Should, TermQuery(Term(field=0, type=Str, \"of\"))), (Should, TermQuery(Term(field=0, type=Str, \"great\"))), (Should, TermQuery(Term(field=0, type=Str, \"britain\")))] })");
-    }
 }
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/query_parser/utils.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/query_parser/utils.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,14 @@
         self.0.morphology_configs.extend(other.0.morphology_configs);
         if other.0.term_limit > 0 {
             self.0.term_limit = other.0.term_limit;
         }
         if let Some(exact_matches_promoter) = other.0.exact_matches_promoter {
             self.0.exact_matches_promoter = Some(exact_matches_promoter)
         }
-        if let Some(ner_matches_promoter) = other.0.ner_matches_promoter {
-            self.0.ner_matches_promoter = Some(ner_matches_promoter)
-        }
         if let Some(default_mode) = other.0.default_mode {
             self.0.default_mode = Some(default_mode)
         }
         if let Some(query_language) = other.0.query_language {
             self.0.query_language = Some(query_language)
         }
     }
```

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/local_dependencies/summa-core/src/validators.rs` & `summa_embed-0.17.6/local_dependencies/summa-core/src/validators.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/Cargo.toml` & `summa_embed-0.17.6/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-embed-py"
-version = "0.17.5"
+version = "0.17.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
@@ -13,12 +13,12 @@
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pyo3-log = "0.8"
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.17.5", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
-summa-server = { version = "0.17.5", path = "local_dependencies/summa-server", default_features = false }
+summa-core = { version = "0.17.6", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-server = { version = "0.17.6", path = "local_dependencies/summa-server", default_features = false }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.17.5/.gitignore` & `summa_embed-0.17.6/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/src/lib.rs` & `summa_embed-0.17.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.17.5/Cargo.lock` & `summa_embed-0.17.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
@@ -86,25 +95,25 @@
 
 [[package]]
 name = "anstyle-query"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "anstyle-wincon"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
@@ -135,21 +144,21 @@
 dependencies = [
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "7b2d0f03b3640e3a630367e40c468cb7f309529c708ed1d88597047b0e7c6ef7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -196,14 +205,29 @@
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base-x"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4cbbc9d0964165b47557570cce6c952866c2678457aca742aafc9fb771d30270"
 
 [[package]]
 name = "base64"
@@ -381,30 +405,29 @@
  "multihash 0.18.1",
  "serde",
  "unsigned-varint",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.8"
+version = "4.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9394150f5b4273a1763355bd1c2ec54cc5a2593f790587bcd6b2c947cfa9211"
+checksum = "384e169cc618c613d5e3ca6404dda77a8685a63e08660dcc64abaf7da7cb0c7a"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.8"
+version = "4.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a78fbdd3cc2914ddf37ba444114bc7765bbdcb55ec9cbe6fa054f0137400717"
+checksum = "ef137bbe35aab78bdb468ccfba75a5f4d8321ae011d34063770780545176af2d"
 dependencies = [
  "anstream",
  "anstyle",
- "bitflags 1.3.2",
  "clap_lex",
  "once_cell",
  "strsim",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -701,15 +724,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -777,15 +800,15 @@
 version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.2.16",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
@@ -849,20 +872,20 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "fs4"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7672706608ecb74ab2e055c68327ffc25ae4cac1e12349204fd5fb0f3487cce2"
+checksum = "2eeb4ed9e12f43b7fa0baae3f9cdda28352770132ef2e09a23760c29cae8bd47"
 dependencies = [
- "rustix",
- "windows-sys 0.48.0",
+ "rustix 0.38.2",
+ "windows-sys",
 ]
 
 [[package]]
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
@@ -925,15 +948,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1004,14 +1027,20 @@
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "h2"
 version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
@@ -1079,23 +1108,14 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "htmlescape"
 version = "0.3.1"
@@ -1250,17 +1270,17 @@
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "ipfs-hamt-directory"
 version = "0.1.1"
 dependencies = [
  "anyhow",
@@ -1288,38 +1308,37 @@
  "ipfs-hamt-directory",
  "multihash 0.18.1",
  "pyo3",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
- "windows-sys 0.48.0",
+ "hermit-abi",
+ "rustix 0.38.2",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "c0aa48fab2893d8a49caa94082ae8488f4e1050d73b367881dcd2198f4199fd8"
 
 [[package]]
 name = "izihawa-fst"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12ab646c8dd0c6ea3f36c02d4bd61773536509d822445aecf9c88362558c2244"
 dependencies = [
@@ -1493,14 +1512,20 @@
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -1530,17 +1555,17 @@
  "scoped-tls",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "lru"
-version = "0.10.0"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03f1160296536f10c833a82dca22267d5486734230d47bf00bf435885814ba1e"
+checksum = "718e8fae447df0c7e1ba7f5189829e63fd536945c8988d61444c19039f16b670"
 dependencies = [
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "matchers"
 version = "0.1.0"
@@ -1650,15 +1675,15 @@
 name = "mio"
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "multibase"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b3539ec3c1f04ac9748a260728e855f261b4977f5c3406612c884564f329404"
@@ -1773,19 +1798,19 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "num_enum"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1803,14 +1828,23 @@
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oneshot"
@@ -1840,15 +1874,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -2062,15 +2096,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3e8cba4ec22bada7fc55ffe51e2deb6a0e0db2d0b7ab0b103acc80d2510c190"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "pest_meta"
 version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a01f71cb40bd8bb94232df14b946909e14660e33fc05db3e50ae2a82d7ea0ca0"
@@ -2088,37 +2122,37 @@
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -2437,17 +2471,17 @@
 checksum = "9d6da84cc204722a989e01ba2f6e1e276e190f22263d0cb6ce8526fcdb0d2e1f"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -2682,31 +2716,50 @@
  "filetime",
  "libipld",
  "quick-protobuf",
  "sha2",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "8818fa822adcc98b18fedbb3632a6a33213c070556b5aa7c4c8cc21cff565c4c"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys",
- "windows-sys 0.48.0",
+ "linux-raw-sys 0.3.8",
+ "windows-sys",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys 0.4.3",
+ "windows-sys",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
@@ -2715,19 +2768,19 @@
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "scoped-tls"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1cf6437eb19a8f4a6cc0f7dca544973b0b78843adbfeb3683d1a94a0024a294"
@@ -2759,17 +2812,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.165"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "c939f902bb7d0ccc5bce4f03297e161543c2dcb30914faf032c2bd0b7a0d48fc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.5.0"
@@ -2798,21 +2851,21 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.165"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "6eaae920e25fffe4019b75ff65e7660e72091e59dd204cb5849bbd6a3fd343d7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
@@ -2960,15 +3013,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.17.5"
+version = "0.17.6"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "chrono",
  "config",
@@ -3008,15 +3061,15 @@
  "time 0.3.22",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.17.5"
+version = "0.17.6"
 dependencies = [
  "async-broadcast",
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -3027,30 +3080,30 @@
  "summa-server",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
-version = "0.29.0"
+version = "0.29.1"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
  "tokio",
  "tonic",
  "tonic-build",
  "tonic-reflection",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.17.5"
+version = "0.17.6"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3133,17 +3186,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.22"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3338,16 +3391,16 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
  "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
- "rustix",
- "windows-sys 0.48.0",
+ "rustix 0.37.22",
+ "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
@@ -3359,15 +3412,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -3433,29 +3486,30 @@
 checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "tokio-io-timeout"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30b74022ada614a1b4834de765f9bb43877f910cc8ce4be40e89042c9223a8bf"
@@ -3468,15 +3522,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3674,15 +3728,15 @@
 name = "tracing-attributes"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -3897,15 +3951,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3931,15 +3985,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -3996,131 +4050,74 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
```

