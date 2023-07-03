# Comparing `tmp/propan-0.1.4.6.tar.gz` & `tmp/propan-0.1.5.0.tar.gz`

## Comparing `propan-0.1.4.6.tar` & `propan-0.1.5.0.tar`

### file list

```diff
@@ -1,188 +1,190 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.6/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/__about__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/__main__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/_compat.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/py.typed
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/constants.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    19850 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/logging.py
--rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/__init__.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/app.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/nats.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/sqs.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/publish.sh
--rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.6/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.6/LICENSE
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 propan-0.1.4.6/README.md
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.4.6/pyproject.toml
--rw-r--r--   0        0        0    18745 2020-02-02 00:00:00.000000 propan-0.1.4.6/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.0/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.0/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/__about__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/__main__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/_compat.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/py.typed
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/constants.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    19850 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/consts.py
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/nats_js_broker.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/logging.py
+-rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/rabbit/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/__init__.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/kafka.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/nats.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.0/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.0/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.5.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.0/LICENSE
+-rw-r--r--   0        0        0    14822 2020-02-02 00:00:00.000000 propan-0.1.5.0/README.md
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    19171 2020-02-02 00:00:00.000000 propan-0.1.5.0/PKG-INFO
```

### Comparing `propan-0.1.4.6/CONTRIBUTING.md` & `propan-0.1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/SECURITY.md` & `propan-0.1.5.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.5.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.5.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/workflows/documentation.yml` & `propan-0.1.5.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/workflows/publish_coverage.yml` & `propan-0.1.5.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/workflows/publish_pypi.yml` & `propan-0.1.5.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/.github/workflows/tests.yml` & `propan-0.1.5.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
       sqs:
         image: softwaremill/elasticmq-native
         ports:
           - 9324:9324
 
       nats:
-        image: nats
+        image: diementros/nats:js
         ports:
           - 4222:4222
 
       redis:
         image: redis:alpine
         ports:
           - 6379:6379
@@ -87,31 +87,32 @@
           name: coverage
           path: coverage
 
   test-e2e-nats:
     runs-on: ubuntu-latest
     services:
       nats:
-        image: nats
+        image: diementros/nats:js
         ports:
           - 4222:4222
+
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[testsuite,async-nats]
       - run: mkdir coverage
       - name: Test
-        run: coverage run -m pytest -m "run" -k test_run_nats_correct tests/cli/test_run.py
+        run: coverage run -m pytest -m "run and nats" tests/cli/test_run.py
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
         uses: actions/upload-artifact@v3
         with:
           name: coverage
@@ -133,15 +134,15 @@
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[testsuite,async-rabbit]
       - run: mkdir coverage
       - name: Test
-        run: coverage run -m pytest -m "run" -k test_run_rabbit_correct tests/cli/test_run.py
+        run: coverage run -m pytest -m "run and rabbit" tests/cli/test_run.py
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
         uses: actions/upload-artifact@v3
         with:
           name: coverage
@@ -174,15 +175,15 @@
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[testsuite,async-kafka]
       - run: mkdir coverage
       - name: Test
-        run: coverage run -m pytest -m "run" -k test_run_kafka_correct tests/cli/test_run.py
+        run: coverage run -m pytest -m "run and kafka" tests/cli/test_run.py
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
         uses: actions/upload-artifact@v3
         with:
           name: coverage
@@ -204,15 +205,15 @@
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[testsuite,async-sqs]
       - run: mkdir coverage
       - name: Test
-        run: coverage run -m pytest -m "run" -k test_run_sqs_correct tests/cli/test_run.py
+        run: coverage run -m pytest -m "run and sqs" tests/cli/test_run.py
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
         uses: actions/upload-artifact@v3
         with:
           name: coverage
@@ -234,15 +235,15 @@
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[testsuite,async-redis]
       - run: mkdir coverage
       - name: Test
-        run: coverage run -m pytest -m "run" -k test_run_redis_correct tests/cli/test_run.py
+        run: coverage run -m pytest -m "run and redis" tests/cli/test_run.py
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
         uses: actions/upload-artifact@v3
         with:
           name: coverage
```

### Comparing `propan-0.1.4.6/examples/3_lifespan_events.py` & `propan-0.1.5.0/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/4_cli_attributes_promotion.py` & `propan-0.1.5.0/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/5_publishing.py` & `propan-0.1.5.0/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/6_arguments_casting.py` & `propan-0.1.5.0/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/7_handler_errors_processing.py` & `propan-0.1.5.0/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/dependencies/1_dependency_injection.py` & `propan-0.1.5.0/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.5.0/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.5.0/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.5.0/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.5.0/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/dependencies/7_annotated.py` & `propan-0.1.5.0/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/quart.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.5.0/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/rabbit/direct.py` & `propan-0.1.5.0/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/rabbit/fanout.py` & `propan-0.1.5.0/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/rabbit/header.py` & `propan-0.1.5.0/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/rabbit/topic.py` & `propan-0.1.5.0/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/redis/direct.py` & `propan-0.1.5.0/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/redis/pattern.py` & `propan-0.1.5.0/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/examples/serialization/protobuf.py` & `propan-0.1.5.0/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/__about__.py` & `propan-0.1.5.0/propan/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.4.6"
+__version__ = "0.1.5.0"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.4.6/propan/__init__.py` & `propan-0.1.5.0/propan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     from propan.brokers.rabbit import RabbitBroker, RabbitRouter
 except ImportError:
     RabbitBroker = RabbitRouter = about.INSTALL_RABBIT  # type: ignore
 
 try:
