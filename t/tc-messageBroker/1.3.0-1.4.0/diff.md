# Comparing `tmp/tc-messageBroker-1.3.0.tar.gz` & `tmp/tc-messageBroker-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.3.0.tar", last modified: Sat Jul  1 08:52:14 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.4.0.tar", last modified: Mon Jul  3 11:23:57 2023, max compression
```

## Comparing `tc-messageBroker-1.3.0.tar` & `tc-messageBroker-1.4.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.845271 tc-messageBroker-1.3.0/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.771222 tc-messageBroker-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 11:23:57.771222 tc-messageBroker-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:23:57.771222 tc-messageBroker-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.763222 tc-messageBroker-1.4.0/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.763222 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.763222 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.767222 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.767222 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.767222 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.767222 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.763222 tc-messageBroker-1.4.0/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 11:23:57.000000 tc-messageBroker-1.4.0/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 11:23:57.000000 tc-messageBroker-1.4.0/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:23:57.000000 tc-messageBroker-1.4.0/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 11:23:57.000000 tc-messageBroker-1.4.0/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 11:23:57.000000 tc-messageBroker-1.4.0/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.767222 tc-messageBroker-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.767222 tc-messageBroker-1.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:57.771222 tc-messageBroker-1.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_queue_declare_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-03 11:23:32.000000 tc-messageBroker-1.4.0/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.3.0/PKG-INFO` & `tc-messageBroker-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.3.0
+Version: 1.4.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.3.0/README.md` & `tc-messageBroker-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/setup.py` & `tc-messageBroker-1.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.3.0",
+    version="1.4.0",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.4.0/tc_messageBroker/message_broker.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,29 +26,40 @@
     def __new__(cls, broker_url: str, port: int, username: str, password: str):
         ## making it singleton
         if not hasattr(cls, "instance"):
             cls.instance = super(RabbitMQ, cls).__new__(cls)
         return cls.instance
 
     def connect(
-        self, queue_name: str, consume_options: dict = None, heartbeat: int = 60
+        self,
+        queue_name: str,
+        consume_options: dict = None,
+        heartbeat: int = 60,
+        **kwargs,
     ) -> bool:
         """
         connect the rabbitMQ broker and start consuming
 
         Parameters:
         -------------
         queue_name : str
             the queue name to connect
         consume_options : dict
             additional arguments for basic_consume method
             default is `None`
         heartbeat : int
             the number of seconds for a message to stay alive
             default is 60 seconds
+        **kwargs :
+            queue_durable : bool
+                is the queue durable or not
+                default is True
+            queue_auto_delete : bool
+                Deleting the queue after the consumer cancels or disconnect
+                default is False
 
         Returns:
         ---------
         is_successful : bool
             if True, connecting to rabbitMQ server was successful
             otherwise would return False
         """
@@ -63,27 +74,54 @@
                     heartbeat=heartbeat,  ## disabling the heartbeat
                 ),
             )
             self.channel = self.connection.channel()
 
             # make sure that the channel is created,
             # if not this statement will create it
-            self.channel.queue_declare(queue=queue_name)
+            self._queue_declare(queue_name=queue_name, kwargs=kwargs)
 
             self.channel.basic_consume(
                 queue=queue_name,
                 on_message_callback=self._consume_callback,
                 auto_ack=False,
                 arguments=consume_options,
             )
             return True
         except Exception as exp:
             logging.error(f" Something went wrong with RabbitMQ {exp}")
             return False
 
+    def _get_declare_queue_param(self, kwargs):
+        """
+        kwargs must have `queue_auto_delete`, and `queue_durability`
+        or must not have, other kwargs would be skipped
+
+        Returns:
+        -----------
+        queue_durability : bool
+            the queue durability over rabbitMQ getting down
+        queue_auto_delete : bool
+            to delete or not delete the queue
+            if consumer disconnects or cancells consuming
+        """
+        queue_durability = None
+        if "queue_durable" in kwargs.keys():
+            queue_durability = kwargs["queue_durable"]
+        else:
+            queue_durability = True
+
+        queue_auto_delete = None
+        if "queue_auto_delete" in kwargs.keys():
+            queue_auto_delete = kwargs["queue_auto_delete"]
+        else:
+            queue_auto_delete = False
+
+        return queue_durability, queue_auto_delete
+
     def _consume_callback(self, ch, method, properties, body) -> bool:
         """
         consume a message with a specific body
 
         Parameters:
         -------------
         method : any
@@ -114,19 +152,28 @@
             self.connection.add_callback_threadsafe(
                 functools.partial(
                     self.channel.basic_ack,
                     delivery_tag=method.delivery_tag,
                 )
             )
 
-    def consume(self, queue_name: str, consume_options: dict = None):
+    def consume(self, queue_name: str, consume_options: dict = None, **kwargs):
         """
         set consuming events from a queue
