# Comparing `tmp/kafkaconnect-1.2.0.tar.gz` & `tmp/kafkaconnect-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaconnect-1.2.0.tar", last modified: Tue Jun 13 01:02:42 2023, max compression
+gzip compressed data, was "kafkaconnect-1.3.0.tar", last modified: Mon Jul  3 15:11:22 2023, max compression
```

## Comparing `kafkaconnect-1.2.0.tar` & `kafkaconnect-1.3.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.168847 kafkaconnect-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.152846 kafkaconnect-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.152846 kafkaconnect-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/.github/workflows/strimzi-kafka.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-13 01:02:42.168847 kafkaconnect-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.148845 kafkaconnect-1.2.0/connectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.152846 kafkaconnect-1.2.0/connectors/jdbc_sink/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/connectors/jdbc_sink/jdbc-sink-connector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.152846 kafkaconnect-1.2.0/connectors/mirrormaker2/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/connectors/mirrormaker2/checkpoint-connector.json
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/connectors/mirrormaker2/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/connectors/mirrormaker2/heartbeat-connector.json
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/connectors/mirrormaker2/mirror-source-connector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.152846 kafkaconnect-1.2.0/connectors/s3_sink/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/connectors/s3_sink/s3-sink-connector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.160846 kafkaconnect-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/manifest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.160846 kafkaconnect-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    71856 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/requirements/main.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.160846 kafkaconnect-1.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/scripts/docker-tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/scripts/install-base-packages.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-13 01:02:42.172847 kafkaconnect-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.148845 kafkaconnect-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.160846 kafkaconnect-1.2.0/src/kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.164847 kafkaconnect-1.2.0/src/kafkaconnect/influxdb_sink/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/influxdb_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/influxdb_sink/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/influxdb_sink/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.164847 kafkaconnect-1.2.0/src/kafkaconnect/jdbc_sink/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/jdbc_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/jdbc_sink/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.164847 kafkaconnect-1.2.0/src/kafkaconnect/mirrormaker2/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/mirrormaker2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/mirrormaker2/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.164847 kafkaconnect-1.2.0/src/kafkaconnect/s3_sink/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/s3_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/s3_sink/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/src/kafkaconnect/topic_names_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.164847 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-13 01:02:42.000000 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-13 01:02:42.000000 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:02:42.000000 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 01:02:42.000000 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:02:36.000000 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 01:02:42.000000 kafkaconnect-1.2.0/src/kafkaconnect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.164847 kafkaconnect-1.2.0/strimzi-kafka/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/strimzi-kafka/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/strimzi-kafka/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.168847 kafkaconnect-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:02:42.168847 kafkaconnect-1.2.0/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_create_or_update.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_pause.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_plugins.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_remove.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_restart.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_resume.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_status.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_tasks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_topics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/cassettes/test_validate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-13 01:02:28.000000 kafkaconnect-1.2.0/tests/test_topic_names_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.github/workflows/strimzi-kafka.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.298359 kafkaconnect-1.3.0/connectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/connectors/jdbc_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/jdbc_sink/jdbc-sink-connector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/connectors/mirrormaker2/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/checkpoint-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/heartbeat-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/mirrormaker2/mirror-source-connector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/connectors/s3_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/connectors/s3_sink/s3-sink-connector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/manifest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    77184 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/requirements/main.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.302359 kafkaconnect-1.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/scripts/docker-tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/scripts/install-base-packages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.298359 kafkaconnect-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/src/kafkaconnect/topic_names_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:11:17.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 15:11:22.000000 kafkaconnect-1.3.0/src/kafkaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/strimzi-kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/strimzi-kafka/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/strimzi-kafka/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.306359 kafkaconnect-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:11:22.310359 kafkaconnect-1.3.0/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_create_or_update.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_pause.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_plugins.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_remove.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_restart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_resume.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_tasks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_topics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/cassettes/test_validate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 15:11:11.000000 kafkaconnect-1.3.0/tests/test_topic_names_set.py
```

### Comparing `kafkaconnect-1.2.0/.github/workflows/ci.yaml` & `kafkaconnect-1.3.0/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -160,11 +160,11 @@
         run: |
           python -m pip install --upgrade pip
           pip install .
           pip install --upgrade setuptools wheel
       - name: Build a binary wheel and a source tarball
         run: python setup.py sdist bdist_wheel
       - name: Publish package
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           user: __token__
           password: ${{ secrets.PYPI_SQRE_ADMIN }}
```

### Comparing `kafkaconnect-1.2.0/.github/workflows/strimzi-kafka.yaml` & `kafkaconnect-1.3.0/.github/workflows/strimzi-kafka.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/.gitignore` & `kafkaconnect-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/.pre-commit-config.yaml` & `kafkaconnect-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/CHANGELOG.rst` & `kafkaconnect-1.3.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/Dockerfile` & `kafkaconnect-1.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/LICENSE` & `kafkaconnect-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/Makefile` & `kafkaconnect-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/PKG-INFO` & `kafkaconnect-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaconnect
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python client for managing Kafka connectors.
 Home-page: https://github.com/lsst-sqre/kafka-connect-manager
 Author: Association of Universities for Research in Astronomy, Inc. (AURA)
 Author-email: sqre-admin@lists.lsst.org
 Project-URL: Change log, https://github.com/lsst-sqre/kafka-connect-manager/blob/master/CHANGELOG.rst
 Project-URL: Source code, https://github.com/lsst-sqre/kafka-connect-manager
 Project-URL: Issue tracker, https://github.com/lsst-sqre/kafka-connect-manager/issues
