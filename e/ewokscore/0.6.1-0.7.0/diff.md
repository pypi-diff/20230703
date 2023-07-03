# Comparing `tmp/ewokscore-0.6.1.tar.gz` & `tmp/ewokscore-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewokscore-0.6.1.tar", last modified: Tue Jun 20 20:49:52 2023, max compression
+gzip compressed data, was "dist/ewokscore-0.7.0.tar", last modified: Mon Jul  3 08:35:52 2023, max compression
```

## Comparing `ewokscore-0.6.1.tar` & `ewokscore-0.7.0.tar`

### file list

```diff
@@ -1,133 +1,136 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-20 13:03:15.000000 ewokscore-0.6.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-20 20:49:52.000000 ewokscore-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-20 13:03:15.000000 ewokscore-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-20 13:03:15.000000 ewokscore-0.6.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-20 20:49:52.000000 ewokscore-0.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-20 13:03:15.000000 ewokscore-0.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-20 20:47:49.000000 ewokscore-0.6.1/src/ewokscore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/bindings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/cliutils/
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/cliutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/cliutils/cliconvertutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/cliutils/cliexecuteutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/cliutils/clilogutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/cliutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/dynamictask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/events/
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/contexts.py
--rw-rw-rw-   0 root         (0) root         (0)     4996 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/global_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/handlers/base.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/handlers/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/initialize_events.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/events/send_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/graph/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/error_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/graph/execute/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:49:46.000000 ewokscore-0.6.1/src/ewokscore/graph/execute/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/execute/sequential.py
--rw-rw-rw-   0 root         (0) root         (0)     7034 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/multigraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/graph/schema/
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/schema/v0_0.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/schema/v0_1.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/schema/v0_2.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    10989 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/subgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/taskgraph.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/graph/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     8690 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     8562 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/inittask.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/methodtask.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/missing_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/file.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     6064 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/persistence/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/ppftasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3415 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/registration.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-06-20 20:47:49.000000 ewokscore-0.6.1/src/ewokscore/scripttask.py
--rw-rw-rw-   0 root         (0) root         (0)    14409 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7274 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/taskwithprogress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:49:46.000000 ewokscore-0.6.1/src/ewokscore/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/discover_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:49:46.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/acyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/acyclic2.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/acyclic3.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/cyclic1.py
--rw-rw-rw-   0 root         (0) root         (0)     4139 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/demo.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/empty.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/triangle1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/loadtest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:49:46.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/loadtest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/loadtest/graph.json
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/loadtest/subgraph.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:49:46.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/addfunc.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/condsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/errorsumtask.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/nooutputtask.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/simplemethods.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/sumlist.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/sumtask.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7990 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_default_error_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_dynamic_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     7341 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_execute_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6597 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_graph_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_graph_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_graph_start_end_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_link_is_required.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_method_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_persistence.py
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-06-20 17:01:37.000000 ewokscore-0.6.1/src/ewokscore/tests/test_script_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8223 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_sub_graph.py
--rw-rw-rw-   0 root         (0) root         (0)    10843 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_sub_graph_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     6101 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_task_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_uri.py
--rw-rw-rw-   0 root         (0) root         (0)    14406 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_variable.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_variable_namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/test_workflow_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:49:46.000000 ewokscore-0.6.1/src/ewokscore/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4916 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/tests/utils/show.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21421 2023-06-20 13:03:15.000000 ewokscore-0.6.1/src/ewokscore/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4215 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 20:49:52.000000 ewokscore-0.6.1/src/ewokscore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-03 08:01:07.000000 ewokscore-0.7.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-03 08:35:52.000000 ewokscore-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-07-03 08:01:07.000000 ewokscore-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-03 08:01:07.000000 ewokscore-0.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-07-03 08:35:52.000000 ewokscore-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 08:01:07.000000 ewokscore-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-03 08:34:01.000000 ewokscore-0.7.0/src/ewokscore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/bindings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/cliutils/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/cliconvertutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/cliexecuteutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/clilogutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/cliutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/dynamictask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/events/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/global_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/handlers/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/initialize_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/events/send_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/graph/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/error_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/graph/execute/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/graph/execute/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/execute/sequential.py
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/multigraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/v0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/v0_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/schema/v0_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    10989 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/subgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/taskgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/graph/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8690 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8893 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/inittask.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/methodtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/missing_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2800 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/notebooktask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/persistence/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/ppftasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3415 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/registration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/scripttask.py
+-rw-rw-rw-   0 root         (0) root         (0)    14409 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7274 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/taskwithprogress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/discover_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/cyclic1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/triangle1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/graph.json
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/loadtest/subgraph.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/addfunc.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/condsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/errorsumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/nooutputtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     3072 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/notebooktask.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/simplemethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumlist.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumtask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7990 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_default_error_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_dynamic_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7341 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_execute_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6597 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_graph_start_end_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_link_is_required.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_method_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_notebook_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_persistence.py
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_script_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8223 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    10843 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     6101 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_task_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_variable_namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7495 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/test_workflow_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 08:35:46.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/tests/utils/show.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21421 2023-07-03 08:01:07.000000 ewokscore-0.7.0/src/ewokscore/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 08:35:52.000000 ewokscore-0.7.0/src/ewokscore.egg-info/top_level.txt
```

### Comparing `ewokscore-0.6.1/LICENSE.md` & `ewokscore-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/PKG-INFO` & `ewokscore-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.6.1
+Version: 0.7.0
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/issues/
 Keywords: ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: notebooks
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE.md
 
 # ewokscore