-    from propan.brokers.nats import NatsBroker, NatsRouter
+    from propan.brokers.nats import NatsBroker, NatsJSBroker, NatsRouter
 except ImportError:
-    NatsBroker = NatsRouter = about.INSTALL_NATS  # type: ignore
+    NatsJSBroker = NatsBroker = NatsRouter = about.INSTALL_NATS  # type: ignore
 
 try:
     from propan.brokers.redis import RedisBroker, RedisRouter
 except ImportError:
     RedisBroker = RedisRouter = about.INSTALL_REDIS  # type: ignore
 
 try:
@@ -48,14 +48,15 @@
     "Context",
     "ContextRepo",
     "Depends",
     # brokers
     "PropanMessage",
     ## nats
     "NatsBroker",
+    "NatsJSBroker",
     "NatsRouter",
     ## rabbit
     "RabbitBroker",
     "RabbitRouter",
     ## redis
     "RedisBroker",
     "RedisRouter",
```

### Comparing `propan-0.1.4.6/propan/_compat.py` & `propan-0.1.5.0/propan/_compat.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/annotations.py` & `propan-0.1.5.0/propan/annotations.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,22 +26,30 @@
         aio_pika.robust_channel.RobustChannel, ContextField("broker.channel")
     ]
 except ImportError:
     RabbitBroker = RabbitMessage = Channel = about.INSTALL_RABBIT
 
 
 try:
+    from nats.aio.client import Client
     from nats.aio.msg import Msg
+    from nats.js.client import JetStreamContext
 
     from propan.brokers.nats import NatsBroker as NB
+    from propan.brokers.nats import NatsJSBroker as NJB
 
     NatsBroker = Annotated[NB, ContextField("broker")]
+    NatsJSBroker = Annotated[NJB, ContextField("broker")]
     NatsMessage = Annotated[Msg, ContextField("message")]
+    NatsConnection = Annotated[Client, ContextField("broker._connection")]
+    NatsJS = Annotated[JetStreamContext, ContextField("broker._connection")]
 except ImportError:
-    NatsBroker = NatsMessage = about.INSTALL_NATS
+    NatsBroker = (
+        NatsMessage
+    ) = NatsJSBroker = NatsJS = NatsConnection = about.INSTALL_NATS
 
 
 try:
     from redis.asyncio.client import Redis as R
 
     from propan.brokers.redis import RedisBroker as RedB
 
@@ -75,13 +83,13 @@
 except ImportError:
     SQSBroker = client = queue_url = about.INSTALL_SQS
 
 
 assert any(
     (
         all((RabbitBroker, RabbitMessage, Channel)),
-        all((NatsBroker, NatsMessage)),
+        all((NatsBroker, NatsJSBroker, NatsJS, NatsMessage)),
         all((RedisBroker, Redis)),
         all((KafkaBroker, KafkaMessage, Producer)),
         all((SQSBroker, client, queue_url)),
     )
 ), about.INSTALL_MESSAGE
```

### Comparing `propan-0.1.4.6/propan/types.py` & `propan-0.1.5.0/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/__init__.py` & `propan-0.1.5.0/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/channels.py` & `propan-0.1.5.0/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/info.py` & `propan-0.1.5.0/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/main.py` & `propan-0.1.5.0/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/message.py` & `propan-0.1.5.0/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/security.py` & `propan-0.1.5.0/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/subscription.py` & `propan-0.1.5.0/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/bindings/amqp.py` & `propan-0.1.5.0/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/bindings/kafka.py` & `propan-0.1.5.0/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/bindings/main.py` & `propan-0.1.5.0/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/asyncapi/bindings/redis.py` & `propan-0.1.5.0/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/push_back_watcher.py` & `propan-0.1.5.0/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/_model/broker_usecase.py` & `propan-0.1.5.0/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/_model/routing.py` & `propan-0.1.5.0/propan/brokers/_model/routing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/_model/schemas.py` & `propan-0.1.5.0/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/_model/utils.py` & `propan-0.1.5.0/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.5.0/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.5.0/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/kafka/routing.pyi` & `propan-0.1.5.0/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/kafka/schemas.py` & `propan-0.1.5.0/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/nats/nats_broker.py` & `propan-0.1.5.0/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.5.0/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/nats/routing.pyi` & `propan-0.1.5.0/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/nats/schemas.py` & `propan-0.1.5.0/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/rabbit/logging.py` & `propan-0.1.5.0/propan/brokers/rabbit/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.5.0/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/rabbit/routing.pyi` & `propan-0.1.5.0/propan/brokers/rabbit/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/rabbit/schemas.py` & `propan-0.1.5.0/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/rabbit/utils.py` & `propan-0.1.5.0/propan/brokers/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/redis/redis_broker.py` & `propan-0.1.5.0/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.5.0/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/redis/routing.pyi` & `propan-0.1.5.0/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/redis/schemas.py` & `propan-0.1.5.0/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/sqs/routing.pyi` & `propan-0.1.5.0/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/sqs/schema.py` & `propan-0.1.5.0/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.5.0/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.5.0/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/main.py` & `propan-0.1.5.0/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/docs/app.py` & `propan-0.1.5.0/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/docs/gen.py` & `propan-0.1.5.0/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/docs/serving.py` & `propan-0.1.5.0/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/startproject/core.py` & `propan-0.1.5.0/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/app.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import typer
 
 from propan.cli.startproject.async_app.kafka import create_kafka