```

### Comparing `kafkaconnect-1.2.0/README.rst` & `kafkaconnect-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/connectors/mirrormaker2/docker-compose.yaml` & `kafkaconnect-1.3.0/connectors/mirrormaker2/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/connectors/mirrormaker2/mirror-source-connector.json` & `kafkaconnect-1.3.0/connectors/mirrormaker2/mirror-source-connector.json`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/connectors/s3_sink/s3-sink-connector.json` & `kafkaconnect-1.3.0/connectors/s3_sink/s3-sink-connector.json`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/Makefile` & `kafkaconnect-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/changelog.rst` & `kafkaconnect-1.3.0/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/conf.py` & `kafkaconnect-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/contributing.rst` & `kafkaconnect-1.3.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/development.rst` & `kafkaconnect-1.3.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/index.rst` & `kafkaconnect-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/installation.rst` & `kafkaconnect-1.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/overview.rst` & `kafkaconnect-1.3.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/docs/userguide.rst` & `kafkaconnect-1.3.0/docs/userguide.rst`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/pyproject.toml` & `kafkaconnect-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/requirements/dev.txt` & `kafkaconnect-1.3.0/requirements/dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/dev.txt requirements/dev.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/dev.txt requirements/dev.in
 #
 alabaster==0.7.13 \
     --hash=sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3 \
     --hash=sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2
     # via sphinx
+annotated-types==0.5.0 \
+    --hash=sha256:47cdc3490d9ac1506ce92c7aaa76c579dc3509ff11e098fc867e5130ab7be802 \
+    --hash=sha256:58da39888f92c276ad970249761ebea80ba544b77acddaa1a4d6cf78287d45fd
+    # via pydantic
 attrs==23.1.0 \
     --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
     --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
     # via
     #   jsonschema
     #   pytest-docker
 babel==2.12.1 \
@@ -37,17 +41,17 @@
     --hash=sha256:b57adba8a1444faf784394de3436233728a1ecaeb6e07e8c22c8848f179b893c \
     --hash=sha256:bf4fa8b2ca74381bb5442c089350f09a3f17797829d958fad058d6e44d9eb83c \
     --hash=sha256:ca3204d00d3cb2dfed07f2d74a25f12fc12f73e606fcaa6975d1f7ae69cacbb2 \
     --hash=sha256:cbb03eec97496166b704ed663a53680ab57c5084b2fc98ef23291987b525cb7d \
     --hash=sha256:e9a51bbfe7e9802b5f3508687758b564069ba937748ad7b9e890086290d2f79e \
     --hash=sha256:fbdaec13c5105f0c4e5c52614d04f0bca5f5af007910daa8b6b12095edaa67b3
     # via paramiko
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via
     #   -c requirements/main.txt
     #   requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
@@ -201,126 +205,135 @@
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via
     #   -c requirements/main.txt
     #   documenteer
     #   sphinx-click
-coverage[toml]==7.2.3 \
-    --hash=sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93 \
-    --hash=sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013 \
-    --hash=sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f \
-    --hash=sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21 \
-    --hash=sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462 \
-    --hash=sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc \
-    --hash=sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df \
-    --hash=sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1 \
-    --hash=sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235 \
-    --hash=sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934 \
-    --hash=sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9 \
-    --hash=sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1 \
-    --hash=sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48 \
-    --hash=sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4 \
-    --hash=sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe \
-    --hash=sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a \
-    --hash=sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b \
-    --hash=sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21 \
-    --hash=sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d \
-    --hash=sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa \
-    --hash=sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367 \
-    --hash=sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535 \
-    --hash=sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152 \
-    --hash=sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e \
-    --hash=sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539 \
-    --hash=sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1 \
-    --hash=sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925 \
-    --hash=sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0 \
-    --hash=sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2 \
-    --hash=sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab \
-    --hash=sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841 \
-    --hash=sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30 \
-    --hash=sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91 \
-    --hash=sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c \
-    --hash=sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257 \
-    --hash=sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9 \
-    --hash=sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040 \
-    --hash=sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911 \
-    --hash=sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623 \
-    --hash=sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259 \
-    --hash=sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c \
-    --hash=sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79 \
-    --hash=sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5 \
-    --hash=sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4 \
-    --hash=sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4 \
-    --hash=sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22 \
-    --hash=sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd \
-    --hash=sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1 \
-    --hash=sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910 \
-    --hash=sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859 \
-    --hash=sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312
+coverage[toml]==7.2.7 \
+    --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
+    --hash=sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2 \
+    --hash=sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a \
+    --hash=sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a \
+    --hash=sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01 \
+    --hash=sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6 \
+    --hash=sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7 \
+    --hash=sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f \
+    --hash=sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02 \
+    --hash=sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c \
+    --hash=sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063 \
+    --hash=sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a \
+    --hash=sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5 \
+    --hash=sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959 \
+    --hash=sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97 \
+    --hash=sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6 \
+    --hash=sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f \
+    --hash=sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9 \
+    --hash=sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5 \
+    --hash=sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f \
+    --hash=sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562 \
+    --hash=sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe \
+    --hash=sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9 \
+    --hash=sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f \
+    --hash=sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb \
+    --hash=sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb \
+    --hash=sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1 \
+    --hash=sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb \
+    --hash=sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250 \
+    --hash=sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e \
+    --hash=sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511 \
+    --hash=sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5 \
+    --hash=sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59 \
+    --hash=sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2 \
+    --hash=sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d \
+    --hash=sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3 \
+    --hash=sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4 \
+    --hash=sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de \
+    --hash=sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9 \
+    --hash=sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833 \
+    --hash=sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0 \
+    --hash=sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9 \
+    --hash=sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d \
+    --hash=sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050 \
+    --hash=sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d \
+    --hash=sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6 \
+    --hash=sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353 \
+    --hash=sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb \
+    --hash=sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e \
+    --hash=sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8 \
+    --hash=sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495 \
+    --hash=sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2 \
+    --hash=sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd \
+    --hash=sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27 \
+    --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
+    --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
+    --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
+    --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
+    --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
+    --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/dev.in
-cryptography==40.0.2 \
-    --hash=sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440 \
-    --hash=sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288 \
-    --hash=sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b \
-    --hash=sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958 \
-    --hash=sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b \
-    --hash=sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d \
-    --hash=sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a \
-    --hash=sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404 \
-    --hash=sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b \
-    --hash=sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e \
-    --hash=sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2 \
-    --hash=sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c \
-    --hash=sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b \
-    --hash=sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9 \
-    --hash=sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b \
-    --hash=sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636 \
-    --hash=sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99 \
-    --hash=sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e \
-    --hash=sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9
+cryptography==41.0.1 \
+    --hash=sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db \
+    --hash=sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a \
+    --hash=sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039 \
+    --hash=sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c \
+    --hash=sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3 \
+    --hash=sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485 \
+    --hash=sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c \
+    --hash=sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca \
+    --hash=sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5 \
+    --hash=sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5 \
+    --hash=sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3 \
+    --hash=sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb \
+    --hash=sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43 \
+    --hash=sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31 \
+    --hash=sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc \
+    --hash=sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b \
+    --hash=sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006 \
+    --hash=sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a \
+    --hash=sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699
     # via paramiko
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
 distro==1.8.0 \
     --hash=sha256:02e111d1dc6a50abb8eed6bf31c3e48ed8b0830d1ea2a1b78c61765c2513fdd8 \
     --hash=sha256:99522ca3e365cac527b44bde033f64c6945d90eb9f769703caaec52b09bbd3ff
     # via docker-compose
-docker[ssh]==6.0.1 \
-    --hash=sha256:896c4282e5c7af5c45e8b683b0b0c33932974fe6e50fc6906a0a83616ab3da97 \
-    --hash=sha256:dbcb3bd2fa80dca0788ed908218bf43972772009b881ed1e20dfc29a65e49782
+docker[ssh]==6.1.3 \
+    --hash=sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20 \
+    --hash=sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9
     # via docker-compose
 docker-compose==1.29.2 \
     --hash=sha256:4c8cd9d21d237412793d18bd33110049ee9af8dab3fe2c213bbd0733959b09b7 \
     --hash=sha256:8d5589373b35c8d3b1c8c1182c6e4a4ff14bffa3dd0b605fcd08f73c94cef809
     # via -r requirements/dev.in
 dockerpty==0.4.1 \
     --hash=sha256:69a9d69d573a0daa31bcd1c0774eeed5c15c295fe719c61aca550ed1393156ce
     # via docker-compose
 docopt==0.6.2 \
     --hash=sha256:49b3a825280bd66b3aa83585ef59c4a8c82f2c8a522dbe754a8bc8d08c85c491
     # via docker-compose
-documenteer[pipelines]==0.7.3 \
-    --hash=sha256:484112cdc4ec621793e5c7a6bf2c1cf7ea5544514e16eba005ef18d296a10b9d \
-    --hash=sha256:74aac4b33e0fb24a41b51e90b85a4d665c54ddc68034d674eba3847688b1b32e
+documenteer[pipelines]==0.8.2 \
+    --hash=sha256:30dcd20bb353b5389c5e7578c1eb13edc163c27cec6270bfe3c938eb51d8c164 \
+    --hash=sha256:3880ed4b8411dd15e4aae19136f0a39f305464adbaa05c8a3d5055385f7e41f9
     # via -r requirements/dev.in
 docutils==0.19 \
     --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
     --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
     # via
     #   pybtex-docutils
     #   sphinx
     #   sphinx-click
     #   sphinx-jinja
     #   sphinxcontrib-bibtex
-filelock==3.12.0 \
-    --hash=sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9 \
-    --hash=sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718
+filelock==3.12.2 \
+    --hash=sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81 \
+    --hash=sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec
     # via virtualenv
 flake8==6.0.0 \
     --hash=sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7 \
     --hash=sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181
     # via
     #   -r requirements/dev.in
     #   flake8-docstrings
@@ -336,17 +349,17 @@
     --hash=sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573 \
     --hash=sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d
     # via documenteer
 graphviz==0.20.1 \
     --hash=sha256:587c58a223b51611c0cf461132da386edd896a029524ca61a1462b880bf97977 \
     --hash=sha256:8c58f14adaa3b947daf26c19bc1e98c4e0702cdc31cf99153e6f06904d492bf8
     # via -r requirements/dev.in
-identify==2.5.22 \
-    --hash=sha256:f0faad595a4687053669c112004178149f6c326db71ee999ae4636685753ad2f \
-    --hash=sha256:f7a93d6cf98e29bd07663c60728e7a4057615068d7a639d132dc883b2d54d31e
+identify==2.5.24 \
+    --hash=sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4 \
+    --hash=sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d
     # via pre-commit
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via
     #   -c requirements/main.txt
     #   requests
@@ -375,65 +388,65 @@
     --hash=sha256:c277a193638dc7683c4c30f6684e3db728a06efb0dc9cf346db8bd0aa6c5d271
     # via pybtex
 lsst-sphinx-bootstrap-theme==0.2.2 \
     --hash=sha256:71c14b309cac280301facdd6db4fc43be9b95962e20c16bb84678fd813f2d2a1
     # via
     #   -r requirements/dev.in
     #   documenteer
-markupsafe==2.1.2 \
-    --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
-    --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
-    --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
-    --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
-    --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
-    --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
-    --hash=sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1 \
-    --hash=sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa \
-    --hash=sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03 \
-    --hash=sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323 \
-    --hash=sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65 \
-    --hash=sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013 \
-    --hash=sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036 \
-    --hash=sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f \
-    --hash=sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4 \
-    --hash=sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419 \
-    --hash=sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2 \
-    --hash=sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619 \
-    --hash=sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a \
-    --hash=sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a \
-    --hash=sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd \
-    --hash=sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7 \
-    --hash=sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666 \
-    --hash=sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65 \
-    --hash=sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859 \
-    --hash=sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625 \
-    --hash=sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff \
-    --hash=sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156 \
-    --hash=sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd \
-    --hash=sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba \
-    --hash=sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f \
-    --hash=sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1 \
-    --hash=sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094 \
-    --hash=sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a \
-    --hash=sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513 \
-    --hash=sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed \
-    --hash=sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d \
-    --hash=sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3 \
-    --hash=sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147 \
-    --hash=sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c \
-    --hash=sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603 \
-    --hash=sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601 \
-    --hash=sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a \
-    --hash=sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1 \
-    --hash=sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d \
-    --hash=sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3 \
-    --hash=sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54 \
-    --hash=sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2 \
-    --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
-    --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
+markupsafe==2.1.3 \
+    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
+    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
+    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
+    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
+    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
+    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
+    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
+    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
+    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
+    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
+    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
+    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
+    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
+    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
+    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
+    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
+    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
+    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
+    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
+    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
+    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
+    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
+    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
+    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
+    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
+    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
+    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
+    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
+    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
+    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
+    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
+    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
+    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
+    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
+    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
+    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
+    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
+    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
+    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
+    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
+    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
+    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
+    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
+    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
+    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
+    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
+    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
+    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
+    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
+    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2
     # via jinja2
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
     # via flake8
 multidict==6.0.4 \
     --hash=sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9 \
@@ -507,76 +520,76 @@
     --hash=sha256:ea20853c6dbbb53ed34cb4d080382169b6f4554d394015f1bef35e881bf83547 \
     --hash=sha256:ee2a1ece51b9b9e7752e742cfb661d2a29e7bcdba2d27e66e28a99f1890e4fa0 \
     --hash=sha256:eeb6dcc05e911516ae3d1f207d4b0520d07f54484c49dfc294d6e7d63b734171 \
     --hash=sha256:f70b98cd94886b49d91170ef23ec5c0e8ebb6f242d734ed7ed677b24d50c82cf \
     --hash=sha256:fc35cb4676846ef752816d5be2193a1e8367b4c1397b74a565a9d0389c433a1d \
     --hash=sha256:ff959bee35038c4624250473988b24f846cbeb2c6639de3602c073f10410ceba
     # via yarl
-mypy==1.2.0 \
-    --hash=sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521 \
-    --hash=sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140 \
-    --hash=sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48 \
-    --hash=sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128 \
-    --hash=sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336 \
-    --hash=sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a \
-    --hash=sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41 \
-    --hash=sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f \
-    --hash=sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e \
-    --hash=sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8 \
-    --hash=sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238 \
-    --hash=sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119 \
-    --hash=sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb \
-    --hash=sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d \
-    --hash=sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed \
-    --hash=sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9 \
-    --hash=sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e \
-    --hash=sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a \
-    --hash=sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5 \
-    --hash=sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950 \
-    --hash=sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937 \
-    --hash=sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394 \
-    --hash=sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6 \
-    --hash=sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602 \
-    --hash=sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1 \
-    --hash=sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba
+mypy==1.4.1 \
+    --hash=sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042 \
+    --hash=sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd \
+    --hash=sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2 \
+    --hash=sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01 \
+    --hash=sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7 \
+    --hash=sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3 \
+    --hash=sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816 \
+    --hash=sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3 \
+    --hash=sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc \
+    --hash=sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4 \
+    --hash=sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b \
+    --hash=sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8 \
+    --hash=sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c \
+    --hash=sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462 \
+    --hash=sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7 \
+    --hash=sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc \
+    --hash=sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258 \
+    --hash=sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b \
+    --hash=sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9 \
+    --hash=sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6 \
+    --hash=sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f \
+    --hash=sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1 \
+    --hash=sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828 \
+    --hash=sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878 \
+    --hash=sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f \
+    --hash=sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b
     # via -r requirements/dev.in
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via mypy
-nodeenv==1.7.0 \
-    --hash=sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e \
-    --hash=sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b
+nodeenv==1.8.0 \
+    --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
+    --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
     # via pre-commit
 numpydoc==1.5.0 \
     --hash=sha256:b0db7b75a32367a0e25c23b397842c65e344a1206524d16c8069f0a1c91b5f4c \
     --hash=sha256:c997759fb6fc32662801cece76491eedbc0ec619b514932ffd2b270ae89c07f9
     # via documenteer
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via
     #   docker
     #   pytest
     #   sphinx
-paramiko==3.1.0 \
-    --hash=sha256:6950faca6819acd3219d4ae694a23c7a87ee38d084f70c1724b0c0dbb8b75769 \
-    --hash=sha256:f0caa660e797d9cd10db6fc6ae81e2c9b2767af75c3180fcd0e46158cd368d7f
+paramiko==3.2.0 \
+    --hash=sha256:93cdce625a8a1dc12204439d45033f3261bdb2c201648cfcdc06f9fd0f94ec29 \
+    --hash=sha256:df0f9dd8903bc50f2e10580af687f3015bf592a377cd438d2ec9546467a14eb8
     # via docker
-platformdirs==3.2.0 \
-    --hash=sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08 \
-    --hash=sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e
+platformdirs==3.8.0 \
+    --hash=sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc \
+    --hash=sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e
     # via virtualenv
-pluggy==1.0.0 \
-    --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
-    --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
+pluggy==1.2.0 \
+    --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
+    --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
-pre-commit==3.2.2 \
-    --hash=sha256:0b4210aea813fe81144e87c5a291f09ea66f199f367fa1df41b55e1d26e1e2b4 \
-    --hash=sha256:5b808fcbda4afbccf6d6633a56663fed35b6c2bc08096fd3d47ce197ac351d9d
+pre-commit==3.3.3 \
+    --hash=sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb \
+    --hash=sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023
     # via -r requirements/dev.in
 pybtex==0.24.0 \
     --hash=sha256:818eae35b61733e5c007c3fcd2cfb75ed1bc8b4173c1f70b56cc4c0802d34755 \
     --hash=sha256:e1e0c8c69998452fea90e9179aa2a98ab103f3eed894405b7264e517cc2fcc0f
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
@@ -588,52 +601,101 @@
     --hash=sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053 \
     --hash=sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610
     # via flake8
 pycparser==2.21 \
     --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
     --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
     # via cffi
-pydantic==1.10.7 \
-    --hash=sha256:01aea3a42c13f2602b7ecbbea484a98169fb568ebd9e247593ea05f01b884b2e \
-    --hash=sha256:0cd181f1d0b1d00e2b705f1bf1ac7799a2d938cce3376b8007df62b29be3c2c6 \
-    --hash=sha256:10a86d8c8db68086f1e30a530f7d5f83eb0685e632e411dbbcf2d5c0150e8dcd \
-    --hash=sha256:193924c563fae6ddcb71d3f06fa153866423ac1b793a47936656e806b64e24ca \
-    --hash=sha256:464855a7ff7f2cc2cf537ecc421291b9132aa9c79aef44e917ad711b4a93163b \
-    --hash=sha256:516f1ed9bc2406a0467dd777afc636c7091d71f214d5e413d64fef45174cfc7a \
-    --hash=sha256:6434b49c0b03a51021ade5c4daa7d70c98f7a79e95b551201fff682fc1661245 \
-    --hash=sha256:64d34ab766fa056df49013bb6e79921a0265204c071984e75a09cbceacbbdd5d \
-    --hash=sha256:670bb4683ad1e48b0ecb06f0cfe2178dcf74ff27921cdf1606e527d2617a81ee \
-    --hash=sha256:68792151e174a4aa9e9fc1b4e653e65a354a2fa0fed169f7b3d09902ad2cb6f1 \
-    --hash=sha256:701daea9ffe9d26f97b52f1d157e0d4121644f0fcf80b443248434958fd03dc3 \
-    --hash=sha256:7d45fc99d64af9aaf7e308054a0067fdcd87ffe974f2442312372dfa66e1001d \
-    --hash=sha256:80b1fab4deb08a8292d15e43a6edccdffa5377a36a4597bb545b93e79c5ff0a5 \
-    --hash=sha256:82dffb306dd20bd5268fd6379bc4bfe75242a9c2b79fec58e1041fbbdb1f7914 \
-    --hash=sha256:8c7f51861d73e8b9ddcb9916ae7ac39fb52761d9ea0df41128e81e2ba42886cd \
-    --hash=sha256:950ce33857841f9a337ce07ddf46bc84e1c4946d2a3bba18f8280297157a3fd1 \
-    --hash=sha256:976cae77ba6a49d80f461fd8bba183ff7ba79f44aa5cfa82f1346b5626542f8e \
-    --hash=sha256:9f6f0fd68d73257ad6685419478c5aece46432f4bdd8d32c7345f1986496171e \
-    --hash=sha256:a7cd2251439988b413cb0a985c4ed82b6c6aac382dbaff53ae03c4b23a70e80a \
-    --hash=sha256:abfb7d4a7cd5cc4e1d1887c43503a7c5dd608eadf8bc615413fc498d3e4645cd \
-    --hash=sha256:ae150a63564929c675d7f2303008d88426a0add46efd76c3fc797cd71cb1b46f \
-    --hash=sha256:b0f85904f73161817b80781cc150f8b906d521fa11e3cdabae19a581c3606209 \
-    --hash=sha256:b4a849d10f211389502059c33332e91327bc154acc1845f375a99eca3afa802d \
-    --hash=sha256:c15582f9055fbc1bfe50266a19771bbbef33dd28c45e78afbe1996fd70966c2a \
-    --hash=sha256:c230c0d8a322276d6e7b88c3f7ce885f9ed16e0910354510e0bae84d54991143 \
-    --hash=sha256:cc1dde4e50a5fc1336ee0581c1612215bc64ed6d28d2c7c6f25d2fe3e7c3e918 \
-    --hash=sha256:cf135c46099ff3f919d2150a948ce94b9ce545598ef2c6c7bf55dca98a304b52 \
-    --hash=sha256:cfc83c0678b6ba51b0532bea66860617c4cd4251ecf76e9846fa5a9f3454e97e \
-    --hash=sha256:d2a5ebb48958754d386195fe9e9c5106f11275867051bf017a8059410e9abf1f \
-    --hash=sha256:d71e69699498b020ea198468e2480a2f1e7433e32a3a99760058c6520e2bea7e \
-    --hash=sha256:d75ae19d2a3dbb146b6f324031c24f8a3f52ff5d6a9f22f0683694b3afcb16fb \
-    --hash=sha256:dfe2507b8ef209da71b6fb5f4e597b50c5a34b78d7e857c4f8f3115effaef5fe \
-    --hash=sha256:e0cfe895a504c060e5d36b287ee696e2fdad02d89e0d895f83037245218a87fe \
-    --hash=sha256:e79e999e539872e903767c417c897e729e015872040e56b96e67968c3b918b2d \
-    --hash=sha256:ecbbc51391248116c0a055899e6c3e7ffbb11fb5e2a4cd6f2d0b93272118a209 \
-    --hash=sha256:f4a2b50e2b03d5776e7f21af73e2070e1b5c0d0df255a827e7c632962f8315af
+pydantic==2.0 \
+    --hash=sha256:6e313661b310eb5b2c45168ce05d8dd79f57563adaf3906162a917585576b846 \
+    --hash=sha256:8bf7355be5e1207c756dfbc8046236dadd4ce04101fb482e6c8834a06d9aa04f
     # via documenteer
+pydantic-core==2.0.1 \
+    --hash=sha256:007cdcee7e1a40951768d0d250e566b603e25d0fa8b8302901e38560bc9badf9 \
+    --hash=sha256:03d12c44decb122d5feede5408cc6c67e506b64016ce4b59c825d1a8c90f288a \
+    --hash=sha256:0872a1c52da4cfc494e23c83532c7fc1313de311a14334b7a58216a8dea828e0 \
+    --hash=sha256:0b154abef540a76bb2b7a641b3ae1e05e5c4b08eb9ad6c27a217b3c64ffcda0b \
+    --hash=sha256:0c8877d9e0bd128f103a1b0f02899aa7d4be1104eef5dc35e2b633042b64a2d1 \
+    --hash=sha256:0fcdb43190588f6219709b43ffa679e562c0d4a44a50aafb6cc88978da4a84b7 \
+    --hash=sha256:10736490eacc426d681ae6f00f1d8ce01fc77c45086a597e829c3eed127179b1 \
+    --hash=sha256:1672c8c36414c56adf704753b2d7e22e7528d7bd21cd357f24edeff76d4fd4ca \
+    --hash=sha256:16977790d69bac6034baa2349326db2ff465ad346c53b8d54c3674e05b070af2 \
+    --hash=sha256:176eb3ec03da4c36da7708d2398139e13d1130b3b3d1af4334a959f46278baa9 \
+    --hash=sha256:182a0e5ce9382a0a77aab8407ead303b6e310c673a46b18937fa1a90c22ccbc4 \
+    --hash=sha256:1bb6d1057c054056614aefeced05299d3590acf76768538b34ebec9cbbf26953 \
+    --hash=sha256:1c318bd2bdaa88ec078dc7932e108a9c43caeabc84d2cf545081fb6a99ed1b90 \
+    --hash=sha256:1c855ef11370eacff25556658fb7fa243e8c0bd4235fa20a0f473bded2ede252 \
+    --hash=sha256:3a85fde791e6567f879b50b59f1740afc55333060d93548d6bbb46bf1b6a1b49 \
+    --hash=sha256:4372e8fcb458aad1e155c04e663ff1840f36b859fb1422578372712a78866051 \
+    --hash=sha256:44c8cec1d74d74c29da59c86e8cd472851c85b44d75128096ef3751c5c87c204 \
+    --hash=sha256:46bb28295082a22f3c7f5fa5546d669aed7eb43151ec0032e8c352c59f5e36af \
+    --hash=sha256:4eda2b350b02293c7060f2371ad3ce7b00342bd61c8654d2ba374bd10c6b6b66 \
+    --hash=sha256:5e4a918eeae2c566fdcad9ee89d8708a59dc5ec3d5083b61a886b19f82f69f5c \
+    --hash=sha256:5e90b99b6aa9fd6eee6d6f86921d38252c6e55c319dc6c5e411922d0dc173825 \
+    --hash=sha256:5f3158cb4cda580f3b063b03257c7f5c2d9e66f9c2a93466c76056f7c4d5a3b7 \
+    --hash=sha256:6387c2956baf16891e7bc20d864a769c0f9f61799d4895c8f493e2de8f7b88aa \
+    --hash=sha256:659f22427d653769d1b4c672fd2daf53e639a5a93b0dd6fc0b37ef822a6e77d7 \
+    --hash=sha256:6cf3e484bc8e8c8a568d572a6619696d7e2e2aef214b0be503f0814f8bafca9f \
+    --hash=sha256:7176ffa02c45d557cceb75f1290a2ddf53da680c6878aae54e69aafb21c52efd \
+    --hash=sha256:71cf43912edeae476f47d16520e48bddbf9af0ebdd98961c38ca8944f4f22b9d \
+    --hash=sha256:722aa193ba1f587226991a789a3f098235b5f04e85cf815af9e8ad823a5a85e1 \
+    --hash=sha256:73c464afa0a959472045f242ef7cdaf6a38b76a6d7dfa1ef270de0967c04408d \
+    --hash=sha256:76d5d18ef9065ecbf62d6ec82c45ddbb47174a7400eb780040a7ebdad1c0ead8 \
+    --hash=sha256:7727a4fcb93572d4e521b028f1c64f1eda2da49d506b1a6208576faa9e0acd64 \
+    --hash=sha256:79225132aa1fe97a5e947da820b323d63372fb3475d94ff81ca6f91669717a01 \
+    --hash=sha256:7a4fc3e8c788798739f4aa6772d994e4453a17dadb1b8eea4582a31cdfe683d2 \
+    --hash=sha256:7bd78c4f04794a8e527d32c8ec1a26682b35b5c9347bb6e3cc853ba1a43c72a5 \
+    --hash=sha256:88b56a4e7480f4f22fa2faefdb0a887d70420d9cd8cb160677e8abe46769e7b0 \
+    --hash=sha256:88fc72e60d818924cb3d32948b682bcea0dadd0fd2efae9a4d0b7a55e310908a \
+    --hash=sha256:89123ab11a23fa9c332655933350dc231945ca6b1148c1e1960aad0a5a6de1c0 \
+    --hash=sha256:8927c166f20e3933cc9a9a68701acc8de22ee54b70d8c4044ad461b043b3cf9b \
+    --hash=sha256:8945ba48644b45d4e66cc3e56b896e97fb1d7f166dd0ee1eb137bbfdf1285483 \
+    --hash=sha256:8ca5a743af642700fc69dc64e0b964dd7499dcabb399e5cc2223fbc9cb33965d \
+    --hash=sha256:8daded5c64811da4bdc7d6792afa10328bff5c3514536f69457596d4a2646b49 \
+    --hash=sha256:92b01e166a3b69e8054308709acabec1bae65dae83ba6329f4fcc8448e170a06 \
+    --hash=sha256:958964a0ad0cea700b25037b21f5a2da38d19bddaa2f15ce36f51c048a9efe92 \
+    --hash=sha256:9cf1ba93657cad863d23ecb09227665c0abe26c131acd24abb5edc6249a36a70 \
+    --hash=sha256:9ee1c2d0cf5c92faf722ff366814859c764c82b30af7f91b9b1950e15efecb9e \
+    --hash=sha256:a1dd1b182fde9f95f1cc28964612fb1b180fdd3ca2cac881c108db29906b2e01 \
+    --hash=sha256:a7d0de538719feda5cabf19c63cc17345df6a0ab579b95518925d2b25276daaf \
+    --hash=sha256:aad8b177370002f73f08eafefa3d969d9c4498da6d67d8a43ffdeb4b4e560e1c \
+    --hash=sha256:ab7eafb33fdc7aa8667634be58a3d1c8ed3fa8923c6bc5014657bf95b51b4a46 \
+    --hash=sha256:ac6a57d01c0b67563dd273f2b71e9aab643573b569a202bfff7dad502b0b8ee0 \
+    --hash=sha256:adbfc6c7ddd1cca6efe62a0292cae7cf2d05c9ebb139d0da10b0d44346e253c7 \
+    --hash=sha256:adc2efaf0c45135214dff4d18d4aaf2b692249cb369f921fe0fde3a13cf7ddad \
+    --hash=sha256:ae53240f9f92f634b73a3e5ee87b9ec8ac38d5bee96ea65034af58f48d489a65 \
+    --hash=sha256:b23ae8b27b6eff72909a9a88123ac28b746d95f25927ce67d3b0f3dabe099a0a \
+    --hash=sha256:b56f3758b82f26414a4dccd76f05c768df7bd2735e0ac43f3dfff2f5603d32a9 \
+    --hash=sha256:b83e11a68936f80ee92ef1001bf6b9fedf0602396acc417b16a9c136a9b3b7bd \
+    --hash=sha256:bb2daa4e3d4efbf2e2dedc1a7cea3e48ff12d0c95ab2011e7f731bdc97d16ed0 \
+    --hash=sha256:bc99af5be239961d718bbf8e4d6bd1caa6de556e44ed08eb5135cfbefc958728 \
+    --hash=sha256:c04aa22ded4baf29c3c1ec3b76d5264dd91794b974a737251fdd0827abcc2c78 \
+    --hash=sha256:c3f8fea22690c6c33c4d36d2236732da29da560f815cd9aba1d3b5ab59dcb214 \
+    --hash=sha256:c5fef2dc7ed589ea83ac5ce526fcb8e8eb0ab79bfa67f958dafbda0a05ab3018 \
+    --hash=sha256:c656b8d4603af6744ed2f2c0be499790f0913a2186ef7214c88d47d42051ae4b \
+    --hash=sha256:c8e53bae6e58a8ff8e93f9a77440cfe8fc017bb9a8430dc03beb6bdd648572d2 \
+    --hash=sha256:cbbefd38ef80b37d056592c366a164a37b4e87b12f0aba23c35087d890fb31ba \
+    --hash=sha256:ccb06e1667a9784a96e0fc2500b989b8afbe9ac68a39a3c806c056ee228eff3c \
+    --hash=sha256:d6e21da7f7e3935b24bfd17d7c3eefe4c1edca380edaec854a8593796d8d96f1 \
+    --hash=sha256:ddb23eaf427dbbde41b543d98a0c4a7aeb73bf649e3faa75b94a2fd882a669ba \
+    --hash=sha256:ddbad540cba15b5262bd800bb6f0746a4ac719de0fe0a2acab8e0d50eb54ba9a \
+    --hash=sha256:e0dd6bb98271519a309e96e927b52f8ca1323a99762bec87cda8fdaaa221e5cd \
+    --hash=sha256:e0edd3c6762b3ff3fdbd90517a09808e5d67cce86d7c43ec6f5ca3f65bfe7fd9 \
+    --hash=sha256:e2e9025e132761e7ea8dab448923ccd8839c60199e863a6348d7e8b1a674edd1 \
+    --hash=sha256:e4785a8c5440e410394f88e30c3db862ed05841595311ddc969b3fde377f95ea \
+    --hash=sha256:e4b4c836100e5f07189b0aea8b4afae326f169bfdef91e86fd90a0d3c27f0c75 \
+    --hash=sha256:e55fc76ce657208c0d7e21e2e96925993dd4063d5c5ee9227dcdf4e550c02a29 \
+    --hash=sha256:e76a9b0c2b2fb29a80764e106b1ea35c1b96a4e62e7ce7dde44f5df153fd5b66 \
+    --hash=sha256:ef349e4ac794559c1538787a0fbce378a1beb991ef4f7707a6cde3156294259d \
+    --hash=sha256:f0f90928ed48b91d93add357fb1e81cef729bffaff3ab88882b76549434b4574 \
+    --hash=sha256:f9452d470012ee86a00a36f7673843038fd1a88661a28c72e65e7f3f084da8d8 \
+    --hash=sha256:f9fffcb5507bff84a1312d1616406cad157806f105d78bd184d1e6b3b00e6417 \
+    --hash=sha256:fa5a3d49ddbeaa80bb2a8927b90e9cdd43373616ba0b7b7a74a3ae33b5c9640c \
+    --hash=sha256:ff015389ae4ca6869a2fdd16c21ee1ce7c134503f2148efd46db643ce27ca520
+    # via pydantic
 pydocstyle==6.3.0 \
     --hash=sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019 \
     --hash=sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1
     # via flake8-docstrings
 pyflakes==3.0.1 \
     --hash=sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf \
     --hash=sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd
@@ -652,17 +714,17 @@
     --hash=sha256:52cb72a79269189d4e0dc537556f4740f7f0a9ec41c1322598799b0bdad4ef92 \
     --hash=sha256:61f642bf2378713e2c2e1de73444a3778e5f0a38be6fee0fe532fe30060282ff \
     --hash=sha256:8ac7448f09ab85811607bdd21ec2464495ac8b7c66d146bf545b0f08fb9220ba \
     --hash=sha256:a36d4a9dda1f19ce6e03c9a784a2921a4b726b02e1c736600ca9c22029474394 \
     --hash=sha256:a422368fc821589c228f4c49438a368831cb5bbc0eab5ebe1d7fac9dded6567b \
     --hash=sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543
     # via paramiko
-pyparsing==3.0.9 \
-    --hash=sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb \
-    --hash=sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc
+pyparsing==3.1.0 \
+    --hash=sha256:d554a96d1a7d3ddaf7183104485bc19fd80543ad6ac5bdb6426719d766fb06c1 \
+    --hash=sha256:edb662d6fe322d6e990b1594b5feaeadf806803359e3d4d42f11e295e588f0ea
     # via sphinxcontrib-doxylink
 pyrsistent==0.19.3 \
     --hash=sha256:016ad1afadf318eb7911baa24b049909f7f3bb2c5b1ed7b6a8f21db21ea3faa8 \
     --hash=sha256:1a2994773706bbb4995c31a97bc94f1418314923bd1048c6d964837040376440 \
     --hash=sha256:20460ac0ea439a3e79caa1dbd560344b64ed75e85d8703943e0b66c2a6150e4a \
     --hash=sha256:3311cb4237a341aa52ab8448c27e3a9931e2ee09561ad150ba94e4cfd3fc888c \
     --hash=sha256:3a8cb235fa6d3fd7aae6a4f1429bbb1fec1577d978098da1252f0489937786f3 \
@@ -685,17 +747,17 @@
     --hash=sha256:cc5d149f31706762c1f8bda2e8c4f8fead6e80312e3692619a75301d3dbb819a \
     --hash=sha256:ccf0d6bd208f8111179f0c26fdf84ed7c3891982f2edaeae7422575f47e66b64 \
     --hash=sha256:e42296a09e83028b3476f7073fcb69ffebac0e66dbbfd1bd847d61f74db30f19 \
     --hash=sha256:e8f2b814a3dc6225964fa03d8582c6e0b6650d68a232df41e3cc1b66a5d2f8d1 \
     --hash=sha256:f0774bf48631f3a20471dd7c5989657b639fd2d285b861237ea9e82c36a415a9 \
     --hash=sha256:f0e7c4b2f77593871e918be000b96c8107da48444d57005b6a6bc61fb4331b2c
     # via jsonschema
-pytest==7.3.1 \
-    --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
-    --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
     # via
     #   -r requirements/dev.in
     #   pytest-docker
     #   pytest-vcr
 pytest-docker==1.0.1 \
     --hash=sha256:5dd39b10747f166d04946ba5b2bfb64e105b692679ca7191de9869d8f8f0640b \
     --hash=sha256:f6e8a1e660e2ba63a5bd28703cbb13636e0febd4623dafe047afa8254fb9db8f
@@ -744,17 +806,17 @@
     --hash=sha256:fe69978f3f768926cfa37b867e3843918e012cf83f680806599ddce33c2c68b0
     # via
     #   docker-compose
     #   documenteer
     #   pre-commit
     #   pybtex
     #   vcrpy
-requests==2.28.2 \
-    --hash=sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa \
-    --hash=sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   -c requirements/main.txt
     #   docker
     #   docker-compose
     #   documenteer
     #   sphinx
 six==1.16.0 \
@@ -775,27 +837,29 @@
     # via gitdb
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via
     #   pydocstyle
     #   sphinx
-sphinx==6.1.3 \
-    --hash=sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2 \
-    --hash=sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc
+sphinx==6.2.1 \
+    --hash=sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b \
+    --hash=sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912
     # via
+    #   -r requirements/dev.in
     #   documenteer
     #   numpydoc
     #   sphinx-automodapi
     #   sphinx-click
     #   sphinx-jinja
     #   sphinx-prompt
     #   sphinxcontrib-autoprogram
     #   sphinxcontrib-bibtex
     #   sphinxcontrib-doxylink
+    #   sphinxcontrib-jquery
 sphinx-automodapi==0.15.0 \
     --hash=sha256:06848f261fb127b25d35f27c2c4fddb041e76498733da064504f8077cbd27bec \
     --hash=sha256:fd5871e054df7f3e299dde959afffa849f4d01c6eac274c366b06472afcb06aa
     # via
     #   -r requirements/dev.in
     #   documenteer
 sphinx-click==4.4.0 \
@@ -833,14 +897,18 @@
     --hash=sha256:2d66b357b92a08a6b0bbd871cb332a6d8fc334cdd70665b3e10c044ee43b4179 \
     --hash=sha256:8ea5a19b949a31f75e20e9e2fc13c6cbca3644817d1df2d054b497a403bbb759
     # via documenteer
 sphinxcontrib-htmlhelp==2.0.1 \
     --hash=sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff \
     --hash=sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903
     # via sphinx
+sphinxcontrib-jquery==4.1 \
+    --hash=sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a \
+    --hash=sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae
+    # via documenteer
 sphinxcontrib-jsmath==1.0.1 \
     --hash=sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178 \
     --hash=sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8
     # via sphinx
 sphinxcontrib-qthelp==1.0.3 \
     --hash=sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72 \
     --hash=sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6
@@ -849,42 +917,43 @@
     --hash=sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd \
     --hash=sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952
     # via sphinx
 texttable==1.6.7 \
     --hash=sha256:290348fb67f7746931bcdfd55ac7584ecd4e5b0846ab164333f0794b121760f2 \
     --hash=sha256:b7b68139aa8a6339d2c320ca8b1dc42d13a7831a346b446cb9eb385f0c76310c
     # via docker-compose
-types-requests==2.28.11.17 \
-    --hash=sha256:0d580652ce903f643f8c3b494dd01d29367ea57cea0c7ad7f65cf3169092edb0 \
-    --hash=sha256:cc1aba862575019306b2ed134eb1ea994cab1c887a22e18d3383e6dd42e9789b
+types-requests==2.31.0.1 \
+    --hash=sha256:3de667cffa123ce698591de0ad7db034a5317457a596eb0b4944e5a9d9e8d1ac \
+    --hash=sha256:afb06ef8f25ba83d59a1d424bd7a5a939082f94b94e90ab5e6116bd2559deaa3
     # via -r requirements/dev.in
-types-urllib3==1.26.25.10 \
-    --hash=sha256:12c744609d588340a07e45d333bf870069fc8793bcf96bae7a96d4712a42591d \
-    --hash=sha256:c44881cde9fc8256d05ad6b21f50c4681eb20092552351570ab0a8a0653286d6
+types-urllib3==1.26.25.13 \
+    --hash=sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5 \
+    --hash=sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c
     # via types-requests
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via
     #   mypy
     #   pydantic
-urllib3==1.26.15 \
-    --hash=sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305 \
-    --hash=sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42
+    #   pydantic-core
+urllib3==2.0.3 \
+    --hash=sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1 \
+    --hash=sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825
     # via
     #   -c requirements/main.txt
     #   docker
     #   requests
-vcrpy==4.2.1 \
-    --hash=sha256:7cd3e81a2c492e01c281f180bcc2a86b520b173d2b656cb5d89d99475423e013 \
-    --hash=sha256:efac3e2e0b2af7686f83a266518180af7a048619b2f696e7bad9520f5e2eac09
+vcrpy==5.0.0 \
+    --hash=sha256:1ef3ddea819a26eda10b560c70bd74c41855241d431745712e31a5b2de2d05a8 \
+    --hash=sha256:28b66c87be7678896e9e78fee4f6695e3fb153d5d7e5f635416a33658452bb44
     # via pytest-vcr
-virtualenv==20.21.0 \
-    --hash=sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc \
-    --hash=sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68
+virtualenv==20.23.1 \
+    --hash=sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419 \
+    --hash=sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1
     # via pre-commit
 websocket-client==0.59.0 \
     --hash=sha256:2e50d26ca593f70aba7b13a489435ef88b8fc3b5c5643c1ce8808ff9b40f0b32 \
     --hash=sha256:d376bd60eace9d437ab6d7ee16f4ab4e821c9dae591e1b783c58ebd8aaf80c5c
     # via
     #   docker
     #   docker-compose
@@ -961,91 +1030,91 @@
     --hash=sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29 \
     --hash=sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6 \
     --hash=sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034 \
     --hash=sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09 \
     --hash=sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559 \
     --hash=sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639
     # via vcrpy
-yarl==1.8.2 \
-    --hash=sha256:009a028127e0a1755c38b03244c0bea9d5565630db9c4cf9572496e947137a87 \
-    --hash=sha256:0414fd91ce0b763d4eadb4456795b307a71524dbacd015c657bb2a39db2eab89 \
-    --hash=sha256:0978f29222e649c351b173da2b9b4665ad1feb8d1daa9d971eb90df08702668a \
-    --hash=sha256:0ef8fb25e52663a1c85d608f6dd72e19bd390e2ecaf29c17fb08f730226e3a08 \
-    --hash=sha256:10b08293cda921157f1e7c2790999d903b3fd28cd5c208cf8826b3b508026996 \
-    --hash=sha256:1684a9bd9077e922300ecd48003ddae7a7474e0412bea38d4631443a91d61077 \
-    --hash=sha256:1b372aad2b5f81db66ee7ec085cbad72c4da660d994e8e590c997e9b01e44901 \
-    --hash=sha256:1e21fb44e1eff06dd6ef971d4bdc611807d6bd3691223d9c01a18cec3677939e \
-    --hash=sha256:2305517e332a862ef75be8fad3606ea10108662bc6fe08509d5ca99503ac2aee \
-    --hash=sha256:24ad1d10c9db1953291f56b5fe76203977f1ed05f82d09ec97acb623a7976574 \
-    --hash=sha256:272b4f1599f1b621bf2aabe4e5b54f39a933971f4e7c9aa311d6d7dc06965165 \
-    --hash=sha256:2a1fca9588f360036242f379bfea2b8b44cae2721859b1c56d033adfd5893634 \
-    --hash=sha256:2b4fa2606adf392051d990c3b3877d768771adc3faf2e117b9de7eb977741229 \
-    --hash=sha256:3150078118f62371375e1e69b13b48288e44f6691c1069340081c3fd12c94d5b \
-    --hash=sha256:326dd1d3caf910cd26a26ccbfb84c03b608ba32499b5d6eeb09252c920bcbe4f \
-    --hash=sha256:34c09b43bd538bf6c4b891ecce94b6fa4f1f10663a8d4ca589a079a5018f6ed7 \
-    --hash=sha256:388a45dc77198b2460eac0aca1efd6a7c09e976ee768b0d5109173e521a19daf \
-    --hash=sha256:3adeef150d528ded2a8e734ebf9ae2e658f4c49bf413f5f157a470e17a4a2e89 \
-    --hash=sha256:3edac5d74bb3209c418805bda77f973117836e1de7c000e9755e572c1f7850d0 \
-    --hash=sha256:3f6b4aca43b602ba0f1459de647af954769919c4714706be36af670a5f44c9c1 \
-    --hash=sha256:3fc056e35fa6fba63248d93ff6e672c096f95f7836938241ebc8260e062832fe \
-    --hash=sha256:418857f837347e8aaef682679f41e36c24250097f9e2f315d39bae3a99a34cbf \
-    --hash=sha256:42430ff511571940d51e75cf42f1e4dbdded477e71c1b7a17f4da76c1da8ea76 \
-    --hash=sha256:44ceac0450e648de86da8e42674f9b7077d763ea80c8ceb9d1c3e41f0f0a9951 \
-    --hash=sha256:47d49ac96156f0928f002e2424299b2c91d9db73e08c4cd6742923a086f1c863 \
-    --hash=sha256:48dd18adcf98ea9cd721a25313aef49d70d413a999d7d89df44f469edfb38a06 \
-    --hash=sha256:49d43402c6e3013ad0978602bf6bf5328535c48d192304b91b97a3c6790b1562 \
-    --hash=sha256:4d04acba75c72e6eb90745447d69f84e6c9056390f7a9724605ca9c56b4afcc6 \
-    --hash=sha256:57a7c87927a468e5a1dc60c17caf9597161d66457a34273ab1760219953f7f4c \
-    --hash=sha256:58a3c13d1c3005dbbac5c9f0d3210b60220a65a999b1833aa46bd6677c69b08e \
-    --hash=sha256:5df5e3d04101c1e5c3b1d69710b0574171cc02fddc4b23d1b2813e75f35a30b1 \
-    --hash=sha256:63243b21c6e28ec2375f932a10ce7eda65139b5b854c0f6b82ed945ba526bff3 \
-    --hash=sha256:64dd68a92cab699a233641f5929a40f02a4ede8c009068ca8aa1fe87b8c20ae3 \
-    --hash=sha256:6604711362f2dbf7160df21c416f81fac0de6dbcf0b5445a2ef25478ecc4c778 \
-    --hash=sha256:6c4fcfa71e2c6a3cb568cf81aadc12768b9995323186a10827beccf5fa23d4f8 \
-    --hash=sha256:6d88056a04860a98341a0cf53e950e3ac9f4e51d1b6f61a53b0609df342cc8b2 \
-    --hash=sha256:705227dccbe96ab02c7cb2c43e1228e2826e7ead880bb19ec94ef279e9555b5b \
-    --hash=sha256:728be34f70a190566d20aa13dc1f01dc44b6aa74580e10a3fb159691bc76909d \
-    --hash=sha256:74dece2bfc60f0f70907c34b857ee98f2c6dd0f75185db133770cd67300d505f \
-    --hash=sha256:75c16b2a900b3536dfc7014905a128a2bea8fb01f9ee26d2d7d8db0a08e7cb2c \
-    --hash=sha256:77e913b846a6b9c5f767b14dc1e759e5aff05502fe73079f6f4176359d832581 \
-    --hash=sha256:7a66c506ec67eb3159eea5096acd05f5e788ceec7b96087d30c7d2865a243918 \
-    --hash=sha256:8c46d3d89902c393a1d1e243ac847e0442d0196bbd81aecc94fcebbc2fd5857c \
-    --hash=sha256:93202666046d9edadfe9f2e7bf5e0782ea0d497b6d63da322e541665d65a044e \
-    --hash=sha256:97209cc91189b48e7cfe777237c04af8e7cc51eb369004e061809bcdf4e55220 \
-    --hash=sha256:a48f4f7fea9a51098b02209d90297ac324241bf37ff6be6d2b0149ab2bd51b37 \
-    --hash=sha256:a783cd344113cb88c5ff7ca32f1f16532a6f2142185147822187913eb989f739 \
-    --hash=sha256:ae0eec05ab49e91a78700761777f284c2df119376e391db42c38ab46fd662b77 \
-    --hash=sha256:ae4d7ff1049f36accde9e1ef7301912a751e5bae0a9d142459646114c70ecba6 \
-    --hash=sha256:b05df9ea7496df11b710081bd90ecc3a3db6adb4fee36f6a411e7bc91a18aa42 \
-    --hash=sha256:baf211dcad448a87a0d9047dc8282d7de59473ade7d7fdf22150b1d23859f946 \
-    --hash=sha256:bb81f753c815f6b8e2ddd2eef3c855cf7da193b82396ac013c661aaa6cc6b0a5 \
-    --hash=sha256:bcd7bb1e5c45274af9a1dd7494d3c52b2be5e6bd8d7e49c612705fd45420b12d \
-    --hash=sha256:bf071f797aec5b96abfc735ab97da9fd8f8768b43ce2abd85356a3127909d146 \
-    --hash=sha256:c15163b6125db87c8f53c98baa5e785782078fbd2dbeaa04c6141935eb6dab7a \
-    --hash=sha256:cb6d48d80a41f68de41212f3dfd1a9d9898d7841c8f7ce6696cf2fd9cb57ef83 \
-    --hash=sha256:ceff9722e0df2e0a9e8a79c610842004fa54e5b309fe6d218e47cd52f791d7ef \
-    --hash=sha256:cfa2bbca929aa742b5084fd4663dd4b87c191c844326fcb21c3afd2d11497f80 \
-    --hash=sha256:d617c241c8c3ad5c4e78a08429fa49e4b04bedfc507b34b4d8dceb83b4af3588 \
-    --hash=sha256:d881d152ae0007809c2c02e22aa534e702f12071e6b285e90945aa3c376463c5 \
-    --hash=sha256:da65c3f263729e47351261351b8679c6429151ef9649bba08ef2528ff2c423b2 \
-    --hash=sha256:de986979bbd87272fe557e0a8fcb66fd40ae2ddfe28a8b1ce4eae22681728fef \
-    --hash=sha256:df60a94d332158b444301c7f569659c926168e4d4aad2cfbf4bce0e8fb8be826 \
-    --hash=sha256:dfef7350ee369197106805e193d420b75467b6cceac646ea5ed3049fcc950a05 \
-    --hash=sha256:e59399dda559688461762800d7fb34d9e8a6a7444fd76ec33220a926c8be1516 \
-    --hash=sha256:e6f3515aafe0209dd17fb9bdd3b4e892963370b3de781f53e1746a521fb39fc0 \
-    --hash=sha256:e7fd20d6576c10306dea2d6a5765f46f0ac5d6f53436217913e952d19237efc4 \
-    --hash=sha256:ebb78745273e51b9832ef90c0898501006670d6e059f2cdb0e999494eb1450c2 \
-    --hash=sha256:efff27bd8cbe1f9bd127e7894942ccc20c857aa8b5a0327874f30201e5ce83d0 \
-    --hash=sha256:f37db05c6051eff17bc832914fe46869f8849de5b92dc4a3466cd63095d23dfd \
-    --hash=sha256:f8ca8ad414c85bbc50f49c0a106f951613dfa5f948ab69c10ce9b128d368baf8 \
-    --hash=sha256:fb742dcdd5eec9f26b61224c23baea46c9055cf16f62475e11b9b15dfd5c117b \
-    --hash=sha256:fc77086ce244453e074e445104f0ecb27530d6fd3a46698e33f6c38951d5a0f1 \
-    --hash=sha256:ff205b58dc2929191f68162633d5e10e8044398d7a45265f90a0f1d51f85f72c
+yarl==1.9.2 \
+    --hash=sha256:04ab9d4b9f587c06d801c2abfe9317b77cdf996c65a90d5e84ecc45010823571 \
+    --hash=sha256:066c163aec9d3d073dc9ffe5dd3ad05069bcb03fcaab8d221290ba99f9f69ee3 \
+    --hash=sha256:13414591ff516e04fcdee8dc051c13fd3db13b673c7a4cb1350e6b2ad9639ad3 \
+    --hash=sha256:149ddea5abf329752ea5051b61bd6c1d979e13fbf122d3a1f9f0c8be6cb6f63c \
+    --hash=sha256:159d81f22d7a43e6eabc36d7194cb53f2f15f498dbbfa8edc8a3239350f59fe7 \
+    --hash=sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04 \
+    --hash=sha256:22a94666751778629f1ec4280b08eb11815783c63f52092a5953faf73be24191 \
+    --hash=sha256:2a96c19c52ff442a808c105901d0bdfd2e28575b3d5f82e2f5fd67e20dc5f4ea \
+    --hash=sha256:2b0738fb871812722a0ac2154be1f049c6223b9f6f22eec352996b69775b36d4 \
+    --hash=sha256:2c315df3293cd521033533d242d15eab26583360b58f7ee5d9565f15fee1bef4 \
+    --hash=sha256:32f1d071b3f362c80f1a7d322bfd7b2d11e33d2adf395cc1dd4df36c9c243095 \
+    --hash=sha256:3458a24e4ea3fd8930e934c129b676c27452e4ebda80fbe47b56d8c6c7a63a9e \
+    --hash=sha256:38a3928ae37558bc1b559f67410df446d1fbfa87318b124bf5032c31e3447b74 \
+    --hash=sha256:3da8a678ca8b96c8606bbb8bfacd99a12ad5dd288bc6f7979baddd62f71c63ef \
+    --hash=sha256:494053246b119b041960ddcd20fd76224149cfea8ed8777b687358727911dd33 \
+    --hash=sha256:50f33040f3836e912ed16d212f6cc1efb3231a8a60526a407aeb66c1c1956dde \
+    --hash=sha256:52a25809fcbecfc63ac9ba0c0fb586f90837f5425edfd1ec9f3372b119585e45 \
+    --hash=sha256:53338749febd28935d55b41bf0bcc79d634881195a39f6b2f767870b72514caf \
+    --hash=sha256:5415d5a4b080dc9612b1b63cba008db84e908b95848369aa1da3686ae27b6d2b \
+    --hash=sha256:5610f80cf43b6202e2c33ba3ec2ee0a2884f8f423c8f4f62906731d876ef4fac \
+    --hash=sha256:566185e8ebc0898b11f8026447eacd02e46226716229cea8db37496c8cdd26e0 \
+    --hash=sha256:56ff08ab5df8429901ebdc5d15941b59f6253393cb5da07b4170beefcf1b2528 \
+    --hash=sha256:59723a029760079b7d991a401386390c4be5bfec1e7dd83e25a6a0881859e716 \
+    --hash=sha256:5fcd436ea16fee7d4207c045b1e340020e58a2597301cfbcfdbe5abd2356c2fb \
+    --hash=sha256:61016e7d582bc46a5378ffdd02cd0314fb8ba52f40f9cf4d9a5e7dbef88dee18 \
+    --hash=sha256:63c48f6cef34e6319a74c727376e95626f84ea091f92c0250a98e53e62c77c72 \
+    --hash=sha256:646d663eb2232d7909e6601f1a9107e66f9791f290a1b3dc7057818fe44fc2b6 \
+    --hash=sha256:662e6016409828ee910f5d9602a2729a8a57d74b163c89a837de3fea050c7582 \
+    --hash=sha256:674ca19cbee4a82c9f54e0d1eee28116e63bc6fd1e96c43031d11cbab8b2afd5 \
+    --hash=sha256:6a5883464143ab3ae9ba68daae8e7c5c95b969462bbe42e2464d60e7e2698368 \
+    --hash=sha256:6e7221580dc1db478464cfeef9b03b95c5852cc22894e418562997df0d074ccc \
+    --hash=sha256:75df5ef94c3fdc393c6b19d80e6ef1ecc9ae2f4263c09cacb178d871c02a5ba9 \
+    --hash=sha256:783185c75c12a017cc345015ea359cc801c3b29a2966c2655cd12b233bf5a2be \
+    --hash=sha256:822b30a0f22e588b32d3120f6d41e4ed021806418b4c9f0bc3048b8c8cb3f92a \
+    --hash=sha256:8288d7cd28f8119b07dd49b7230d6b4562f9b61ee9a4ab02221060d21136be80 \
+    --hash=sha256:82aa6264b36c50acfb2424ad5ca537a2060ab6de158a5bd2a72a032cc75b9eb8 \
+    --hash=sha256:832b7e711027c114d79dffb92576acd1bd2decc467dec60e1cac96912602d0e6 \
+    --hash=sha256:838162460b3a08987546e881a2bfa573960bb559dfa739e7800ceeec92e64417 \
+    --hash=sha256:83fcc480d7549ccebe9415d96d9263e2d4226798c37ebd18c930fce43dfb9574 \
+    --hash=sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59 \
+    --hash=sha256:891c0e3ec5ec881541f6c5113d8df0315ce5440e244a716b95f2525b7b9f3608 \
+    --hash=sha256:8c2ad583743d16ddbdf6bb14b5cd76bf43b0d0006e918809d5d4ddf7bde8dd82 \
+    --hash=sha256:8c56986609b057b4839968ba901944af91b8e92f1725d1a2d77cbac6972b9ed1 \
+    --hash=sha256:8ea48e0a2f931064469bdabca50c2f578b565fc446f302a79ba6cc0ee7f384d3 \
+    --hash=sha256:8ec53a0ea2a80c5cd1ab397925f94bff59222aa3cf9c6da938ce05c9ec20428d \
+    --hash=sha256:95d2ecefbcf4e744ea952d073c6922e72ee650ffc79028eb1e320e732898d7e8 \
+    --hash=sha256:9b3152f2f5677b997ae6c804b73da05a39daa6a9e85a512e0e6823d81cdad7cc \
+    --hash=sha256:9bf345c3a4f5ba7f766430f97f9cc1320786f19584acc7086491f45524a551ac \
+    --hash=sha256:a60347f234c2212a9f0361955007fcf4033a75bf600a33c88a0a8e91af77c0e8 \
+    --hash=sha256:a74dcbfe780e62f4b5a062714576f16c2f3493a0394e555ab141bf0d746bb955 \
+    --hash=sha256:a83503934c6273806aed765035716216cc9ab4e0364f7f066227e1aaea90b8d0 \
+    --hash=sha256:ac9bb4c5ce3975aeac288cfcb5061ce60e0d14d92209e780c93954076c7c4367 \
+    --hash=sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb \
+    --hash=sha256:b03917871bf859a81ccb180c9a2e6c1e04d2f6a51d953e6a5cdd70c93d4e5a2a \
+    --hash=sha256:b124e2a6d223b65ba8768d5706d103280914d61f5cae3afbc50fc3dfcc016623 \
+    --hash=sha256:b25322201585c69abc7b0e89e72790469f7dad90d26754717f3310bfe30331c2 \
+    --hash=sha256:b7232f8dfbd225d57340e441d8caf8652a6acd06b389ea2d3222b8bc89cbfca6 \
+    --hash=sha256:b8cc1863402472f16c600e3e93d542b7e7542a540f95c30afd472e8e549fc3f7 \
+    --hash=sha256:b9a4e67ad7b646cd6f0938c7ebfd60e481b7410f574c560e455e938d2da8e0f4 \
+    --hash=sha256:be6b3fdec5c62f2a67cb3f8c6dbf56bbf3f61c0f046f84645cd1ca73532ea051 \
+    --hash=sha256:bf74d08542c3a9ea97bb8f343d4fcbd4d8f91bba5ec9d5d7f792dbe727f88938 \
+    --hash=sha256:c027a6e96ef77d401d8d5a5c8d6bc478e8042f1e448272e8d9752cb0aff8b5c8 \
+    --hash=sha256:c0c77533b5ed4bcc38e943178ccae29b9bcf48ffd1063f5821192f23a1bd27b9 \
+    --hash=sha256:c1012fa63eb6c032f3ce5d2171c267992ae0c00b9e164efe4d73db818465fac3 \
+    --hash=sha256:c3a53ba34a636a256d767c086ceb111358876e1fb6b50dfc4d3f4951d40133d5 \
+    --hash=sha256:d4e2c6d555e77b37288eaf45b8f60f0737c9efa3452c6c44626a5455aeb250b9 \
+    --hash=sha256:de119f56f3c5f0e2fb4dee508531a32b069a5f2c6e827b272d1e0ff5ac040333 \
+    --hash=sha256:e65610c5792870d45d7b68c677681376fcf9cc1c289f23e8e8b39c1485384185 \
+    --hash=sha256:e9fdc7ac0d42bc3ea78818557fab03af6181e076a2944f43c38684b4b6bed8e3 \
+    --hash=sha256:ee4afac41415d52d53a9833ebae7e32b344be72835bbb589018c9e938045a560 \
+    --hash=sha256:f364d3480bffd3aa566e886587eaca7c8c04d74f6e8933f3f2c996b7f09bee1b \
+    --hash=sha256:f3b078dbe227f79be488ffcfc7a9edb3409d018e0952cf13f15fd6512847f3f7 \
+    --hash=sha256:f4e2d08f07a3d7d3e12549052eb5ad3eab1c349c53ac51c209a0e5991bbada78 \
+    --hash=sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7
     # via vcrpy
 
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==67.6.1 \
-    --hash=sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a \
-    --hash=sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078
+setuptools==68.0.0 \
+    --hash=sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f \
+    --hash=sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235
     # via
     #   jsonschema
     #   nodeenv
```

