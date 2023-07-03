# Comparing `tmp/hkube_python_wrapper-2.5.0.dev4.tar.gz` & `tmp/hkube_python_wrapper-2.5.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hkube_python_wrapper-2.5.0.dev4.tar", last modified: Thu Mar  2 07:26:46 2023, max compression
+gzip compressed data, was "dist/hkube_python_wrapper-2.5.0.dev5.tar", last modified: Mon Jul  3 13:26:52 2023, max compression
```

## Comparing `hkube_python_wrapper-2.5.0.dev4.tar` & `hkube_python_wrapper-2.5.0.dev5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/cache/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/hkube_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/waitFor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/DataRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/DataServer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/MessageListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/MessageProducer.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/StreamingListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/StreamingManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQPingServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQServers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/base_storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/fs_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/s3_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/task_output_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/tracing/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/DaemonThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/fifo_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/object_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/percentile.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/queueImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/stdout_redirector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/timerImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/url_encode_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23407 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/algorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-02 07:26:44.000000 hkube_python_wrapper-2.5.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/mock_ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/mocks/mockdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:46.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_alg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_alg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_alg/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_hkube_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_storage_manager_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_storage_manager_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_utils_getpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/xtest_communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-02 07:26:40.000000 hkube_python_wrapper-2.5.0.dev4/tests/xtest_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/cache/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/hkube_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/waitFor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/DataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/DataServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/MessageListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/MessageProducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/StreamingListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/StreamingManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQPingServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQServers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/base_storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/fs_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/s3_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/task_output_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/tracing/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/DaemonThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/fifo_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/object_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/queueImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/stdout_redirector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/timerImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/url_encode_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/algorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-03 13:26:50.000000 hkube_python_wrapper-2.5.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/mock_ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/mocks/mockdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:52.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_alg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_alg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_alg/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_hkube_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_storage_manager_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_storage_manager_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_utils_getpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/xtest_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-03 13:26:46.000000 hkube_python_wrapper-2.5.0.dev5/tests/xtest_encoding.py
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/PKG-INFO` & `hkube_python_wrapper-2.5.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkube_python_wrapper
-Version: 2.5.0.dev4
+Version: 2.5.0.dev5
 Summary: Hkube Python Wrapper
 Home-page: https://github.com/kube-HPC/python-wrapper.hkube
 Author: Hkube
 Author-email: hkube.dev@gmail.com
 License: MIT
 Description: # HKube Python Wrapper
         [![Build Status](https://travis-ci.org/kube-HPC/python-wrapper.hkube.svg?branch=master)](https://travis-ci.org/kube-HPC/python-wrapper.hkube)
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/README.md` & `hkube_python_wrapper-2.5.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/cache/caching.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/cache/caching.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/hkube_api.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/hkube_api.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/codeApi/waitFor.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/codeApi/waitFor.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/DataRequest.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/DataRequest.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/DataServer.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/DataServer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/MessageListener.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/MessageListener.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/MessageProducer.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/MessageProducer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/StreamingListener.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/StreamingListener.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/streaming/StreamingManager.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/streaming/StreamingManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import threading
 from .MessageListener import MessageListener
 from .MessageProducer import MessageProducer
 from .StreamingListener import StreamingListener
-from hkube_python_wrapper.util.logger import log
+from hkube_python_wrapper.util.logger import log, algorithmLogger
 
 
 class StreamingManager():
 
     def __init__(self):
         self.threadLocalStorage = threading.local()
         self.threadLocalStorage.sendMessageId = None
@@ -69,15 +69,15 @@
             log.error('no input listeners on _onMessage method')
             return
         for listener in self._inputListener:
             try:
                 listener(msg, origin)
             except Exception as e:
                 log.error("hkube_api message listener threw exception: {e}", e=str(e))
-                log.exception(e)
+                algorithmLogger.exception(e)
         self.threadLocalStorage.messageFlowPattern = []
 
     def _getMessageListeners(self):
         return list(self._messageListeners.values())
 
     def startMessageListening(self):
         self.listeningToMessages = True
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQPingServer.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQPingServer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQRequest.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQRequest.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQServer.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQServer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/ZMQServers.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/ZMQServers.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/ZMQListener.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/Flow.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/MessageQueue.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/communication/zmq/streaming/producer/ZMQProducer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/config/config.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/config/config.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/base_storage_manager.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/base_storage_manager.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/fs_adapter.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/fs_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/s3_adapter.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/s3_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/storage_manager.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/storage/task_output_manager.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/storage/task_output_manager.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/tracing/tracer.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/decorators.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/decorators.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/encoding.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/encoding.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/logger.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 import logging
+import traceback
+
 from hkube_python_wrapper.util.type_check import isString
 from logging import LoggerAdapter
 from hkube_python_wrapper.config import config
 
 
 class Adapter(LoggerAdapter):
     def process(self, msg, kwargs):
         if isString(msg):
             return msg.format(**kwargs), {}
         return msg, kwargs
 
+    def exception(self, err, *args, exc_info=True, **kwargs):
+        if self.isEnabledFor(logging.ERROR):
+            exc_text = self._format_exception(exc_info)
+            self.error('\n' + str(err) + ' ' + exc_text, *args, **kwargs)
+
+    def _format_exception(self, exc_info):
+        if exc_info:
+            stack_trace = traceback.format_exc().strip()
+            return stack_trace.replace('\n', '\\n')
+        return ''
+
 
 log = Adapter(logging.getLogger('wrapper'), {})
+algorithmLogger = Adapter(logging.getLogger('algorithm'), {})
 
 
 def setup():
     level = config.logging.get('level', 'INFO')
     level = level.upper()
     logger = logging.getLogger('wrapper')
     logger.propagate = False
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/object_path.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/object_path.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/percentile.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/percentile.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/stdout_redirector.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/stdout_redirector.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/util/timerImpl.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/util/timerImpl.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/algorunner.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/algorunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .messages import messages
 from hkube_python_wrapper.tracing import Tracer
 from hkube_python_wrapper.codeApi.hkube_api import HKubeApi
 from hkube_python_wrapper.communication.DataServer import DataServer
 from hkube_python_wrapper.communication.streaming.StreamingManager import StreamingManager
 from hkube_python_wrapper.util.queueImpl import Queue, Empty
 from hkube_python_wrapper.util.timerImpl import Timer
-from hkube_python_wrapper.util.logger import log
+from hkube_python_wrapper.util.logger import log ,algorithmLogger
 from hkube_python_wrapper.util.url_encode_impl import url_encode
 from hkube_python_wrapper.util.stdout_redirector import stdout_redirector
 import os
 import sys
 import platform
 import importlib
 import traceback
@@ -224,24 +224,27 @@
         if command == messages.incoming.initialize:
             self._init(data)
         elif command == messages.incoming.start:
             self._start(data)
         elif command == messages.incoming.stop:
             self._stopAlgorithm(data)
         elif command == messages.incoming.streamingInMessage:
-            self.streamingManager.onMessage(messageFlowPattern=None, msg=data['payload'], origin=data['origin'], sendMessageId=data['sendMessageId'])
-            self._wsc.send({'command': messages.outgoing.streamingInMessageDone, 'data': {'sendMessageId': data['sendMessageId']}})
+            self.streamingManager.onMessage(messageFlowPattern=None, msg=data['payload'], origin=data['origin'],
+                                            sendMessageId=data['sendMessageId'])
+            self._wsc.send(
+                {'command': messages.outgoing.streamingInMessageDone, 'data': {'sendMessageId': data['sendMessageId']}})
         elif command == messages.incoming.serviceDiscoveryUpdate:
             self._discovery_update(data)
         elif command == messages.incoming.exit:
             # call exit on different thread to prevent deadlock
             Timer(0.1, lambda: self._exit(data), name="Exit timer").start()
         elif command in [messages.incoming.algorithmExecutionDone, messages.incoming.algorithmExecutionError]:
             self._hkubeApi.algorithmExecutionDone(data)
-        elif command in [messages.incoming.subPipelineDone, messages.incoming.subPipelineError, messages.incoming.subPipelineStopped]:
+        elif command in [messages.incoming.subPipelineDone, messages.incoming.subPipelineError,
+                         messages.incoming.subPipelineStopped]:
             self._hkubeApi.subPipelineDone(data)
         elif command == messages.incoming.dataSourceResponse:
             self._hkubeApi.dataSourceResponse(data)
         elif command == messages.incoming.alreadyConnectedError:
             log.error('Debugger already connected from {hostname}'.format(hostname=data['hostname']))
             # pylint: disable=protected-access
             os._exit(1)
@@ -320,17 +323,17 @@
             else:
                 self._input = options
                 self._job = Job(options)
                 if self._job.isStreaming and not self._job.isStateful:
                     self._algorithm = self._statelessWrapped
                 else:
                     self._algorithm = self._originalAlgorithm
-                method = self._getMethod('init')
-                if (method is not None):
-                    method(options)
+                    method = self._getMethod('init')
+                    if (method is not None):
+                        method(options)
                 self._sendCommand(messages.outgoing.initialized, None)
 
         except Exception as e:
             self.sendError(e)
         finally:
             if (redirector):
                 redirector.flush()
@@ -381,21 +384,25 @@
             if (options):
                 topSpan = options.get('spanId')
             else:
                 topSpan = self._job.spanId
             span = Tracer.instance.create_span("start", topSpan, jobId, taskId, nodeName)
             newInput = self._dataAdapter.getData(self._input)
             self._input.update({'input': newInput})
+            if self._job.isStreaming and not self._job.isStateful:
+                method = self._getMethod('init')
+                if (method is not None):
+                    method(self._input)
             method = self._getMethod('start')
             algorithmData = method(self._input, self._hkubeApi)
             if not (self._stopped):
                 self._handle_response(algorithmData, jobId, taskId, nodeName, savePaths, span)
 
         except Exception as e:
-            traceback.print_exc()
+            algorithmLogger.exception(e)
             Tracer.instance.finish_span(span, e)
             self.sendError(e)
         finally:
             if (redirector):
                 redirector.flush()
                 redirector.events.on_data -= self._log_message
                 redirector.cleanup()
@@ -517,22 +524,24 @@
             code = option.get('exitCode', 0)
             self._active = False
             log.info('Got exit command. Exiting with code {code}', code=code)
             sys.exit(code)
 
         except Exception as e:
             log.error('Got error during exit: {e}', e=e)
+            algorithmLogger.exception(e)
             # pylint: disable=protected-access
             os._exit(0)
 
     def _checkQueueSize(self, event):
         if (self._job.isStreaming):
             if (self.streamingManager.messageProducer):
                 try:
-                    log.info('Messages left in queue on {event}={queue}', event=event, queue=str(len(self.streamingManager.messageProducer.adapter.messageQueue.queue)))
+                    log.info('Messages left in queue on {event}={queue}', event=event,
+                             queue=str(len(self.streamingManager.messageProducer.adapter.messageQueue.queue)))
                 except Exception:
                     log.error('Failed to print number of messages left in queue on {event}', event=event)
             else:
                 log.info('MessageProducer already None on {event}', event=event)
 
     def _sendCommand(self, command, data):
         try:
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/data_adapter.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/data_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/job.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/job.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/messages.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/messages.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/statelessAlgoWrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import threading
-from hkube_python_wrapper.util.logger import log
+from hkube_python_wrapper.util.logger import log, algorithmLogger
 
 class statelessAlgoWrapper(object):
     def __init__(self, algo):
         self._hkubeApi = None
         self.originalAlgorithm = algo
         self.options = None
         self.active = False
@@ -17,15 +17,15 @@
         options['streamInput'] = {'message': msg, 'origin': origin}
         try:
             result = self.originalAlgorithm['start'](options, self._hkubeApi)
             if (self.options['childs']):
                 self._hkubeApi.sendMessage(result)
         except Exception as e:
             log.error('statelessWrapper error, {e}', e=str(e))
-            log.exception(e)
+            algorithmLogger.exception(e)
             self.error = e
 
     def start(self, options, hkube_api):
         # pylint: disable=unused-argument
         self._hkubeApi = hkube_api
         self._hkubeApi.registerInputListener(onMessage=self._invokeAlgorithm)
         self._hkubeApi.startMessageListening()
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper/wrapper/wc.py` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper/wrapper/wc.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/PKG-INFO` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkube-python-wrapper
-Version: 2.5.0.dev4
+Version: 2.5.0.dev5
 Summary: Hkube Python Wrapper
 Home-page: https://github.com/kube-HPC/python-wrapper.hkube
 Author: Hkube
 Author-email: hkube.dev@gmail.com
 License: MIT
 Description: # HKube Python Wrapper
         [![Build Status](https://travis-ci.org/kube-HPC/python-wrapper.hkube.svg?branch=master)](https://travis-ci.org/kube-HPC/python-wrapper.hkube)
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/hkube_python_wrapper.egg-info/SOURCES.txt` & `hkube_python_wrapper-2.5.0.dev5/hkube_python_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/setup.cfg` & `hkube_python_wrapper-2.5.0.dev5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.5.0-dev4
+current_version = 2.5.0-dev5
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/setup.py` & `hkube_python_wrapper-2.5.0.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import print_function, division, absolute_import
 
 import setuptools
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '2.5.0-dev4'
+VERSION = '2.5.0-dev5'
 
 
 
 
 
 packages = setuptools.find_packages()
```

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/configs/config.py` & `hkube_python_wrapper-2.5.0.dev5/tests/configs/config.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/conftest.py` & `hkube_python_wrapper-2.5.0.dev5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/mock_ws_server.py` & `hkube_python_wrapper-2.5.0.dev5/tests/mock_ws_server.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/mocks/mockdata.py` & `hkube_python_wrapper-2.5.0.dev5/tests/mocks/mockdata.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_cache.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_communication.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_communication.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_data_adapter.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_data_adapter.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_encoding.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_hkube_api.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_hkube_api.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_queue.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_storage_manager_fs.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_storage_manager_fs.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_storage_manager_s3.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_storage_manager_s3.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_streaming.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_tracer.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_tracer.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_utils_getpath.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_utils_getpath.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_wrapper.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/test_zmq.py` & `hkube_python_wrapper-2.5.0.dev5/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/xtest_communication.py` & `hkube_python_wrapper-2.5.0.dev5/tests/xtest_communication.py`

 * *Files identical despite different names*

### Comparing `hkube_python_wrapper-2.5.0.dev4/tests/xtest_encoding.py` & `hkube_python_wrapper-2.5.0.dev5/tests/xtest_encoding.py`

 * *Files identical despite different names*