-from propan.cli.startproject.async_app.nats import create_nats
+from propan.cli.startproject.async_app.nats import create_nats, create_nats_js
 from propan.cli.startproject.async_app.rabbit import create_rabbit
 from propan.cli.startproject.async_app.redis import create_redis
 from propan.cli.startproject.async_app.sqs import create_sqs
 
 async_app = typer.Typer(pretty_exceptions_short=True)
 
 
@@ -28,14 +28,21 @@
 @async_app.command()
 def nats(appname: str) -> None:
     """Create an asyncronous Nats Propan project at [APPNAME] directory"""
     project = create_nats(Path.cwd() / appname)
     typer.echo(f"Create an asyncronous Nats Propan project at: {project}")
 
 
+@async_app.command(name="nats-js")
+def nats_js(appname: str) -> None:
+    """Create an asyncronous NatsJS Propan project at [APPNAME] directory"""
+    project = create_nats_js(Path.cwd() / appname)
+    typer.echo(f"Create an asyncronous NatsJS Propan project at: {project}")
+
+
 @async_app.command()
 def kafka(appname: str) -> None:
     """Create an asyncronous Kafka Propan project at [APPNAME] directory"""
     project = create_kafka(Path.cwd() / appname)
     typer.echo(f"Create an asyncronous Kafka Propan project at: {project}")