```

### Comparing `ewokscore-0.6.1/README.md` & `ewokscore-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/setup.cfg` & `ewokscore-0.7.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -33,29 +33,36 @@
 	packaging
 	ewoksutils >=0.1.2
 
 [options.packages.find]
 where = src
 
 [options.package_data]
-* = *.json
+* = *.json, *.ipynb
 
 [options.extras_require]
+notebooks = 
+	papermill
 test = 
+	%(notebooks)s
 	pytest >=7
 	matplotlib >=3
+	ipykernel
 dev = 
 	%(test)s
-	black >=22
+	black[jupyter] >=22
 	flake8 >=4
+	flake8_nb >= 0.3.1
 doc = 
 	%(test)s
 	sphinx >=4.5
 	sphinxcontrib-mermaid >=0.7
 	sphinx-autodoc-typehints >=1.16
+	nbsphinx
+	nbsphinx_link
 
 [options.entry_points]
 ewoks.tasks.class = 
 	ewokscore.tests.examples.tasks.*=ewokscore
 ewoks.tasks.method = 
 	ewokscore.tests.examples.tasks.*=ewokscore
```

### Comparing `ewokscore-0.6.1/src/ewokscore/bindings.py` & `ewokscore-0.7.0/src/ewokscore/bindings.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/cliutils/__init__.py` & `ewokscore-0.7.0/src/ewokscore/cliutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/cliutils/cliconvertutils.py` & `ewokscore-0.7.0/src/ewokscore/cliutils/cliconvertutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/cliutils/cliexecuteutils.py` & `ewokscore-0.7.0/src/ewokscore/cliutils/cliexecuteutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/cliutils/clilogutils.py` & `ewokscore-0.7.0/src/ewokscore/cliutils/clilogutils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/cliutils/utils.py` & `ewokscore-0.7.0/src/ewokscore/cliutils/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/dynamictask.py` & `ewokscore-0.7.0/src/ewokscore/dynamictask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/events/__init__.py` & `ewokscore-0.7.0/src/ewokscore/events/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/events/contexts.py` & `ewokscore-0.7.0/src/ewokscore/events/contexts.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/events/global_state.py` & `ewokscore-0.7.0/src/ewokscore/events/global_state.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/events/initialize_events.py` & `ewokscore-0.7.0/src/ewokscore/events/initialize_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/events/send_events.py` & `ewokscore-0.7.0/src/ewokscore/events/send_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/analysis.py` & `ewokscore-0.7.0/src/ewokscore/graph/analysis.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/compare.py` & `ewokscore-0.7.0/src/ewokscore/graph/compare.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/error_handlers.py` & `ewokscore-0.7.0/src/ewokscore/graph/error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/execute/sequential.py` & `ewokscore-0.7.0/src/ewokscore/graph/execute/sequential.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/graph_io.py` & `ewokscore-0.7.0/src/ewokscore/graph/graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/multigraph.py` & `ewokscore-0.7.0/src/ewokscore/graph/multigraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/schema/__init__.py` & `ewokscore-0.7.0/src/ewokscore/graph/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/serialize.py` & `ewokscore-0.7.0/src/ewokscore/graph/serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/subgraph.py` & `ewokscore-0.7.0/src/ewokscore/graph/subgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/taskgraph.py` & `ewokscore-0.7.0/src/ewokscore/graph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/graph/validate.py` & `ewokscore-0.7.0/src/ewokscore/graph/validate.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/hashing.py` & `ewokscore-0.7.0/src/ewokscore/hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/inittask.py` & `ewokscore-0.7.0/src/ewokscore/inittask.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 from ewoksutils.import_utils import import_qualname
 
 from .task import Task
 from .methodtask import MethodExecutorTask
 from .scripttask import ScriptExecutorTask
 from .ppftasks import PpfMethodExecutorTask
 from .ppftasks import PpfPortTask