### Comparing `kafkaconnect-1.2.0/requirements/main.txt` & `kafkaconnect-1.3.0/requirements/main.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/main.txt requirements/main.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/main.txt requirements/main.in
 #
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via requests
 charset-normalizer==3.1.0 \
     --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
     --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
     --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
     --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
     --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
@@ -85,50 +85,50 @@
     --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
     --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via -r requirements/main.in
-confluent-kafka==2.1.0 \
-    --hash=sha256:003bab03e35bbcfa11b5aa17c99d7c46cf10ce526420e8527b80a15eb0b25ff7 \
-    --hash=sha256:075521da9b7b35a8d57f1dc7a34ef38643c3cb21db39561cf28cf60e548e4835 \
-    --hash=sha256:0ccdea96b5fb47deb965bec87371dc7abda46ff705ebcfc238c1afaa69ebd919 \
-    --hash=sha256:1587a279603f19aa3a4ad3c861495dc3519601bd47152587d6a854172bbef3a7 \
-    --hash=sha256:1da000702d3bd29ac28a11660f45b8fa86210c650cc1f10799e26d201501d1b2 \
-    --hash=sha256:3f8b01b1cbbe456dbe663a2517b040bce83fef5e246fc44c6e5d9a163871ee78 \
-    --hash=sha256:42ee096c53bf7d829b311189ef01ea7793a3f1c1538688d78e5a6a17f75f27f1 \
-    --hash=sha256:57dd5b0dfef8272a3ce28ba404ae1833cc10c72c5779d03363f6b9a4b7862ef5 \
-    --hash=sha256:5ec9e49084b8706564f210466f4aa6041b4d1abf30bca5844b58e11bb315ef54 \
-    --hash=sha256:6fc7bb716c675779c675dda460f6df5686b153573f603976dd392bf8fca321e2 \
-    --hash=sha256:719dcee6a634269105c8c80f1746032fdf247caebcd66f1c4e821b07c0648898 \
-    --hash=sha256:7d05de0d4b16f2a4f3ff4780ffd556259e594a35a227877b1ab033cafdbf8028 \
-    --hash=sha256:7ebabc9cc488d5652dbf9ba28e149b5396c5eb5025792c7a6ae01dbf17ae8b37 \
-    --hash=sha256:8a805d5ffdc4830b37e24fed6465b8df02da7ea4e51571e4399a358cb7a381e7 \
-    --hash=sha256:91ce9aa799b1e7ba0bb03d06e134d3dfb49e4a62cc21b3708b47ce2caecc5e31 \
-    --hash=sha256:a1b9443a286d31c697170c2b628da0a1c82514f6349c06f14daca81a073d6742 \
-    --hash=sha256:a1f3922ce82edb75d84b534d11c4fc099f91d2099bb8f2050d0ab83273590bf6 \
-    --hash=sha256:abdb9642f34d624616d3aa038eff8038a9122e4de7c7c43a46d2f6c4a1d8a323 \
-    --hash=sha256:aff22487d2ac556cb1fa6801e3410d23caba8b91e0e5b705683c1039588e150c \
-    --hash=sha256:b25e28ca874db98f16bf8795771da966ba851e865773d82b8a7fd319bcb0dcd9 \
-    --hash=sha256:b36aa1b8dad3f713ab7e03d5077d858960734066b374f971c70f4cc5b9ed9a48 \
-    --hash=sha256:bf9bb0c55614e1f821c74856039b287eb2f1d3e831ef912a2375e4a72845b370 \
-    --hash=sha256:ca9a936f2ed06b5258a010673c1dbac91e6ba8e0ddbb737091a572615f70f5a4 \
-    --hash=sha256:cae2739684258384f9fe20eb38ccae53efdf80f02ee1acd1dfe1434cc7bcd397 \
-    --hash=sha256:d092153123ced45189b6190599760da3964870686c2046342ebf1f6f5a881025 \
-    --hash=sha256:d1740730d5f664a425ad4c79ffacbb614a67915f3a28fe461e656a6c7b4be551 \
-    --hash=sha256:d57675cdbf89f20fd50cbcec76d0eb0ed9efac70d8a5b08dbd72d6724f81100b \
-    --hash=sha256:e22d0d2383ff5fcdc89816ff120ccfcc0b313711e509a96a74e6b16c20eb68cd \
-    --hash=sha256:f87dd325a61726070a447c5f73901c7c2208c77c5a8d92bf7738560196dc0d09
+confluent-kafka==2.1.1 \
+    --hash=sha256:09c6c44b484c75e88aad802b0433793969218af925d0b9fed4caae704fcd01d6 \
+    --hash=sha256:1cb88bd70cfc191cc81f6164f1f898f8bf2ec501ab7abb03629102b62b706c8a \
+    --hash=sha256:22c88b63dded4c4b71e1e704f04c7209c8e04938b050e399b1883e3411899fe6 \
+    --hash=sha256:326ec2261d994d2cede682d6015d5a10f188d82f0bff9c895e07e59b9e227138 \
+    --hash=sha256:369dfd5d8cd84cf1d9355054e0f2c9e9b8cf3877aeab4a85aec8909e775ae4c2 \
+    --hash=sha256:4767e049c7d76e73b3c9fc036fcab24f1cff79b98c55d78b06edb4354b6e59c1 \
+    --hash=sha256:50b80f7ed6a187f3b3b109ccbf89c4ddf16280c5717d8ee25cd9fac001baae7a \
+    --hash=sha256:51d02f06e67a316d0c4a2cd939bef925ee87488eef78f63e5a054b1b3c5c4431 \
+    --hash=sha256:58126c36afea4c0de58342c5da3c4de2ce46b0951f3c8addb50f9ab340bddb39 \
+    --hash=sha256:5de086a2e607f73ecab9d49b8d1c2adc2ed6a328e4087996f16742acc69062b8 \
+    --hash=sha256:7a6eb7aaced82bf0f99702e76829dfe0d318a5c504bd6a6c36a63737e4b6ff36 \
+    --hash=sha256:7fbaeaf4d236dd62b2822bdd48f276a8b39adc0987d021874368a69ac3b78fab \
+    --hash=sha256:82322e774f307d7fce236a47ced2830a92a43f98194c1d2a277b366587def382 \
+    --hash=sha256:82e286f573904e141f4e56add54f35f6f407713e329a344e0589443591c68481 \
+    --hash=sha256:9069cf9190d121e7a479dde2eb0b89f7f62aeb7ac48d56d28d7d4bc20689c233 \
+    --hash=sha256:a665e74030a85c5f4203538cfe77e401133a849c4b92052a60225b26052a7e9d \
+    --hash=sha256:a91c34aa8f3e4d095f5ed9f5cd7edf1217bed9bb69da412efd8541ace3683860 \
+    --hash=sha256:b517bcd0cbe88abbad60a1a6176f1c8db45d512f109b1a65f0110af4d92aba7c \
+    --hash=sha256:bea62d091cc38a305ab877b349931ae69064b9ea50f350d9f91a86d01b10d85c \
+    --hash=sha256:c378b7d01ea1f4b2fc587ccd6f17059b1afd2d39489de797e0df87ec25ab8a67 \
+    --hash=sha256:c5ce525dbccabbf8cd0f0df975237e5c823a286b9a853fdeac8141336c29b4ef \
+    --hash=sha256:c906bb753381c809dbd8576507ff3410193f8edb28a63caef85ccd0f85996b4d \
+    --hash=sha256:ca305c3256f7943ff0127d5e9797f7e4c314838232749db4ac8920552c38c0dd \
+    --hash=sha256:cb3c81563fcc9071ae799529a7a1a3aa8fb4d94770222aaa811b3e2a54e87f8a \
+    --hash=sha256:cb7b2f61db54f4b16609273f42c19fb05d69f44df5af8eaeff7cc502a9b8ff8f \
+    --hash=sha256:d673820d3473406fbd30e0a38d6fbd6b7b5a6a0db36ca2c1b4a7d5b9bc079dd1 \
+    --hash=sha256:dac1be768ece728ca9a15933a2f6c8184a4f0854d81a22302c90a222ec8ca55a \
+    --hash=sha256:e30ece4692355cc61b0acfe70d319c6ed4e38110e9b16c82619b46b58485f16b \
+    --hash=sha256:f37cdeacb94a1c43b8bc5dddbe44b0bd72b932b906597ad62795cd43ef5aa6b8
     # via -r requirements/main.in
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
-requests==2.28.2 \
-    --hash=sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa \
-    --hash=sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via -r requirements/main.in
-urllib3==1.26.15 \
-    --hash=sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305 \
-    --hash=sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42
+urllib3==2.0.3 \
+    --hash=sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1 \
+    --hash=sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825
     # via requests