```

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/core.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/nats.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/rabbit.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,63 +6,71 @@
     create_config_dir,
     create_env,
     create_project_dir,
 )
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
-def create_nats(dir: Path) -> Path:
+def create_rabbit(dir: Path) -> Path:
     project_dir = _create_project_dir(dir)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
 def _create_project_dir(dirname: Path) -> Path:
-    project_dir = create_project_dir(dirname, "propan[async-nats]")
+    project_dir = create_project_dir(dirname, "propan[async-rabbit]")
 
     write_file(
         project_dir / "docker-compose.yaml",
         'version: "3"',
         "",
         "services:",
-        "  nats:",
-        "    image: nats",
+        "  rabbit:",
+        "    image: rabbitmq",
+        "    environment:",
+        "      RABBITMQ_DEFAULT_USER: guest",
+        "      RABBITMQ_DEFAULT_PASS: guest",
+        "    healthcheck:",
+        "      test: rabbitmq-diagnostics -q ping",
+        "      interval: 3s",
+        "      timeout: 30s",
+        "      retries: 3",
         "    ports:",
-        "      - 4222:4222",
-        "      - 8222:8222  # management",
+        "      - 5672:5672",
         "",
         "  app:",
         "    build: .",
         "    environment:",
-        "      APP_BROKER__URL: nats://nats:4222/",
+        "      APP_BROKER__URL: amqp://guest:guest@rabbit:5672/",
         "    volumes:",
         "      - ./app:/home/user/app:ro",
         "    depends_on:",
-        "      - nats",
+        "      rabbit:",
+        "        condition: service_healthy",
     )
 
     return project_dir
 
 
 def _create_app_dir(app: Path) -> Path:
     app_dir = touch_dir(app)
-    create_app_file(app_dir, "NatsBroker")
+    create_app_file(app_dir, "RabbitBroker")
     return app_dir
 
 
 def _create_config_dir(config: Path) -> Path:
     config_dir = create_config_dir(config)
-    create_env(config_dir, "nats://localhost:4222/")
+    create_env(config_dir, "amqp://guest:guest@localhost:5672/")
     return config_dir
 
 
 def _create_apps_dir(apps: Path) -> Path:
     apps_dir = create_apps_dir(apps)
 
     create_handlers_file(
         apps_dir / "handlers.py",
-        "NatsRouter",
+        "RabbitRouter",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/nats.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,71 +6,72 @@
     create_config_dir,
     create_env,
     create_project_dir,
 )
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
-def create_rabbit(dir: Path) -> Path:
-    project_dir = _create_project_dir(dir)
-    app_dir = _create_app_dir(project_dir / "app")
+def create_nats(dir: Path) -> Path:
+    project_dir = _create_project_dir(dir, js=False)
+    app_dir = _create_app_dir(project_dir / "app", js=False)
     _create_config_dir(app_dir / "config")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
-def _create_project_dir(dirname: Path) -> Path:
-    project_dir = create_project_dir(dirname, "propan[async-rabbit]")
+def create_nats_js(dir: Path) -> Path:
+    project_dir = _create_project_dir(dir, js=True)
+    app_dir = _create_app_dir(project_dir / "app", js=True)
+    _create_config_dir(app_dir / "config")
+    _create_apps_dir(app_dir / "apps")
+    return project_dir
+
+
+def _create_project_dir(dirname: Path, js: bool) -> Path:
+    project_dir = create_project_dir(dirname, "propan[async-nats]")
 
     write_file(
         project_dir / "docker-compose.yaml",
         'version: "3"',
         "",
         "services:",
-        "  rabbit:",
-        "    image: rabbitmq",
-        "    environment:",
-        "      RABBITMQ_DEFAULT_USER: guest",
-        "      RABBITMQ_DEFAULT_PASS: guest",
-        "    healthcheck:",
-        "      test: rabbitmq-diagnostics -q ping",
-        "      interval: 3s",
-        "      timeout: 30s",
-        "      retries: 3",
+        "  nats:",
+        "    image: nats",
         "    ports:",
-        "      - 5672:5672",
+        "      - 4222:4222",
+        "      - 8222:8222  # management",
+        "    command: -js" if js else "",
         "",
         "  app:",
         "    build: .",
         "    environment:",
-        "      APP_BROKER__URL: amqp://guest:guest@rabbit:5672/",
+        "      APP_BROKER__URL: nats://nats:4222/",
         "    volumes:",
         "      - ./app:/home/user/app:ro",
         "    depends_on:",
-        "      rabbit:",
-        "        condition: service_healthy",
+        "      - nats",
     )
 
     return project_dir
 
 
-def _create_app_dir(app: Path) -> Path:
+def _create_app_dir(app: Path, js: bool) -> Path:
     app_dir = touch_dir(app)
-    create_app_file(app_dir, "RabbitBroker")
+    create_app_file(app_dir, "NatsJSBroker" if js else "NatsBroker")
     return app_dir
 
 
 def _create_config_dir(config: Path) -> Path:
     config_dir = create_config_dir(config)
-    create_env(config_dir, "amqp://guest:guest@localhost:5672/")
+    create_env(config_dir, "nats://localhost:4222/")
     return config_dir
 
 
 def _create_apps_dir(apps: Path) -> Path:
     apps_dir = create_apps_dir(apps)
 
     create_handlers_file(
         apps_dir / "handlers.py",
-        "RabbitRouter",
+        "NatsRouter",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/redis.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.5.0/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/supervisors/basereload.py` & `propan-0.1.5.0/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/supervisors/multiprocess.py` & `propan-0.1.5.0/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/supervisors/utils.py` & `propan-0.1.5.0/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/supervisors/watchfiles.py` & `propan-0.1.5.0/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/utils/imports.py` & `propan-0.1.5.0/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/utils/logs.py` & `propan-0.1.5.0/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/cli/utils/parser.py` & `propan-0.1.5.0/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/fastapi/__init__.py` & `propan-0.1.5.0/propan/fastapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,28 @@
 
 try:
     from propan.fastapi.kafka import KafkaRouter
 except ImportError:
     KafkaRouter = about.INSTALL_KAFKA  # type: ignore
 
 try:
-    from propan.fastapi.nats import NatsRouter
+    from propan.fastapi.nats import NatsJSRouter, NatsRouter
 except ImportError:
-    NatsRouter = about.INSTALL_NATS  # type: ignore
+    NatsRouter = NatsJSRouter = about.INSTALL_NATS  # type: ignore
 
 try:
     from propan.fastapi.sqs import SQSRouter
 except ImportError:
     SQSRouter = about.INSTALL_SQS  # type: ignore
 
 assert any(
     (RabbitRouter, RedisRouter, KafkaRouter, NatsRouter, SQSRouter)
 ), about.INSTALL_MESSAGE
 
-__all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter", "NatsRouter", "SQSRouter")
+__all__ = (
+    "RabbitRouter",
+    "RedisRouter",
+    "KafkaRouter",
+    "NatsRouter",
+    "SQSRouter",
+    "NatsJSRouter",
+)
```

