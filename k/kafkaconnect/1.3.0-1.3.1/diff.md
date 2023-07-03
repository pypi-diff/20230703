# Comparing `tmp/kafkaconnect-1.3.0.tar.gz` & `tmp/kafkaconnect-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaconnect-1.3.0.tar", last modified: Mon Jul  3 15:11:22 2023, max compression
+gzip compressed data, was "kafkaconnect-1.3.1.tar", last modified: Mon Jul  3 17:02:04 2023, max compression
```

## Comparing `kafkaconnect-1.3.0.tar` & `kafkaconnect-1.3.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.github/workflows/strimzi-kafka.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.298359 kafkaconnect-1.3.0/connectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/connectors/jdbc_sink/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/jdbc_sink/jdbc-sink-connector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/connectors/mirrormaker2/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/checkpoint-connector.json
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/heartbeat-connector.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/mirror-source-connector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/connectors/s3_sink/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/s3_sink/s3-sink-connector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/manifest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    77184 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/main.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/scripts/docker-tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/scripts/install-base-packages.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.298359 kafkaconnect-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/topic_names_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:11:17.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/strimzi-kafka/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/strimzi-kafka/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/strimzi-kafka/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_create_or_update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_pause.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_plugins.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_remove.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_restart.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_resume.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_status.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_tasks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_topics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_validate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_topic_names_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.927784 kafkaconnect-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.919784 kafkaconnect-1.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.919784 kafkaconnect-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/.github/workflows/strimzi-kafka.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-03 17:02:04.927784 kafkaconnect-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.915784 kafkaconnect-1.3.1/connectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.919784 kafkaconnect-1.3.1/connectors/jdbc_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/connectors/jdbc_sink/jdbc-sink-connector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.919784 kafkaconnect-1.3.1/connectors/mirrormaker2/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/connectors/mirrormaker2/checkpoint-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/connectors/mirrormaker2/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/connectors/mirrormaker2/heartbeat-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/connectors/mirrormaker2/mirror-source-connector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.919784 kafkaconnect-1.3.1/connectors/s3_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/connectors/s3_sink/s3-sink-connector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.919784 kafkaconnect-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/manifest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    77184 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/requirements/main.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/scripts/docker-tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/scripts/install-base-packages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-03 17:02:04.927784 kafkaconnect-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.915784 kafkaconnect-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/src/kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/src/kafkaconnect/influxdb_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/influxdb_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/influxdb_sink/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/influxdb_sink/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/src/kafkaconnect/jdbc_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/jdbc_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/jdbc_sink/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/src/kafkaconnect/mirrormaker2/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/mirrormaker2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/mirrormaker2/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/src/kafkaconnect/s3_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/s3_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/s3_sink/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/src/kafkaconnect/topic_names_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-03 17:02:04.000000 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 17:02:04.000000 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:02:04.000000 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 17:02:04.000000 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:01:59.000000 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 17:02:04.000000 kafkaconnect-1.3.1/src/kafkaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.923784 kafkaconnect-1.3.1/strimzi-kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/strimzi-kafka/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/strimzi-kafka/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.927784 kafkaconnect-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:02:04.927784 kafkaconnect-1.3.1/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_create_or_update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_pause.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_plugins.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_remove.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_restart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_resume.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_tasks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_topics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/cassettes/test_validate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 17:01:53.000000 kafkaconnect-1.3.1/tests/test_topic_names_set.py
```

### Comparing `kafkaconnect-1.3.0/.github/workflows/ci.yaml` & `kafkaconnect-1.3.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/.github/workflows/strimzi-kafka.yaml` & `kafkaconnect-1.3.1/.github/workflows/strimzi-kafka.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/.gitignore` & `kafkaconnect-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/.pre-commit-config.yaml` & `kafkaconnect-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/CHANGELOG.rst` & `kafkaconnect-1.3.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ##########
 Change log
 ##########
 
+1.3.1 (2023-07-03)
+==================
+
+* Add the --remove-prefix option to rename measurements in the InfluxDB Sink connector
+
 1.2.0 (2023-06-12)
 ==================
 
 * Add support to Strimzi Kafka 0.35.1 and Kafka 3.4.0
 
 1.1.0 (2023-05-28)
 ==================
```

### Comparing `kafkaconnect-1.3.0/Dockerfile` & `kafkaconnect-1.3.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/LICENSE` & `kafkaconnect-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/Makefile` & `kafkaconnect-1.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/PKG-INFO` & `kafkaconnect-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaconnect
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for managing Kafka connectors.
 Home-page: https://github.com/lsst-sqre/kafka-connect-manager
 Author: Association of Universities for Research in Astronomy, Inc. (AURA)
 Author-email: sqre-admin@lists.lsst.org
 Project-URL: Change log, https://github.com/lsst-sqre/kafka-connect-manager/blob/master/CHANGELOG.rst
 Project-URL: Source code, https://github.com/lsst-sqre/kafka-connect-manager
 Project-URL: Issue tracker, https://github.com/lsst-sqre/kafka-connect-manager/issues
@@ -41,14 +41,19 @@
   :scale: 100%
   :target: https://hub.docker.com/repository/docker/lsstsqre/kafkaconnect
 
 ##########
 Change log
 ##########
 