+from .notebooktask import NotebookExecutorTask
 from .dynamictask import get_dynamically_task_class
 from .node import get_node_label
 from .node import NodeIdType
 
 
 TASK_EXECUTABLE_ATTRIBUTE = (
     "class",
     "method",
     "ppfmethod",
     "ppfport",
     "script",
+    "notebook",
     "task",
     "task_type",
 )
 
 TASK_EXECUTABLE_ATTRIBUTE_ALL = TASK_EXECUTABLE_ATTRIBUTE + ("graph",)
 
 TASK_EXECUTABLE_ATTRIBUTE_STR = (
@@ -142,35 +144,46 @@
         "varinfo": varinfo,
         "node_id": node_id,
         "node_attrs": node_attrs,
         "execinfo": execinfo,
     }
     if task_type == "class":
         return Task.instantiate(task_info["task_identifier"], **task_kwargs)
-    elif task_type == "method":
+
+    if task_type == "method":
         task_inputs[MethodExecutorTask.METHOD_ARGUMENT] = task_info["task_identifier"]
         return MethodExecutorTask(**task_kwargs)
-    elif task_type == "ppfmethod":
+
+    if task_type == "ppfmethod":
         task_inputs[PpfMethodExecutorTask.METHOD_ARGUMENT] = task_info[
             "task_identifier"
         ]
         return PpfMethodExecutorTask(**task_kwargs)
-    elif task_type == "ppfport":
+
+    if task_type == "ppfport":
         return PpfPortTask(**task_kwargs)
-    elif task_type == "script":
+
+    if task_type == "script":
         task_inputs[ScriptExecutorTask.SCRIPT_ARGUMENT] = task_info["task_identifier"]
         return ScriptExecutorTask(**task_kwargs)
-    elif task_type == "generated":
+
+    if task_type == "method":
+        task_inputs[NotebookExecutorTask.NOTEBOOK_ARGUMENT] = task_info[
+            "task_identifier"
+        ]
+        return NotebookExecutorTask(**task_kwargs)
+
+    if task_type == "generated":
         task_class = get_dynamically_task_class(
             node_attrs.get("task_generator"), task_info["task_identifier"]
         )
         return task_class(**task_kwargs)