### Comparing `propan-0.1.4.6/propan/fastapi/core/route.py` & `propan-0.1.5.0/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/fastapi/core/router.py` & `propan-0.1.5.0/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/fastapi/kafka/router.pyi` & `propan-0.1.5.0/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/fastapi/rabbit/router.pyi` & `propan-0.1.5.0/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/fastapi/redis/router.pyi` & `propan-0.1.5.0/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/fastapi/sqs/router.pyi` & `propan-0.1.5.0/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/log/formatter.py` & `propan-0.1.5.0/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/log/logging.py` & `propan-0.1.5.0/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/test/__init__.py` & `propan-0.1.5.0/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/test/kafka.py` & `propan-0.1.5.0/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/test/nats.py` & `propan-0.1.5.0/propan/test/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,87 @@
+import re
 import sys
 from types import MethodType
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
-from nats.aio.msg import Msg
+from typing_extensions import TypeAlias
 
 if sys.version_info < (3, 8):
     from asyncmock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
-from propan import NatsBroker
+from propan._compat import model_to_json
+from propan.brokers.redis.redis_broker import RedisBroker
+from propan.brokers.redis.schemas import RedisMessage
 from propan.test.utils import call_handler
 from propan.types import SendableMessage
 
 __all__ = (
     "build_message",
-    "TestNatsBroker",
+    "TestRedisBroker",
 )
 
+Msg: TypeAlias = Dict[str, Union[bytes, str, None]]
+
 
 def build_message(
     message: SendableMessage,
-    subject: str,
+    channel: str,
     *,
     reply_to: str = "",
     headers: Optional[Dict[str, Any]] = None,
 ) -> Msg:
-    msg, content_type = NatsBroker._encode_message(message)
-    return Msg(
-        _client=None,  # type: ignore
-        subject=subject,
-        reply=reply_to,
-        data=msg,
-        headers={
-            **(headers or {}),
-            "content-type": content_type or "",
-        },
-    )
+    msg, content_type = RedisBroker._encode_message(message)
+    return {
+        "type": "message",
+        "pattern": None,
+        "channel": channel.encode(),
+        "data": model_to_json(
+            RedisMessage(
+                data=msg,
+                headers={
+                    "content-type": content_type or "",
+                    **(headers or {}),
+                },
+                reply_to=reply_to,
+            )
+        ).encode(),
+    }
 
 
 async def publish(
-    self: NatsBroker,
+    self: RedisBroker,
     message: SendableMessage,
-    subject: str,
+    channel: str,
     *,
     reply_to: str = "",
     headers: Optional[Dict[str, Any]] = None,
     callback: bool = False,
     callback_timeout: Optional[float] = 30.0,
     raise_timeout: bool = False,
 ) -> Any:
     incoming = build_message(
         message=message,
-        subject=subject,
+        channel=channel,
         reply_to=reply_to,
         headers=headers,
     )
 
     for handler in self.handlers:  # pragma: no branch
-        if subject == handler.subject:  # pragma: no branch
+        if (
+            not handler.pattern and handler.channel == channel
+        ) or (  # pragma: no branch
+            handler.pattern and re.match(handler.channel, channel)
+        ):
             r = await call_handler(
                 handler, incoming, callback, callback_timeout, raise_timeout
             )
             if callback:  # pragma: no branch
                 return r
 
 
-def TestNatsBroker(broker: NatsBroker) -> NatsBroker:
+def TestRedisBroker(broker: RedisBroker) -> RedisBroker:
     broker.connect = AsyncMock()  # type: ignore
     broker.start = AsyncMock()  # type: ignore
     broker.publish = MethodType(publish, broker)  # type: ignore
     return broker
```

### Comparing `propan-0.1.4.6/propan/test/rabbit.py` & `propan-0.1.5.0/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/test/redis.py` & `propan-0.1.5.0/propan/test/nats.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,92 @@
-import re
 import sys
 from types import MethodType
 from typing import Any, Dict, Optional, Union
+from uuid import uuid4
 
-from typing_extensions import TypeAlias
+from nats.aio.msg import Msg
 
 if sys.version_info < (3, 8):
     from asyncmock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
-from propan._compat import model_to_json
-from propan.brokers.redis.redis_broker import RedisBroker
-from propan.brokers.redis.schemas import RedisMessage
+from propan import NatsBroker
 from propan.test.utils import call_handler
 from propan.types import SendableMessage
 
 __all__ = (
     "build_message",
-    "TestRedisBroker",
+    "TestNatsBroker",
 )
 