+1.3.1 (2023-07-03)
+==================
+
+* Add the --remove-prefix option to rename measurements in the InfluxDB Sink connector
+
 1.2.0 (2023-06-12)
 ==================
 
 * Add support to Strimzi Kafka 0.35.1 and Kafka 3.4.0
 
 1.1.0 (2023-05-28)
 ==================
```

### Comparing `kafkaconnect-1.3.0/README.rst` & `kafkaconnect-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/connectors/mirrormaker2/docker-compose.yaml` & `kafkaconnect-1.3.1/connectors/mirrormaker2/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/connectors/mirrormaker2/mirror-source-connector.json` & `kafkaconnect-1.3.1/connectors/mirrormaker2/mirror-source-connector.json`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/connectors/s3_sink/s3-sink-connector.json` & `kafkaconnect-1.3.1/connectors/s3_sink/s3-sink-connector.json`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/Makefile` & `kafkaconnect-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/changelog.rst` & `kafkaconnect-1.3.1/docs/changelog.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ##########
 Change log
 ##########
 
+1.3.1 (2023-07-03)
+==================
+
+* Add the --remove-prefix option to rename measurements in the InfluxDB Sink connector
+
 1.2.0 (2023-06-12)
 ==================
 
 * Add support to Strimzi Kafka 0.35.1 and Kafka 3.4.0
 
 1.1.0 (2023-05-28)
 ==================
```

### Comparing `kafkaconnect-1.3.0/docs/conf.py` & `kafkaconnect-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/contributing.rst` & `kafkaconnect-1.3.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/development.rst` & `kafkaconnect-1.3.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/index.rst` & `kafkaconnect-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/installation.rst` & `kafkaconnect-1.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/overview.rst` & `kafkaconnect-1.3.1/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/docs/userguide.rst` & `kafkaconnect-1.3.1/docs/userguide.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/pyproject.toml` & `kafkaconnect-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/requirements/dev.txt` & `kafkaconnect-1.3.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/requirements/main.txt` & `kafkaconnect-1.3.1/requirements/main.txt`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/scripts/install-base-packages.sh` & `kafkaconnect-1.3.1/scripts/install-base-packages.sh`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/setup.cfg` & `kafkaconnect-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/cli.py` & `kafkaconnect-1.3.1/src/kafkaconnect/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/config.py` & `kafkaconnect-1.3.1/src/kafkaconnect/config.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/connect.py` & `kafkaconnect-1.3.1/src/kafkaconnect/connect.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/cli.py` & `kafkaconnect-1.3.1/src/kafkaconnect/influxdb_sink/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/config.py` & `kafkaconnect-1.3.1/src/kafkaconnect/influxdb_sink/config.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/cli.py` & `kafkaconnect-1.3.1/src/kafkaconnect/jdbc_sink/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/cli.py` & `kafkaconnect-1.3.1/src/kafkaconnect/mirrormaker2/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/cli.py` & `kafkaconnect-1.3.1/src/kafkaconnect/s3_sink/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect/topic_names_set.py` & `kafkaconnect-1.3.1/src/kafkaconnect/topic_names_set.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect.egg-info/PKG-INFO` & `kafkaconnect-1.3.1/src/kafkaconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaconnect
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for managing Kafka connectors.
 Home-page: https://github.com/lsst-sqre/kafka-connect-manager
 Author: Association of Universities for Research in Astronomy, Inc. (AURA)
 Author-email: sqre-admin@lists.lsst.org
 Project-URL: Change log, https://github.com/lsst-sqre/kafka-connect-manager/blob/master/CHANGELOG.rst
 Project-URL: Source code, https://github.com/lsst-sqre/kafka-connect-manager
 Project-URL: Issue tracker, https://github.com/lsst-sqre/kafka-connect-manager/issues
@@ -41,14 +41,19 @@
   :scale: 100%
   :target: https://hub.docker.com/repository/docker/lsstsqre/kafkaconnect
 
 ##########
 Change log
 ##########
 
+1.3.1 (2023-07-03)
+==================
+
+* Add the --remove-prefix option to rename measurements in the InfluxDB Sink connector
+
 1.2.0 (2023-06-12)
 ==================
 
 * Add support to Strimzi Kafka 0.35.1 and Kafka 3.4.0
 
 1.1.0 (2023-05-28)
 ==================
```

### Comparing `kafkaconnect-1.3.0/src/kafkaconnect.egg-info/SOURCES.txt` & `kafkaconnect-1.3.1/src/kafkaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_config.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_config.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_create_or_update.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_create_or_update.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_info.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_info.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_list.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_list.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_pause.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_pause.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_plugins.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_plugins.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_remove.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_remove.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_restart.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_restart.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_resume.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_resume.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_status.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_status.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_tasks.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_tasks.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_topics.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_topics.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/cassettes/test_validate.yaml` & `kafkaconnect-1.3.1/tests/cassettes/test_validate.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/docker-compose.yml` & `kafkaconnect-1.3.1/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/test_cli.py` & `kafkaconnect-1.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/test_connect.py` & `kafkaconnect-1.3.1/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/test_kafka.py` & `kafkaconnect-1.3.1/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.3.0/tests/test_topic_names_set.py` & `kafkaconnect-1.3.1/tests/test_topic_names_set.py`

 * *Files identical despite different names*