-    else:
-        node_label = get_node_label(node_id, node_attrs)
-        raise_task_error(node_label, all=False)
+
+    node_label = get_node_label(node_id, node_attrs)
+    raise_task_error(node_label, all=False)
 
 
 def add_dynamic_inputs(
     dynamic_inputs: dict,
     link_attrs: dict,
     source_results: dict,
     source_id: Optional[NodeIdType] = None,
@@ -209,43 +222,46 @@
             dynamic_inputs[input_arg] = source_results
 
 
 def task_executable(node_id: NodeIdType, node_attrs: dict):
     task_type, task_info = task_executable_info(node_id, node_attrs)
     if task_type == "class":
         return task_info["task_identifier"], import_qualname
-    elif task_type == "method":
+    if task_type == "method":
         return task_info["task_identifier"], import_method
-    elif task_type == "ppfmethod":
+    if task_type == "ppfmethod":
         return task_info["task_identifier"], import_method
-    elif task_type == "ppfport":
+    if task_type == "ppfport":
         return None, None
-    elif task_type == "script":
+    if task_type == "script":
         return task_info["task_identifier"], None
-    elif task_type == "generated":
+    if task_type == "notebook":
+        return task_info["task_identifier"], None
+    if task_type == "generated":
         return task_info["task_identifier"], partial(
             get_dynamically_task_class, node_attrs.get("task_generator")
         )
-    else:
-        node_label = get_node_label(node_id, node_attrs)
-        raise_task_error(node_label, all=False)
+    node_label = get_node_label(node_id, node_attrs)
+    raise_task_error(node_label, all=False)
 
 
 def get_task_class(node_id: NodeIdType, node_attrs: dict):
     task_type, task_info = task_executable_info(node_id, node_attrs)
     if task_type == "class":
         return Task.get_subclass(task_info["task_identifier"])
-    elif task_type == "method":
+    if task_type == "method":
         return MethodExecutorTask
-    elif task_type == "ppfmethod":
+    if task_type == "ppfmethod":
         return PpfMethodExecutorTask
-    elif task_type == "ppfport":
+    if task_type == "ppfport":
         return PpfPortTask
-    elif task_type == "script":
+    if task_type == "script":
         return ScriptExecutorTask
-    elif task_type == "task":
+    if task_type == "notebook":
+        return NotebookExecutorTask
+    if task_type == "task":
         return get_dynamically_task_class(
             node_attrs.get("task_generator"), task_info["task_identifier"]
         )
-    else:
-        node_label = get_node_label(node_id, node_attrs)
-        raise_task_error(node_label, all=False)
+
+    node_label = get_node_label(node_id, node_attrs)
+    raise_task_error(node_label, all=False)
```

### Comparing `ewokscore-0.6.1/src/ewokscore/methodtask.py` & `ewokscore-0.7.0/src/ewokscore/methodtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/missing_data.py` & `ewokscore-0.7.0/src/ewokscore/missing_data.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/node.py` & `ewokscore-0.7.0/src/ewokscore/node.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/persistence/atomic.py` & `ewokscore-0.7.0/src/ewokscore/persistence/atomic.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/persistence/file.py` & `ewokscore-0.7.0/src/ewokscore/persistence/file.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/persistence/json.py` & `ewokscore-0.7.0/src/ewokscore/persistence/json.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/persistence/nexus.py` & `ewokscore-0.7.0/src/ewokscore/persistence/nexus.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/persistence/proxy.py` & `ewokscore-0.7.0/src/ewokscore/persistence/proxy.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/persistence/uri.py` & `ewokscore-0.7.0/src/ewokscore/persistence/uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/ppftasks.py` & `ewokscore-0.7.0/src/ewokscore/ppftasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/progress.py` & `ewokscore-0.7.0/src/ewokscore/progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/registration.py` & `ewokscore-0.7.0/src/ewokscore/registration.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/scripttask.py` & `ewokscore-0.7.0/src/ewokscore/scripttask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/task.py` & `ewokscore-0.7.0/src/ewokscore/task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/task_discovery.py` & `ewokscore-0.7.0/src/ewokscore/task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/taskwithprogress.py` & `ewokscore-0.7.0/src/ewokscore/taskwithprogress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/__init__.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/acyclic1.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/acyclic2.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic2.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/acyclic3.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/acyclic3.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/cyclic1.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/cyclic1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/demo.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/demo.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/graphs/triangle1.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/graphs/triangle1.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/sumlist.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumlist.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/examples/tasks/sumtask.py` & `ewokscore-0.7.0/src/ewokscore/tests/examples/tasks/sumtask.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_cli_utils.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_default_error_handlers.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_default_error_handlers.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_dynamic_tasks.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_events.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_examples.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_execute_graph.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_execute_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_graph.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_graph_io.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_graph_io.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_graph_schema.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_graph_schema.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_graph_serialize.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_graph_start_end_nodes.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_graph_start_end_nodes.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_hashing.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_link_is_required.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_link_is_required.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_method_task.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_method_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_persistence.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_script_task.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_script_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_sub_graph.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_sub_graph_serialize.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_sub_graph_serialize.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_task.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_task_discovery.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_task_progress.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_task_progress.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_uri.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_variable.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_variable_namespaces.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_variable_namespaces.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/test_workflow_events.py` & `ewokscore-0.7.0/src/ewokscore/tests/test_workflow_events.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/tests/utils/results.py` & `ewokscore-0.7.0/src/ewokscore/tests/utils/results.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/utils.py` & `ewokscore-0.7.0/src/ewokscore/utils.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore/variable.py` & `ewokscore-0.7.0/src/ewokscore/variable.py`

 * *Files identical despite different names*

### Comparing `ewokscore-0.6.1/src/ewokscore.egg-info/PKG-INFO` & `ewokscore-0.7.0/src/ewokscore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ewokscore
-Version: 0.6.1
+Version: 0.7.0
 Summary: API for graphs and tasks in Ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/
 Project-URL: Documentation, https://ewokscore.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewokscore/issues/
 Keywords: ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: notebooks
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE.md
 
 # ewokscore
```

### Comparing `ewokscore-0.6.1/src/ewokscore.egg-info/SOURCES.txt` & `ewokscore-0.7.0/src/ewokscore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/ewokscore/bindings.py
 src/ewokscore/dynamictask.py
 src/ewokscore/hashing.py
 src/ewokscore/inittask.py
 src/ewokscore/methodtask.py
 src/ewokscore/missing_data.py
 src/ewokscore/node.py
+src/ewokscore/notebooktask.py
 src/ewokscore/ppftasks.py
 src/ewokscore/progress.py
 src/ewokscore/registration.py
 src/ewokscore/scripttask.py
 src/ewokscore/task.py
 src/ewokscore/task_discovery.py
 src/ewokscore/taskwithprogress.py
@@ -75,14 +76,15 @@
 src/ewokscore/tests/test_graph_io.py
 src/ewokscore/tests/test_graph_schema.py
 src/ewokscore/tests/test_graph_serialize.py
 src/ewokscore/tests/test_graph_start_end_nodes.py
 src/ewokscore/tests/test_hashing.py
 src/ewokscore/tests/test_link_is_required.py
 src/ewokscore/tests/test_method_task.py
+src/ewokscore/tests/test_notebook_task.py
 src/ewokscore/tests/test_persistence.py
 src/ewokscore/tests/test_script_task.py
 src/ewokscore/tests/test_sub_graph.py
 src/ewokscore/tests/test_sub_graph_serialize.py
 src/ewokscore/tests/test_task.py
 src/ewokscore/tests/test_task_discovery.py
 src/ewokscore/tests/test_task_progress.py
@@ -103,13 +105,14 @@
 src/ewokscore/tests/examples/loadtest/graph.json
 src/ewokscore/tests/examples/loadtest/subgraph.json
 src/ewokscore/tests/examples/tasks/__init__.py
 src/ewokscore/tests/examples/tasks/addfunc.py
 src/ewokscore/tests/examples/tasks/condsumtask.py
 src/ewokscore/tests/examples/tasks/errorsumtask.py
 src/ewokscore/tests/examples/tasks/nooutputtask.py
+src/ewokscore/tests/examples/tasks/notebooktask.ipynb
 src/ewokscore/tests/examples/tasks/simplemethods.py
 src/ewokscore/tests/examples/tasks/sumlist.py
 src/ewokscore/tests/examples/tasks/sumtask.py
 src/ewokscore/tests/utils/__init__.py
 src/ewokscore/tests/utils/results.py
 src/ewokscore/tests/utils/show.py
```