-Msg: TypeAlias = Dict[str, Union[bytes, str, None]]
+
+class PatchedMessage(Msg):
+    async def ack(self) -> None:
+        pass
+
+    async def ack_sync(self, timeout: float = 1) -> None:
+        pass
+
+    async def nak(self, delay: Union[int, float, None] = None) -> None:
+        pass
+
+    async def term(self) -> None:
+        pass
+
+    async def in_progress(self) -> None:
+        pass
 
 
 def build_message(
     message: SendableMessage,
-    channel: str,
+    subject: str,
     *,
     reply_to: str = "",
     headers: Optional[Dict[str, Any]] = None,
-) -> Msg:
-    msg, content_type = RedisBroker._encode_message(message)
-    return {
-        "type": "message",
-        "pattern": None,
-        "channel": channel.encode(),
-        "data": model_to_json(
-            RedisMessage(
-                data=msg,
-                headers={
-                    "content-type": content_type or "",
-                    **(headers or {}),
-                },
-                reply_to=reply_to,
-            )
-        ).encode(),
-    }
+) -> PatchedMessage:
+    msg, content_type = NatsBroker._encode_message(message)
+    return PatchedMessage(
+        _client=None,  # type: ignore
+        subject=subject,
+        reply=reply_to or str(uuid4()),
+        data=msg,
+        headers={
+            **(headers or {}),
+            "content-type": content_type or "",
+        },
+    )
 
 
 async def publish(
-    self: RedisBroker,
+    self: NatsBroker,
     message: SendableMessage,
-    channel: str,
+    subject: str,
     *,
     reply_to: str = "",
     headers: Optional[Dict[str, Any]] = None,
     callback: bool = False,
     callback_timeout: Optional[float] = 30.0,
     raise_timeout: bool = False,
 ) -> Any:
     incoming = build_message(
         message=message,
-        channel=channel,
+        subject=subject,
         reply_to=reply_to,
         headers=headers,
     )
 
     for handler in self.handlers:  # pragma: no branch
-        if (
-            not handler.pattern and handler.channel == channel
-        ) or (  # pragma: no branch
-            handler.pattern and re.match(handler.channel, channel)
-        ):
+        if subject == handler.subject:  # pragma: no branch
             r = await call_handler(
                 handler, incoming, callback, callback_timeout, raise_timeout
             )
             if callback:  # pragma: no branch
                 return r
 
 
-def TestRedisBroker(broker: RedisBroker) -> RedisBroker:
+def TestNatsBroker(broker: NatsBroker) -> NatsBroker:
     broker.connect = AsyncMock()  # type: ignore
     broker.start = AsyncMock()  # type: ignore
+    broker._raw_connection = AsyncMock()  # type: ignore
     broker.publish = MethodType(publish, broker)  # type: ignore
     return broker
```

### Comparing `propan-0.1.4.6/propan/test/sqs.py` & `propan-0.1.5.0/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/test/utils.py` & `propan-0.1.5.0/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/utils/functions.py` & `propan-0.1.5.0/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/utils/context/main.py` & `propan-0.1.5.0/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/propan/utils/context/types.py` & `propan-0.1.5.0/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/LICENSE` & `propan-0.1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/README.md` & `propan-0.1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 |                   | async                                                   | sync                                        |
 |-------------------|:-------------------------------------------------------:|:-------------------------------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :hammer_and_wrench: WIP :hammer_and_wrench: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Nats**          | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
-| **NatsJS**        | :hammer_and_wrench: **WIP** :hammer_and_wrench:         | :mag: planning :mag:                        |
+| **NatsJS**        | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ActiveMQ**      | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ZeroMQ**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 
 ---