```

### Comparing `kafkaconnect-1.2.0/scripts/install-base-packages.sh` & `kafkaconnect-1.3.0/scripts/install-base-packages.sh`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/setup.cfg` & `kafkaconnect-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/cli.py` & `kafkaconnect-1.3.0/src/kafkaconnect/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/config.py` & `kafkaconnect-1.3.0/src/kafkaconnect/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,16 +46,19 @@
 
 
 @dataclass
 class ConnectorConfig(ABC):
     """Connector configuration interface."""
 
     @abstractmethod
-    def update_topics(self, topics: Set[str]) -> None:
-        """update_topics() abstract method to override."""
+    def update_config(self, topics: Set[str]) -> None:
+        """Update connector configuration.
+
+        Abstract method to be implemented by subclasses.
+        """
         pass
 
     @staticmethod
     def format_field_names(fields: List[Tuple[str, Any]]) -> Dict[str, str]:
         """Rename a field name by replacing '_' with '.'.
 
         Dictionary factory used with the dataclasses.asdict() method.
```

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/connect.py` & `kafkaconnect-1.3.0/src/kafkaconnect/connect.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/influxdb_sink/cli.py` & `kafkaconnect-1.3.0/src/kafkaconnect/influxdb_sink/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,14 +215,22 @@
     "--tags",
     "tags",
     envvar="KAFKA_CONNECT_INFLUXDB_TAGS",
     default="",
     show_default=True,
     help="Fields in the Avro payload that are treated as InfluxDB tags.",
 )