+        queue_name : str
+            the queue name to consume
+        **kwargs :
+            queue_durable : bool
+                is the queue durable or not
+                default is True
+            queue_auto_delete : bool
+                Deleting the queue after the consumer cancels or disconnect
+                default is False
         """
-        self.channel.queue_declare(queue=queue_name)
+        self._queue_declare(queue_name=queue_name, kwargs=kwargs)
 
         self.channel.basic_consume(
             queue=queue_name,
             on_message_callback=self._consume_callback,
             arguments=consume_options,
             auto_ack=False,
         )
@@ -149,16 +196,14 @@
         options : any
             additional arguments for basic_publish method
             default is `None`
 
         """
         data = self._define_data(event=event, content=content)
 
-        self.channel.queue_declare(queue=queue_name)
-
         self.channel.basic_publish(
             exchange=self.exchange_name,
             routing_key=queue_name,
             body=data,
             properties=options,
         )
 
@@ -223,30 +268,61 @@
             exchange_type=type,
             durable=durable,
             auto_delete=auto_delete,
             arguments=options,
         )
         self.exchange_name = name
 
+    def _queue_declare(self, queue_name: str, **kwargs):
+        """
+        declare the queue
+
+        Parameters:
+        --------------
+        queue_name : str
+        **kwargs :
+            queue_durable : bool
+                is the queue durable or not
+                default is True
+            queue_auto_delete : bool
+                Deleting the queue after the consumer cancels or disconnect
+                default is False
+        """
+        (queue_durability, queue_auto_delete) = self._get_declare_queue_param(kwargs)
+
+        # make sure that the channel is created,
+        # if not this statement will create it
+        self.channel.queue_declare(
+            queue=queue_name, durable=queue_durability, auto_delete=queue_auto_delete
+        )
+
     def bind_queue_to_exchange(
-        self, queue_name: str, exchange_name: str, pattern: str
+        self, queue_name: str, exchange_name: str, pattern: str, **kwargs
     ) -> None:
         """
         bind a queue to a special exchange point
 
         Parameters:
         -----------
         queue_name : str
             the name of the queue we want to bind
         exchange_name : str
             the exchange point name
         pattern : str
             routing_key of the queue
+        **kwargs :
+            queue_durable : bool
+                is the queue durable or not
+                default is True
+            queue_auto_delete : bool
+                Deleting the queue after the consumer cancels or disconnect
+                default is False
         """
-        self.channel.queue_declare(queue=queue_name)
+
+        self._queue_declare(queue_name=queue_name, kwargs=kwargs)
 
         self.channel.queue_bind(
             queue=queue_name, exchange=exchange_name, routing_key=pattern
         )
 
     def publish_on_exchange(
         self,
```

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py` & `tc-messageBroker-1.4.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.4.0/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.3.0
+Version: 1.4.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.3.0/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.4.0/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,12 +35,13 @@
 tests/unit/test_choreagraphy_base.py
 tests/unit/test_enum_status.py
 tests/unit/test_event.py
 tests/unit/test_message_broker.py
 tests/unit/test_mongodb.py
 tests/unit/test_predefined_transactions.py
 tests/unit/test_queue.py
+tests/unit/test_queue_declare_params.py
 tests/unit/test_saga_base.py
 tests/unit/test_saga_base_utils.py
 tests/unit/test_saga_next.py
 tests/unit/test_saga_start.py
 tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.3.0/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.4.0/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/integration/test_mongodb.py` & `tc-messageBroker-1.4.0/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/integration/test_saga.py` & `tc-messageBroker-1.4.0/tests/integration/test_saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_choreagraphy_base.py` & `tc-messageBroker-1.4.0/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_message_broker.py` & `tc-messageBroker-1.4.0/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_predefined_transactions.py` & `tc-messageBroker-1.4.0/tests/unit/test_predefined_transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_saga_base.py` & `tc-messageBroker-1.4.0/tests/unit/test_saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_saga_base_utils.py` & `tc-messageBroker-1.4.0/tests/unit/test_saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_saga_next.py` & `tc-messageBroker-1.4.0/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_saga_start.py` & `tc-messageBroker-1.4.0/tests/unit/test_saga_start.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.3.0/tests/unit/test_transactions.py` & `tc-messageBroker-1.4.0/tests/unit/test_transactions.py`

 * *Files identical despite different names*