@@ -228,15 +228,14 @@
 Also, you can specify your own dependencies, call dependencies functions (like `FastAPI Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 from propan import PropanApp, RabbitBroker, Context, Depends
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-
 app = PropanApp(rabbit_broker)
 
 async def dependency(user_id: int) -> bool:
     return True
 
 @rabbit_broker.handle("test")
 async def base_handler(user_id: int,
@@ -244,14 +243,35 @@
                        broker: RabbitBroker = Context()):
     assert dep is True
     assert broker is rabbit_broker
 ```
 
 ---
 
+## RPC over MQ
+
+Also, **Propan** allows you to use **RPC** requests over your broker with a simple way:
+
+```python
+from propan import PropanApp, RabbitBroker
+
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
+app = PropanApp(rabbit_broker)
+
+@broker.handle("ping")
+async def base_handler():
+    return "pong"
+
+@app.after_startup
+async def self_ping():
+    assert (await broker.publish("", "ping")) == "pong"
+```
+
+---
+
 ## Project Documentation
 
 **Propan** automatically generates documentation for your project according to the <a href="https://www.asyncapi.com/" target="_blank">**AsyncAPI**</a> specification. You can work with both generated artifacts and place a Web view of your documentation on resources available to related teams.
 
 The availability of such documentation significantly simplifies the integration of services: you can immediately see what channels and message format the application works with. And most importantly, it doesn't cost you anything - **Propan** has already done everything for you!
 
 ![HTML-page](https://lancetnik.github.io/Propan/assets/img/docs-html-short.png)
```

#### html2text {}

```diff
@@ -28,22 +28,22 @@
 | async | sync | |-------------------|:----------------------------------------
 ---------------:|:-------------------------------------------:| | **RabbitMQ**
 | :heavy_check_mark: **stable** :heavy_check_mark: | :hammer_and_wrench: WIP :
 hammer_and_wrench: | | **Redis** | :heavy_check_mark: **stable** :
 heavy_check_mark: | :mag: planning :mag: | | **Nats** | :heavy_check_mark:
 **stable** :heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning:
 **beta** :warning: | :mag: planning :mag: | | **SQS** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **WIP** :
-hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
-:mag: planning :mag: | | **Redis Streams** | :mag: planning :mag: | :mag:
-planning :mag: | | **Pulsar** | :mag: planning :mag: | :mag: planning :mag: | |
-**ActiveMQ** | :mag: planning :mag: | :mag: planning :mag: | | **ZeroMQ** | :
-mag: planning :mag: | :mag: planning :mag: | --- ### â­ Support the project
-â­ If you are interested in this project, please give me feedback by: - giving
-the [repository](https://github.com/Lancetnik/Propan) a star - tweet about
+warning: | :mag: planning :mag: | | **NatsJS** | :warning: **beta** :warning: |
+:mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
+| | **Redis Streams** | :mag: planning :mag: | :mag: planning :mag: | |
+**Pulsar** | :mag: planning :mag: | :mag: planning :mag: | | **ActiveMQ** | :
+mag: planning :mag: | :mag: planning :mag: | | **ZeroMQ** | :mag: planning :
+mag: | :mag: planning :mag: | --- ### â­ Support the project â­ If you are
+interested in this project, please give me feedback by: - giving the
+[repository](https://github.com/Lancetnik/Propan) a star - tweet about
 **Propan** and let me and others know why you use it. - joining Discord_server.
 Your support helps me to stay in touch with you and encourages us to continue
 developing and improving the library. Thank you for your support! Really, share
 information about this project with overs. The bigger community we have - the
 better project will be! --- ## Declarative? With declarative tools you can
 define **what you need to get**. With traditional imperative tools you must
 write **what you need to do**. Take a look at classic imperative tools, such as
@@ -86,52 +86,58 @@
 you can specify your own dependencies, call dependencies functions (like
 `FastAPI Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/
 examples/dependencies). ```python from propan import PropanApp, RabbitBroker,
 Context, Depends rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:
 5672/") app = PropanApp(rabbit_broker) async def dependency(user_id: int) -
 > bool: return True @rabbit_broker.handle("test") async def base_handler
 (user_id: int, dep: bool = Depends(dependency), broker: RabbitBroker = Context
-()): assert dep is True assert broker is rabbit_broker ``` --- ## Project
-Documentation **Propan** automatically generates documentation for your project
-according to the **AsyncAPI** specification. You can work with both generated
-artifacts and place a Web view of your documentation on resources available to
-related teams. The availability of such documentation significantly simplifies
-the integration of services: you can immediately see what channels and message
-format the application works with. And most importantly, it doesn't cost you
-anything - **Propan** has already done everything for you! ![HTML-page](https:/
-/lancetnik.github.io/Propan/assets/img/docs-html-short.png) --- ## CLI power
-**Propan** has its own CLI tool that provided the following features: * project
-generation * multiprocessing workers * project hot reloading * documentation
-generating and hosting * custom command line arguments passing ### Context
-passing For example: pass your current *.env* project setting to context
-```bash propan run serve:app --env=.env.dev ``` ```python from propan import
-PropanApp, RabbitBroker from propan.annotations import ContextRepo from
-pydantic import BaseSettings broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) class Settings(BaseSettings):
-... @app.on_startup async def setup(env: str, context: ContextRepo): settings =
-Settings(_env_file=env) context.set_global("settings", settings) ``` ###
-Project template Also, **Propan CLI** is able to generate a production-ready
-application template: ```bash propan create async rabbit [projectname] ```
-*Notice: project template require* `pydantic[dotenv]` *installation.* Run the
-created project: ```bash # Run rabbimq first docker compose --file
-[projectname]/docker-compose.yaml up -d # Run project propan run
-[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
-development experience! --- ## HTTP Frameworks integrations ### Any Framework
-You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
-them according to your application lifespan. ```python from propan import
-NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
-NatsBroker("nats://localhost:4222") @broker.handle("test") async def
-base_handler(body): print(body) @app.after_server_start async def start_broker
-(app, loop): await broker.start() @app.after_server_stop async def stop_broker
-(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
-be used as part of **FastAPI**. Just import a **PropanRouter** you need and
-declare the message handler using the `@event` decorator. This decorator is
-similar to the decorator `@handle` for the corresponding brokers. ```python
-from fastapi import Depends, FastAPI from pydantic import BaseModel from
-propan.fastapi import RabbitRouter router = RabbitRouter("amqp://guest:
-guest@localhost:5672") app = FastAPI(lifespan=router.lifespan_context) class
-Incoming(BaseModel): m: dict def call(): return True @router.event("test")
-async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
-"Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
-framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
-tree/main/examples) ## Contributors Thanks for all of these amazing peoples
-made the project better! [https://contrib.rocks/image?repo=Lancetnik/Propan]
+()): assert dep is True assert broker is rabbit_broker ``` --- ## RPC over MQ
+Also, **Propan** allows you to use **RPC** requests over your broker with a
+simple way: ```python from propan import PropanApp, RabbitBroker broker =
+RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(rabbit_broker) @broker.handle("ping") async def base_handler(): return "pong"
+@app.after_startup async def self_ping(): assert (await broker.publish("",
+"ping")) == "pong" ``` --- ## Project Documentation **Propan** automatically
+generates documentation for your project according to the **AsyncAPI**
+specification. You can work with both generated artifacts and place a Web view
+of your documentation on resources available to related teams. The availability
+of such documentation significantly simplifies the integration of services: you
+can immediately see what channels and message format the application works
+with. And most importantly, it doesn't cost you anything - **Propan** has
+already done everything for you! ![HTML-page](https://lancetnik.github.io/
+Propan/assets/img/docs-html-short.png) --- ## CLI power **Propan** has its own
+CLI tool that provided the following features: * project generation *
+multiprocessing workers * project hot reloading * documentation generating and
+hosting * custom command line arguments passing ### Context passing For
+example: pass your current *.env* project setting to context ```bash propan run
+serve:app --env=.env.dev ``` ```python from propan import PropanApp,
+RabbitBroker from propan.annotations import ContextRepo from pydantic import
+BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
+setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
+context.set_global("settings", settings) ``` ### Project template Also,
+**Propan CLI** is able to generate a production-ready application template:
+```bash propan create async rabbit [projectname] ``` *Notice: project template
+require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
+Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
+d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
+Now you can enjoy a new development experience! --- ## HTTP Frameworks
+integrations ### Any Framework You can use **Propan** `MQBrokers` without
+`PropanApp`. Just *start* and *stop* them according to your application
+lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
+Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
+@broker.handle("test") async def base_handler(body): print(body)
+@app.after_server_start async def start_broker(app, loop): await broker.start()
+@app.after_server_stop async def stop_broker(app, loop): await broker.close()
+``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
+Just import a **PropanRouter** you need and declare the message handler using
+the `@event` decorator. This decorator is similar to the decorator `@handle`
+for the corresponding brokers. ```python from fastapi import Depends, FastAPI
+from pydantic import BaseModel from propan.fastapi import RabbitRouter router =
+RabbitRouter("amqp://guest:guest@localhost:5672") app = FastAPI
+(lifespan=router.lifespan_context) class Incoming(BaseModel): m: dict def call
+(): return True @router.event("test") async def hello(m: Incoming, d = Depends
+(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
+(router) ``` ## Examples To see more framework usages go to [**examples/**]
+(https://github.com/Lancetnik/Propan/tree/main/examples) ## Contributors Thanks
+for all of these amazing peoples made the project better! [https://
+contrib.rocks/image?repo=Lancetnik/Propan]
```

### Comparing `propan-0.1.4.6/pyproject.toml` & `propan-0.1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.6/PKG-INFO` & `propan-0.1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.4.6
+Version: 0.1.5.0
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -159,15 +159,15 @@
 |                   | async                                                   | sync                                        |
 |-------------------|:-------------------------------------------------------:|:-------------------------------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :hammer_and_wrench: WIP :hammer_and_wrench: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Nats**          | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag:                        |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
-| **NatsJS**        | :hammer_and_wrench: **WIP** :hammer_and_wrench:         | :mag: planning :mag:                        |
+| **NatsJS**        | :warning: **beta** :warning:                            | :mag: planning :mag:                        |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ActiveMQ**      | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 | **ZeroMQ**        | :mag: planning :mag:                                    | :mag: planning :mag:                        |
 
 ---
@@ -322,15 +322,14 @@
 Also, you can specify your own dependencies, call dependencies functions (like `FastAPI Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 from propan import PropanApp, RabbitBroker, Context, Depends
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-
 app = PropanApp(rabbit_broker)
 
 async def dependency(user_id: int) -> bool:
     return True
 
 @rabbit_broker.handle("test")
 async def base_handler(user_id: int,
@@ -338,14 +337,35 @@
                        broker: RabbitBroker = Context()):
     assert dep is True
     assert broker is rabbit_broker
 ```
 
 ---
 
+## RPC over MQ
+
+Also, **Propan** allows you to use **RPC** requests over your broker with a simple way:
+
+```python
+from propan import PropanApp, RabbitBroker
+
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
+app = PropanApp(rabbit_broker)
+
+@broker.handle("ping")
+async def base_handler():
+    return "pong"
+
+@app.after_startup
+async def self_ping():
+    assert (await broker.publish("", "ping")) == "pong"
+```
+
+---
+
 ## Project Documentation
 
 **Propan** automatically generates documentation for your project according to the <a href="https://www.asyncapi.com/" target="_blank">**AsyncAPI**</a> specification. You can work with both generated artifacts and place a Web view of your documentation on resources available to related teams.
 
 The availability of such documentation significantly simplifies the integration of services: you can immediately see what channels and message format the application works with. And most importantly, it doesn't cost you anything - **Propan** has already done everything for you!
 
 ![HTML-page](https://lancetnik.github.io/Propan/assets/img/docs-html-short.png)
```