+@click.option(
+    "--remove-prefix",
+    "remove_prefix",
+    envvar="KAFKA_CONNECT_INFLUXDB_REMOVE_PREFIX",
+    default="",
+    show_default=True,
+    help="Prefix to remove from topic name to use as measurement name.",
+)
 @click.pass_context
 def create_influxdb_sink(
     ctx: click.Context,
     topiclist: tuple,
     name: str,
     connect_influx_url: str,
     connect_influx_db: str,
@@ -237,14 +245,15 @@
     excluded_topic_regex: str,
     connect_influx_error_policy: str,
     connect_influx_max_retries: str,
     connect_influx_retry_interval: str,
     connect_progress_enabled: str,
     timestamp: str,
     tags: str,
+    remove_prefix: str,
 ) -> int:
     """Create an instance of the InfluxDB Sink connector.
 
     A list of topics can be specified using the TOPICLIST argument.
     If not, topics are discovered from Kafka. Use the ``--topic-regex`` and
     ``--excluded_topics`` options to help in selecting the topics
     that you want to write to InfluxDB. To check for new topics and update
@@ -263,27 +272,28 @@
         connect_influx_username=connect_influx_username,
         connect_influx_password=connect_influx_password,
         connect_influx_error_policy=connect_influx_error_policy,
         connect_influx_max_retries=connect_influx_max_retries,
         connect_influx_retry_interval=connect_influx_retry_interval,
         connect_progress_enabled=(connect_progress_enabled == "true"),
         tags=tags,
+        remove_prefix=remove_prefix,
     )
     # The variadic argument is a tuple
     topics: Set[str] = set(topiclist)
     if not topics:
         click.echo("Discoverying Kafka topics...")
         t = TopicNamesSet.from_kafka(config, topic_regex, excluded_topic_regex)
         topics = t.topic_names_set
         n = 0 if not topics else len(topics)
         click.echo(f"Found {n} topics.")
     connect = Connect(connect_url=config.connect_url)
     if topics:
-        influx_config.update_topics(topics, timestamp)
-        # --validate option
+        influx_config.update_config(topics, timestamp)
+        # --validate option returns the validation results
         if validate:
             click.echo(
                 connect.validate(
                     name=influx_config.connector_class,
                     connect_config=influx_config.asjson(),
                 )
             )
@@ -321,15 +331,15 @@
                 t = TopicNamesSet.from_kafka(
                     config, topic_regex, excluded_topic_regex
                 )
                 current_topics = t.topic_names_set
                 new_topics = list(set(current_topics) - set(topics))
                 if new_topics:
                     click.echo("Found new topics, updating the connector...")
-                    influx_config.update_topics(current_topics, timestamp)
+                    influx_config.update_config(current_topics, timestamp)
                     connect.create_or_update(
                         name=name, connect_config=influx_config.asjson()
                     )
                     topics = current_topics
             except KeyboardInterrupt:
                 raise click.ClickException("Interruped.")
     return 0
```

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/jdbc_sink/cli.py` & `kafkaconnect-1.3.0/src/kafkaconnect/jdbc_sink/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/mirrormaker2/cli.py` & `kafkaconnect-1.3.0/src/kafkaconnect/mirrormaker2/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/s3_sink/cli.py` & `kafkaconnect-1.3.0/src/kafkaconnect/s3_sink/cli.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect/topic_names_set.py` & `kafkaconnect-1.3.0/src/kafkaconnect/topic_names_set.py`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect.egg-info/PKG-INFO` & `kafkaconnect-1.3.0/src/kafkaconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaconnect
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python client for managing Kafka connectors.
 Home-page: https://github.com/lsst-sqre/kafka-connect-manager
 Author: Association of Universities for Research in Astronomy, Inc. (AURA)
 Author-email: sqre-admin@lists.lsst.org
 Project-URL: Change log, https://github.com/lsst-sqre/kafka-connect-manager/blob/master/CHANGELOG.rst
 Project-URL: Source code, https://github.com/lsst-sqre/kafka-connect-manager
 Project-URL: Issue tracker, https://github.com/lsst-sqre/kafka-connect-manager/issues
```

### Comparing `kafkaconnect-1.2.0/src/kafkaconnect.egg-info/SOURCES.txt` & `kafkaconnect-1.3.0/src/kafkaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_config.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_config.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_create_or_update.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_create_or_update.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_info.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_info.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_list.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_list.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_pause.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_pause.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_plugins.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_plugins.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_remove.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_remove.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_restart.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_restart.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_resume.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_resume.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_status.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_status.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_tasks.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_tasks.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_topics.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_topics.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/cassettes/test_validate.yaml` & `kafkaconnect-1.3.0/tests/cassettes/test_validate.yaml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/docker-compose.yml` & `kafkaconnect-1.3.0/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `kafkaconnect-1.2.0/tests/test_cli.py` & `kafkaconnect-1.3.0/tests/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     assert result.exit_code == 0
     # This query is built by InfluxConfig.update_influx_kcql()
     assert (
         '"connect.influx.kcql": '
         '"INSERT INTO t1 SELECT * FROM t1 WITHTIMESTAMP sys_time() '
         'TIMESTAMPUNIT=MICROSECONDS"' in result.output
     )
-    # Topics are added by ConnectConfig.update_topics()
+    # Topics are added by ConnectConfig.update_config()
     assert '"topics": "t1"' in result.output
 
 
 def test_influxdb_tags() -> None:
     """Test influxdb-sink with tags support."""
     runner = CliRunner()
     result = runner.invoke(
@@ -72,14 +72,37 @@
     assert (
         '"connect.influx.kcql": '
         '"INSERT INTO t1 SELECT * FROM t1 WITHTIMESTAMP sys_time() '
         'TIMESTAMPUNIT=MICROSECONDS WITHTAG(test)"' in result.output
     )
 
 
+def test_remove_prefix() -> None:
+    """Test influxdb-sink with remove_prefix support."""
+    runner = CliRunner()
+    result = runner.invoke(
+        main,
+        [
+            "create",
+            "influxdb-sink",
+            "--dry-run",
+            "--remove-prefix",
+            "abc.",
+            "abc.t1",
+        ],
+    )
+    assert result.exit_code == 0
+    # Add WITHTAG clause to the influx kcql query when using tags
+    assert (
+        '"connect.influx.kcql": '
+        '"INSERT INTO t1 SELECT * FROM abc.t1 WITHTIMESTAMP sys_time() '
+        'TIMESTAMPUNIT=MICROSECONDS"' in result.output
+    )
+
+
 def test_password_from_env() -> None:
     """Test getting the influxdb password from the environment."""
     env = {"KAFKA_CONNECT_INFLUXDB_PASSWORD": "envpasswd"}
     runner = CliRunner()
     result = runner.invoke(
         main, args=["create", "influxdb-sink", "--dry-run", "t1"], env=env
     )
```

### Comparing `kafkaconnect-1.2.0/tests/test_connect.py` & `kafkaconnect-1.3.0/tests/test_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,16 +101,17 @@
         connect_influx_username="foo",
         connect_influx_password="bar",
         connect_influx_error_policy="foo",
         connect_influx_max_retries="1",
         connect_influx_retry_interval="1",
         connect_progress_enabled=True,
         tags="",
+        remove_prefix="",
     )
-    connect_config.update_topics({"t1", "t2", "t3"})
+    connect_config.update_config({"t1", "t2", "t3"})
     result = connect.create_or_update(
         name="influxdb-sink", connect_config=connect_config.asjson()
     )
     assert "influxdb-sink" in result
 
 
 @pytest.mark.vcr
@@ -125,16 +126,17 @@
         connect_influx_username="foo",
         connect_influx_password="bar",
         connect_influx_error_policy="foo",
         connect_influx_max_retries="1",
         connect_influx_retry_interval="1",
         connect_progress_enabled=True,
         tags="",
+        remove_prefix="",
     )
-    connect_config.update_topics({"t1", "t2", "t3"})
+    connect_config.update_config({"t1", "t2", "t3"})
     result = connect.validate(
         name="InfluxSinkConnector", connect_config=connect_config.asjson()
     )
     assert "error_count" in result
 
 
 @pytest.mark.vcr
```

### Comparing `kafkaconnect-1.2.0/tests/test_kafka.py` & `kafkaconnect-1.3.0/tests/test_kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,17 @@
         connect_influx_username="foo",
         connect_influx_password="bar",
         connect_influx_error_policy="foo",
         connect_influx_max_retries="1",
         connect_influx_retry_interval="1",
         connect_progress_enabled=True,
         tags="",
+        remove_prefix="",
     )
-    connect_config.update_topics(t.topic_names_set)
+    connect_config.update_config(t.topic_names_set)
     # Create the connector using the Kafka Connect API
     connect.create_or_update(
         name="influxdb-sink", connect_config=connect_config.asjson()
     )
     # List connectors from the Kafka Connect API
     list = connect.list()
     assert "influxdb-sink" in list
```

### Comparing `kafkaconnect-1.2.0/tests/test_topic_names_set.py` & `kafkaconnect-1.3.0/tests/test_topic_names_set.py`

 * *Files identical despite different names*

