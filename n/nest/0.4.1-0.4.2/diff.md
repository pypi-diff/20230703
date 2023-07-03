# Comparing `tmp/nest-0.4.1.tar.gz` & `tmp/nest-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nest-0.4.1.tar", last modified: Mon Mar 14 16:08:20 2022, max compression
+gzip compressed data, was "nest-0.4.2.tar", last modified: Mon Jul  3 17:53:31 2023, max compression
```

## Comparing `nest-0.4.1.tar` & `nest-0.4.2.tar`

### file list

```diff
@@ -1,117 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.998597 nest-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1050 2022-03-14 15:34:55.000000 nest-0.4.1/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)    15220 2021-06-20 07:10:57.000000 nest-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2718 2022-03-14 16:08:19.998597 nest-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1680 2022-03-14 15:34:55.000000 nest-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.990597 nest-0.4.1/nest/
--rw-rw-rw-   0 root         (0) root         (0)     1947 2022-03-14 15:34:55.000000 nest-0.4.1/nest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2022-03-03 15:03:31.000000 nest-0.4.1/nest/clean_up.py
--rw-rw-rw-   0 root         (0) root         (0)      320 2022-03-14 15:34:55.000000 nest-0.4.1/nest/config.json
--rw-rw-rw-   0 root         (0) root         (0)     3967 2022-03-14 15:34:55.000000 nest-0.4.1/nest/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.990597 nest-0.4.1/nest/engine/
--rw-rw-rw-   0 root         (0) root         (0)      504 2022-03-03 15:03:31.000000 nest-0.4.1/nest/engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4759 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/dynamic_routing.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2021-11-01 14:30:09.000000 nest-0.4.1/nest/engine/ethtool.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2022-03-14 15:34:55.000000 nest-0.4.1/nest/engine/exec.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2022-03-01 15:53:35.000000 nest-0.4.1/nest/engine/ip_address.py
--rw-rw-rw-   0 root         (0) root         (0)     4149 2021-11-01 14:30:09.000000 nest-0.4.1/nest/engine/ip_link.py
--rw-rw-rw-   0 root         (0) root         (0)     1819 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/ip_mpls_route.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/ip_netns.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/ip_route.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/iperf3.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/ipv6_states.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/iterators.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/netperf.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2022-03-14 15:34:55.000000 nest-0.4.1/nest/engine/ping.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2021-10-10 07:01:32.000000 nest-0.4.1/nest/engine/setns.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/sysctl.py
--rw-rw-rw-   0 root         (0) root         (0)     7956 2021-11-02 18:09:47.000000 nest-0.4.1/nest/engine/tc.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2021-10-10 07:01:32.000000 nest-0.4.1/nest/engine/uname.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2021-06-20 07:10:57.000000 nest-0.4.1/nest/engine/util.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-03-14 15:34:55.000000 nest-0.4.1/nest/exception.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2021-06-20 07:10:57.000000 nest-0.4.1/nest/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/experiment/
--rw-rw-rw-   0 root         (0) root         (0)      249 2021-06-20 07:10:57.000000 nest-0.4.1/nest/experiment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6367 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/experiment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/experiment/info/
--rw-rw-rw-   0 root         (0) root         (0)     2072 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/info/README.txt
--rw-rw-rw-   0 root         (0) root         (0)      846 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/interrupts.py
--rw-rw-rw-   0 root         (0) root         (0)     3162 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/pack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/experiment/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-20 07:10:57.000000 nest-0.4.1/nest/experiment/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/parser/iperf3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/experiment/parser/iterators/
--rw-rw-rw-   0 root         (0) root         (0)      522 2021-06-20 07:10:57.000000 nest-0.4.1/nest/experiment/parser/iterators/ss.sh
--rw-rw-rw-   0 root         (0) root         (0)      463 2021-06-20 07:10:57.000000 nest-0.4.1/nest/experiment/parser/iterators/tc.sh
--rw-rw-rw-   0 root         (0) root         (0)     6654 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/parser/netperf.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/parser/ping.py
--rw-rw-rw-   0 root         (0) root         (0)     3317 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/parser/runnerbase.py
--rw-rw-rw-   0 root         (0) root         (0)     5857 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/parser/ss.py
--rw-rw-rw-   0 root         (0) root         (0)    12257 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/parser/tc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/experiment/plotter/
--rw-rw-rw-   0 root         (0) root         (0)      520 2021-06-20 07:10:57.000000 nest-0.4.1/nest/experiment/plotter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2021-11-01 14:30:09.000000 nest-0.4.1/nest/experiment/plotter/common.py
--rw-rw-rw-   0 root         (0) root         (0)     3569 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/plotter/iperf3.py
--rw-rw-rw-   0 root         (0) root         (0)     3122 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/plotter/netperf.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/plotter/ping.py
--rw-rw-rw-   0 root         (0) root         (0)     7558 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/plotter/ss.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2021-11-01 14:30:09.000000 nest-0.4.1/nest/experiment/plotter/tc.py
--rw-rw-rw-   0 root         (0) root         (0)     7441 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/results.py
--rw-rw-rw-   0 root         (0) root         (0)    18118 2022-03-14 15:34:55.000000 nest-0.4.1/nest/experiment/run_exp.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2021-06-20 07:10:57.000000 nest-0.4.1/nest/global_variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/input_validator/
--rw-rw-rw-   0 root         (0) root         (0)     1702 2022-03-14 15:34:55.000000 nest-0.4.1/nest/input_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2022-03-14 15:34:55.000000 nest-0.4.1/nest/input_validator/input_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     3344 2022-03-14 15:34:55.000000 nest-0.4.1/nest/input_validator/metric.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2022-03-14 15:34:55.000000 nest-0.4.1/nest/input_validator/typing_helper_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     4832 2022-03-14 15:34:55.000000 nest-0.4.1/nest/logging_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2022-03-14 15:34:55.000000 nest-0.4.1/nest/network_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.994598 nest-0.4.1/nest/routing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-20 07:10:57.000000 nest-0.4.1/nest/routing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2021-06-20 07:10:57.000000 nest-0.4.1/nest/routing/isis.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2022-03-14 15:34:55.000000 nest-0.4.1/nest/routing/ldp.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2021-10-10 07:01:32.000000 nest-0.4.1/nest/routing/ospf.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2021-06-20 07:10:57.000000 nest-0.4.1/nest/routing/rip.py
--rw-rw-rw-   0 root         (0) root         (0)     4151 2022-03-14 15:34:55.000000 nest-0.4.1/nest/routing/route_daemons.py
--rw-rw-rw-   0 root         (0) root         (0)    10963 2022-03-14 15:34:55.000000 nest-0.4.1/nest/routing/routing_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2021-06-20 07:10:57.000000 nest-0.4.1/nest/routing/zebra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.998597 nest-0.4.1/nest/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-10-16 07:11:42.000000 nest-0.4.1/nest/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4705 2021-11-01 14:30:09.000000 nest-0.4.1/nest/tests/test_address_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4056 2022-03-14 15:34:55.000000 nest-0.4.1/nest/tests/test_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2022-03-14 15:34:55.000000 nest-0.4.1/nest/tests/test_input_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2021-11-01 14:30:09.000000 nest-0.4.1/nest/tests/test_offload.py
--rw-rw-rw-   0 root         (0) root         (0)     2152 2022-02-15 16:49:22.000000 nest-0.4.1/nest/tests/test_routing_frr.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2022-02-15 16:49:22.000000 nest-0.4.1/nest/tests/test_routing_frr_ipv6.py
--rw-rw-rw-   0 root         (0) root         (0)     3179 2022-03-14 15:34:55.000000 nest-0.4.1/nest/tests/test_routing_quagga.py
--rw-rw-rw-   0 root         (0) root         (0)     2307 2022-02-15 16:49:22.000000 nest-0.4.1/nest/tests/test_routing_quagga_ipv6.py
--rw-rw-rw-   0 root         (0) root         (0)     2379 2021-11-01 14:30:09.000000 nest-0.4.1/nest/tests/test_static_routing_mpls.py
--rw-rw-rw-   0 root         (0) root         (0)     8093 2022-03-14 15:34:55.000000 nest-0.4.1/nest/tests/test_topology.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2021-06-20 07:10:57.000000 nest-0.4.1/nest/tests/test_topology_address.py
--rw-rw-rw-   0 root         (0) root         (0)     2846 2021-06-20 07:10:57.000000 nest-0.4.1/nest/tests/test_topology_address_ipv6.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2021-06-20 07:10:57.000000 nest-0.4.1/nest/tests/test_topology_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.998597 nest-0.4.1/nest/topology/
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7830 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/address.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/address_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7732 2021-11-07 08:47:45.000000 nest-0.4.1/nest/topology/device.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2021-06-20 07:10:57.000000 nest-0.4.1/nest/topology/id_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     4028 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/ifb.py
--rw-rw-rw-   0 root         (0) root         (0)    14940 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/network.py
--rw-rw-rw-   0 root         (0) root         (0)    11782 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/node.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2021-11-01 14:30:09.000000 nest-0.4.1/nest/topology/switch.py
--rw-rw-rw-   0 root         (0) root         (0)    11634 2021-11-07 08:47:45.000000 nest-0.4.1/nest/topology/traffic_control.py
--rw-rw-rw-   0 root         (0) root         (0)     7242 2022-03-14 15:34:55.000000 nest-0.4.1/nest/topology/veth_end.py
--rw-rw-rw-   0 root         (0) root         (0)    10319 2021-11-01 14:30:09.000000 nest-0.4.1/nest/topology_map.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2021-06-20 07:10:57.000000 nest-0.4.1/nest/user.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-03-14 15:34:55.000000 nest-0.4.1/nest/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 16:08:19.990597 nest-0.4.1/nest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2718 2022-03-14 16:08:19.000000 nest-0.4.1/nest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2726 2022-03-14 16:08:19.000000 nest-0.4.1/nest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-14 16:08:19.000000 nest-0.4.1/nest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-03-14 16:08:19.000000 nest-0.4.1/nest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-03-14 16:08:19.000000 nest-0.4.1/nest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-14 16:08:19.998597 nest-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1933 2022-03-14 15:34:55.000000 nest-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.725460 nest-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-02 15:53:23.000000 nest-0.4.2/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)    15220 2022-07-30 05:06:43.000000 nest-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-07-03 17:53:31.725460 nest-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2022-07-30 05:06:43.000000 nest-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.709459 nest-0.4.2/nest/
+-rw-rw-rw-   0 root         (0) root         (0)     2102 2022-10-26 03:53:35.000000 nest-0.4.2/nest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-06-29 03:38:37.000000 nest-0.4.2/nest/clean_up.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-25 19:03:10.000000 nest-0.4.2/nest/config.json
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2023-06-29 03:38:37.000000 nest-0.4.2/nest/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.713459 nest-0.4.2/nest/engine/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-12 03:51:00.000000 nest-0.4.2/nest/engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/coap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8282 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/coap_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/coap_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     5643 2023-02-23 21:33:30.000000 nest-0.4.2/nest/engine/dynamic_routing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/ethtool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4974 2022-10-25 13:08:35.000000 nest-0.4.2/nest/engine/exec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/ip_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     4149 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/ip_link.py
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/ip_mpls_route.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/ip_netns.py
+-rw-rw-rw-   0 root         (0) root         (0)     2825 2023-06-29 03:38:37.000000 nest-0.4.2/nest/engine/ip_route.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2023-04-25 19:03:10.000000 nest-0.4.2/nest/engine/iperf3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2022-10-26 03:53:35.000000 nest-0.4.2/nest/engine/ipv6_states.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/iterators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-04-25 19:03:10.000000 nest-0.4.2/nest/engine/netperf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/ping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/setns.py
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-06-29 03:38:37.000000 nest-0.4.2/nest/engine/sysctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-06-29 03:38:37.000000 nest-0.4.2/nest/engine/t_shark.py
+-rw-rw-rw-   0 root         (0) root         (0)     7956 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/tc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/tcp_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/uname.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2022-07-30 05:06:43.000000 nest-0.4.2/nest/engine/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2022-07-30 05:06:43.000000 nest-0.4.2/nest/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.713459 nest-0.4.2/nest/experiment/
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13944 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/experiment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.713459 nest-0.4.2/nest/experiment/info/
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2023-03-12 09:43:31.000000 nest-0.4.2/nest/experiment/info/README.txt
+-rw-rw-rw-   0 root         (0) root         (0)      846 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/interrupts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/pack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.713459 nest-0.4.2/nest/experiment/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2023-01-31 18:25:10.000000 nest-0.4.2/nest/experiment/parser/coap.py
+-rw-rw-rw-   0 root         (0) root         (0)    15740 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/parser/iperf3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.717459 nest-0.4.2/nest/experiment/parser/iterators/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/parser/iterators/ss.sh
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/parser/iterators/tc.sh
+-rw-rw-rw-   0 root         (0) root         (0)     6646 2023-04-25 19:03:10.000000 nest-0.4.2/nest/experiment/parser/netperf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-01-31 18:25:10.000000 nest-0.4.2/nest/experiment/parser/ping.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2022-10-26 03:53:35.000000 nest-0.4.2/nest/experiment/parser/runnerbase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6795 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/parser/ss.py
+-rw-rw-rw-   0 root         (0) root         (0)    12278 2023-01-31 18:25:10.000000 nest-0.4.2/nest/experiment/parser/tc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.717459 nest-0.4.2/nest/experiment/plotter/
+-rw-rw-rw-   0 root         (0) root         (0)      520 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/plotter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-03-12 09:43:31.000000 nest-0.4.2/nest/experiment/plotter/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3583 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/plotter/iperf3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3122 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/plotter/netperf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/plotter/ping.py
+-rw-rw-rw-   0 root         (0) root         (0)     7561 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/plotter/ss.py
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2022-07-30 05:06:43.000000 nest-0.4.2/nest/experiment/plotter/tc.py
+-rw-rw-rw-   0 root         (0) root         (0)     9563 2023-04-14 16:07:41.000000 nest-0.4.2/nest/experiment/results.py
+-rw-rw-rw-   0 root         (0) root         (0)    26589 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/run_exp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6307 2023-06-29 03:38:37.000000 nest-0.4.2/nest/experiment/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2022-07-30 05:06:43.000000 nest-0.4.2/nest/global_variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.717459 nest-0.4.2/nest/input_validator/
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2022-07-30 05:06:43.000000 nest-0.4.2/nest/input_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5629 2022-07-30 05:06:43.000000 nest-0.4.2/nest/input_validator/input_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5734 2022-07-30 05:06:43.000000 nest-0.4.2/nest/input_validator/metric.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2022-07-30 05:06:43.000000 nest-0.4.2/nest/input_validator/typing_helper_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     4820 2022-07-30 05:06:43.000000 nest-0.4.2/nest/logging_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2022-10-26 03:53:35.000000 nest-0.4.2/nest/network_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.717459 nest-0.4.2/nest/routing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-30 05:06:43.000000 nest-0.4.2/nest/routing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2022-10-26 03:53:35.000000 nest-0.4.2/nest/routing/isis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2022-10-26 03:53:35.000000 nest-0.4.2/nest/routing/ldp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4364 2023-01-31 18:25:10.000000 nest-0.4.2/nest/routing/ospf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2023-01-31 18:25:10.000000 nest-0.4.2/nest/routing/rip.py
+-rw-rw-rw-   0 root         (0) root         (0)     4674 2023-01-31 18:25:10.000000 nest-0.4.2/nest/routing/route_daemons.py
+-rw-rw-rw-   0 root         (0) root         (0)    14670 2023-02-02 06:40:02.000000 nest-0.4.2/nest/routing/routing_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2022-07-30 05:06:43.000000 nest-0.4.2/nest/routing/static_routing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2022-10-26 03:53:35.000000 nest-0.4.2/nest/routing/zebra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.721460 nest-0.4.2/nest/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6246 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_address_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7928 2023-06-29 03:38:37.000000 nest-0.4.2/nest/tests/test_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_input_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8361 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_iperf3_server_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_offload.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-01-31 18:25:10.000000 nest-0.4.2/nest/tests/test_routing_bird_ipv4.py
+-rw-rw-rw-   0 root         (0) root         (0)     3613 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_routing_frr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_routing_frr_ipv6.py
+-rw-rw-rw-   0 root         (0) root         (0)     4095 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_routing_frr_multi_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_routing_quagga.py
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_routing_quagga_ipv6.py
+-rw-rw-rw-   0 root         (0) root         (0)     3995 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_routing_quagga_multi_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_static_routing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_static_routing_mpls.py
+-rw-rw-rw-   0 root         (0) root         (0)    18781 2022-11-26 08:38:23.000000 nest-0.4.2/nest/tests/test_topology.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_topology_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     2846 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_topology_address_ipv6.py
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_topology_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2022-10-26 03:53:35.000000 nest-0.4.2/nest/tests/test_topology_map_thread_safety.py
+-rw-rw-rw-   0 root         (0) root         (0)     4009 2023-06-29 03:38:37.000000 nest-0.4.2/nest/tests/test_topology_packet_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2022-07-30 05:06:43.000000 nest-0.4.2/nest/tests/test_topology_ping_preload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.721460 nest-0.4.2/nest/topology/
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7830 2022-07-30 05:06:43.000000 nest-0.4.2/nest/topology/address.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/address_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.721460 nest-0.4.2/nest/topology/device/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-07-30 05:06:43.000000 nest-0.4.2/nest/topology/device/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/device/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)    18919 2023-06-29 03:38:37.000000 nest-0.4.2/nest/topology/device/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3962 2023-06-29 03:38:37.000000 nest-0.4.2/nest/topology/device/ifb.py
+-rw-rw-rw-   0 root         (0) root         (0)    12179 2023-06-29 03:38:37.000000 nest-0.4.2/nest/topology/device/traffic_control.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2022-07-30 05:06:43.000000 nest-0.4.2/nest/topology/device/veth_end.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/id_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.725460 nest-0.4.2/nest/topology/interface/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20740 2023-04-25 19:03:10.000000 nest-0.4.2/nest/topology/interface/base_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/interface/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/network.py
+-rw-rw-rw-   0 root         (0) root         (0)    15702 2023-06-29 03:38:37.000000 nest-0.4.2/nest/topology/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-06-29 03:38:37.000000 nest-0.4.2/nest/topology/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology/switch.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2022-10-26 03:53:35.000000 nest-0.4.2/nest/topology_map.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2022-07-30 05:06:43.000000 nest-0.4.2/nest/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-02 16:13:47.000000 nest-0.4.2/nest/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 17:53:31.709459 nest-0.4.2/nest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-07-03 17:53:31.000000 nest-0.4.2/nest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-07-03 17:53:31.000000 nest-0.4.2/nest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 17:53:31.000000 nest-0.4.2/nest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-03 17:53:31.000000 nest-0.4.2/nest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-03 17:53:31.000000 nest-0.4.2/nest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 17:53:31.725460 nest-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2023-04-25 19:03:10.000000 nest-0.4.2/setup.py
```

### Comparing `nest-0.4.1/AUTHORS.txt` & `nest-0.4.2/AUTHORS.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,62 @@
+Aashish Prateek <prateek2720@gmail.com>
+Abhinaba Rakshit <abhinaba.fbr@gmail.com>
 Aditya Sohoni <adityasohoni@gmail.com>
+Ajay Hajare <ajayghajare@gmail.com>
+Akshay Dhayal <akshaydhayalkd99@gmail.com>
+Alan Tony <alantonye@gmail.com>
+Ankush Chandra <ankushchandra.181co206@nitk.edu.in>
+Arnav Nair <arnavnair13@gmail.com>
 Ayushi Jain <ajain3765@gmail.com>
 Balaji Naidu <balajinaidu.191ec111@nitk.edu.in>
+Bhavya Geetanjali <geetanjalijorige.191cs125@nitk.edu.in>
+Chaitanya Samal <chaitanyasamal12@gmail.com>
+Dayma Khan <daymakhan23@gmail.com>
 Dhanasekhar <dhanasekhar1699@gmail.com>
+Dhanwin Rao <dhanwinrao18@gmail.com>
 Dheeraj Kumar Srivastava <dksri1996@gmail.com>
 Divya Meena <18divya06@gmail.com>
 Felipe Murakami <fhmurakami@gmail.com>
 Himanshu Kashyap <himanshukashyap1122@gmail.com>
+Ikjot Singh Dhody <ikjotsd@gmail.com>
+Irfan Backer <irfanbacker@hotmail.com>
+Ishaan Singh <asishaan.191cs124@nitk.edu.in>
 Jay Rathod <jay.m.rathod.01@gmail.com>
+Ketan Ganvit <ketanganvit112@gmail.com>
+Kinshuk Kashyap <kinshuk.181it222@nitk.edu.in>
+Kruthika K Sudhama <kruthikaksudhama@gmail.com>
+Mithilesh Kannojiya <mithileshkannojiya@gmail.com>
 Mohit P. Tahiliani <tahiliani.nitk@gmail.com>
 Narayan G <gnarayang@gmail.com>
+Niranjan S Yadiyala <niranjan.sy99@gmail.com>
+Nuthan Kumar S <nuthankumars10@gmail.com>
+Pallavi Gupta <pallavijan947@gmail.com>
 Piyush Kumar Mishra <piyushkumarm868@gmail.com>
 Pranab Nandy <nandypranab3@gmail.com>
+Pranav Joshi <pranavjoshixavierite@gmail.com>
+Pranav Kumar <pranavnkps@gmail.com>
+Priyanka G Pai <pgp.191cs236@nitk.edu.in>
+Rahul Kumar <rahulkr.191cs239@nitk.edu.in>
+Rahul Roy <rahul741222@gmail.com>
+Raj Kumar Raj <ravishraj12@gmail.com>
 Rohan B. Rangari <rrangari94@gmail.com>
 Rohit M P <rohitmp99@gmail.com>
+Rohit Parihar <rohit.191cs245@nitk.edu.in>
+Sachin Shivaji Doddamani <ronhartforddelta19@gmail.com>
 Sadik Dange <sadikdange25@gmail.com>
+Sai Krishna Anand <saikrishna001207@gmail.com>
 Sai Sree Harsha <sreesai1412@gmail.com>
 Satyam Prakash <satyamprakash2828@gmail.com>
 Saurabhkumar Desale <saurabhkumardesale@gmail.com>
 Shanthanu S Rai <shanthanu.s.rai9@gmail.com>
 Shashank D <shashankindiamanoj@gmail.com>
+Shelley Tated <tatedshelley@gmail.com>
+Shivangi Tomar <geegatomar@gmail.com>
+Shreesha Bharadwaj <bharadwajshreesha@gmail.com>
+Shreyash Waghmare <shreyash210299@gmail.com>
+Suhas K S <suhasks123@gmail.com>
 Swati Singh <swatikdma@gmail.com>
 Urvesh Rathod <urveshrathod25@gmail.com>
 Vanessa Fernandes <vanessafernandes.201it164@nitk.edu.in>
+Vashung Muilung <vashungm@gmail.com>
+Vignesh Srinivasan <vignesh1722@gmail.com>
 Vinayak Prakashan Choyyan <pcvinayak1234@gmail.com>
```

### Comparing `nest-0.4.1/LICENSE` & `nest-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/PKG-INFO` & `nest-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: nest
-Version: 0.4.1
+Version: 0.4.2
 Summary: NeST: Network Stack Tester
 Home-page: https://nest.nitk.ac.in/
 Author: NITK
 Author-email: nest@nitk.edu.in
-License: UNKNOWN
 Project-URL: Source, https://gitlab.com/nitk-nest/nest
 Keywords: network,namespace,linux
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
@@ -70,9 +68,7 @@
 ```
 
 **NOTE**: NeST requires **root** access currently to create and manage network namespaces.
 
 ## Contributing
 
 To contribute, read [CONTRIBUTING.md](https://gitlab.com/nitk-nest/nest/-/blob/master/CONTRIBUTING.md)
-
-
```

### Comparing `nest-0.4.1/README.md` & `nest-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/__init__.py` & `nest-0.4.2/nest/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 """
 
 import logging
 import os
 import sys
 import signal
 
-from nest import clean_up
 from .logging_helper import add_logging_level, get_trace_filehandler
 from .user import User
 from . import config
 
 # Set high logging level so that logs aren't printed
 # if user is not running as root
 nest_logger = logging.getLogger(__name__)
@@ -58,12 +57,16 @@
     lambda record: record.levelno != logging.TRACE
 )  # To avoid engine commands to be printed to stdout
 nest_logger.addHandler(ch)
 
 if log_level == "TRACE":
     nest_logger.addHandler(get_trace_filehandler())
 
+# Moving import here, since it's causing issues with running
+# NeST without sudo privilege
+from nest import clean_up  # # pylint: disable=wrong-import-position, wrong-import-order
+
 # On recieving Termination signal, execute the given function
 signal.signal(signal.SIGTERM, clean_up.delete_namespaces)
 
 # Load custom config values
 config.search_config_files()
```

### Comparing `nest-0.4.1/nest/config.py` & `nest-0.4.2/nest/config.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/dynamic_routing.py` & `nest-0.4.2/nest/engine/dynamic_routing.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """Routing commands"""
 from os import path
 from nest.engine.util import is_dependency_installed
 from .. import config
 from .exec import exec_subprocess
 
-
 # Path to routing_suite daemon binaries
 FRR_DAEMONPATH = "/usr/lib/frr/"
 
 
 def run_zebra(ns_id, conf_file, pid_file):
     """
     Runs the zebra daemon
@@ -23,52 +22,60 @@
     conf_file : str
         path to config file
     pid_file : str
         path to pid file
     """
     if config.get_value("routing_suite") == "frr":
         cmd = f"ip netns exec {ns_id} {FRR_DAEMONPATH}zebra --config_file {conf_file} \
-                --pid_file {pid_file} --retain --daemon -N {ns_id}"
+                --pid_file {pid_file} --vrfwnetns --retain --daemon -N {ns_id}"
     else:
         cmd = f"ip netns exec {ns_id} zebra --config_file {conf_file} \
                 --pid_file {pid_file} --retain --daemon"
     exec_subprocess(cmd)
 
 
-def run_ripd(ns_id, conf_file, pid_file, ipv6):
+def run_ripd(ns_id, conf_file, pid_file, ipv6, **kwargs):
     """
     Runs the ripd daemon
 
     Parameters
     ----------
     ns_id : str
         namespace of the router
     conf_file : str
         path to config file
     pid_file : str
         path to pid file
     """
+
     if config.get_value("routing_suite") == "frr":
         if ipv6:
             cmd = f"ip netns exec {ns_id} {FRR_DAEMONPATH}ripngd --config_file {conf_file} \
                     --pid_file {pid_file} --daemon -N {ns_id}"
         else:
             cmd = f"ip netns exec {ns_id} {FRR_DAEMONPATH}ripd --config_file {conf_file} \
                     --pid_file {pid_file} --daemon -N {ns_id}"
+    elif config.get_value("routing_suite") == "bird":
+        if config.get_value("routing_logs"):
+            cmd = f"ip netns exec {ns_id} bird -c {conf_file} -P {pid_file} \
+                     -s {kwargs['socket_file']} -D {kwargs['log_file']}"
+        else:
+            cmd = f"ip netns exec {ns_id} bird -c {conf_file} -P {pid_file} \
+                    -s {kwargs['socket_file']}"
     else:
         if ipv6:
             cmd = f"ip netns exec {ns_id} ripngd --config_file {conf_file} \
                     --pid_file {pid_file} --retain --daemon"
         else:
             cmd = f"ip netns exec {ns_id} ripd --config_file {conf_file} \
                     --pid_file {pid_file} --retain --daemon"
     exec_subprocess(cmd)
 
 
-def run_ospfd(ns_id, conf_file, pid_file, ipv6):
+def run_ospfd(ns_id, conf_file, pid_file, ipv6, **kwargs):
     """
     Runs the ospfd daemon
 
     Parameters
     ----------
     ns_id : str
         namespace of the router
@@ -80,14 +87,21 @@
     if config.get_value("routing_suite") == "frr":
         if ipv6:
             cmd = f"ip netns exec {ns_id} {FRR_DAEMONPATH}ospf6d --config_file {conf_file} \
                 --pid_file {pid_file} --daemon -N {ns_id}"
         else:
             cmd = f"ip netns exec {ns_id} {FRR_DAEMONPATH}ospfd --config_file {conf_file} \
                 --pid_file {pid_file} --daemon -N {ns_id}"
+    elif config.get_value("routing_suite") == "bird":
+        if config.get_value("routing_logs"):
+            cmd = f"ip netns exec {ns_id} bird -c {conf_file} -P {pid_file} \
+                -s {kwargs['socket_file']} -D {kwargs['log_file']}"
+        else:
+            cmd = f"ip netns exec {ns_id} bird -c {conf_file} -P {pid_file} \
+                -s {kwargs['socket_file']}"
     else:
         if ipv6:
             cmd = f"ip netns exec {ns_id} ospf6d --config_file {conf_file} \
             --pid_file {pid_file} --daemon"
         else:
             cmd = f"ip netns exec {ns_id} ospfd --config_file {conf_file} \
                 --pid_file {pid_file} --daemon"
@@ -136,28 +150,31 @@
         exec_subprocess(cmd)
     else:
         raise Exception("Ldp requires Frrouting")
 
 
 def supports_dynamic_routing(daemon):
     """
-    Checks whether frr/quagga is installed
+    Checks whether frr/quagga/bird is installed
 
     Parameters
     ----------
     daemon : str
         routing daemon
 
     Returns
     -------
     bool
-        true if frr/quagga is installed
+        true if frr/quagga/bird is installed
     """
 
-    if config.get_value("routing_suite") == "quagga":
+    if (
+        config.get_value("routing_suite") == "quagga"
+        or config.get_value("routing_suite") == "bird"
+    ):
         return is_dependency_installed(daemon)
 
     if config.get_value("routing_suite") == "frr":
         # /usr/lib/ is the default installation path for frr which is not in PATH.
         # This results in `is_dependency_installed` always returning false for frr, hence we
         # check if the daemon binary exists
         return path.isfile(f"{FRR_DAEMONPATH}{daemon}")
```

### Comparing `nest-0.4.1/nest/engine/ethtool.py` & `nest-0.4.2/nest/engine/ethtool.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/exec.py` & `nest-0.4.2/nest/engine/coap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,80 @@
 # SPDX-License-Identifier: GPL-2.0-only
-# Copyright (c) 2019-2020 NITK Surathkal
+# Copyright (c) 2019-2022 NITK Surathkal
 
-"""Execute Linux commands"""
+"""CoAP commands"""
 
-import logging
-import shlex
-import subprocess
-from subprocess import Popen, PIPE
+import os
 
+from .exec import exec_exp_commands, exec_subprocess_in_background
 
-logger = logging.getLogger(__name__)
-
-# pylint: disable=inconsistent-return-statements
-def exec_subprocess(cmd, shell=False, output=False):
+# pylint: disable=too-many-arguments
+def run_coap_client(ns_name, destination_ip, ipv6, coap_options, out, err):
     """
-    Executes a command
+    Run CoAP client program
 
     Parameters
     ----------
-    cmd : str
-        command to be executed
-    shell : boolean
-        Spawns a shell and executes the command if true
-        (Default value = False)
-    output : boolean
-        True if the output of the `cmd` is to be returned
-        (Default value = False)
+    ns_name : str
+        Name of the client namespace
+    destination_ip : str
+        IP address of the destination namespace
+    ipv6 : bool
+        Indicates whether the IP address is IPv6 or not
+    coap_options : str
+        Options string for running the CoAP client application
+    out : File
+        temporary file to hold the stats
+    err : File
+        temporary file to hold any errors
 
     Returns
     -------
     int
-        Return code received after executing the command
-    """
-
-    # TODO: Commands with pipes are easily executed when
-    # they are run within a shell.
-    # But it may not be the most efficient way.
-
-    temp_cmd = cmd
-    if shell is False:
-        temp_cmd = cmd.split()
-
-    with Popen(temp_cmd, stdout=PIPE, stderr=PIPE, shell=shell) as proc:
-
-        (stdout, _) = proc.communicate()
-        logger.trace(cmd)
-
-        if output:
-            return stdout.decode()
-        return proc.returncode
-
-
-def exec_subprocess_with_live_output(cmd):
+        return code of the command executed
     """
-    Executes command and prints live output to stdout.
-
-    For eg., if ping command is used, then the output for each
-    packet is printed live to stdout.
-
-    Parameters
-    ----------
-    cmd : str
-        Command to be executed
-
-    Returns
-    -------
-    int
-        Return code recieved after executing the command
-    """
-    # Inspired from:
-    # https://fabianlee.org/2019/09/15/python-getting-live-output-from-subprocess-using-poll/
-
-    with Popen(cmd.split(), stdout=PIPE) as process:
-        while True:
-            output = process.stdout.readline()
-            if process.poll() is not None:
-                break
-            if output:
-                print(output.decode(), end="")
-
-        # Print an extra newline at the end
-        print()
-        logger.trace(cmd)
-        return process.poll()
+    # Here, the path to the current file being run `coap.py` is taken
+    # and used to run `coap_client.py` in the same directory. This is
+    # done using the `__file__` dunder variable and the `os` library.
+    path_to_curr_module = os.path.dirname(os.path.abspath(__file__))
+    path_to_client = path_to_curr_module + "/coap_client.py"
+
+    # If destination address is IPv6, check
+    # if square brackets are present to use it as
+    # a hostname. If not, add square brackets.
+    if ipv6:
+        if destination_ip[0] != "[":
+            destination_ip = "[" + destination_ip + "]"
+
+    return exec_exp_commands(
+        f"ip netns exec {ns_name} python3 {path_to_client} -d {destination_ip} {coap_options}",
+        stdout=out,
+        stderr=err,
+    )
 
 
-def exec_exp_commands(cmd, stdout=PIPE, stderr=PIPE, timeout=None):
+def run_coap_server(ns_name, server_options):
     """
-    executes experiment related commands like ss, tc and netperf
+    Run CoAP server program
 
     Parameters
     ----------
-    cmd : str
-        command to be executed
-    stdout : File
-        temp file(usually) to store the output (Default value = subprocess.PIPE)
-    stderr : File
-        temp file(usually) to store errors, if any (Default value = subprocess.PIPE)
-    timeout :
-         (Default value = None)
+    ns_name : str
+        Name of the server namespace
+    server_options : str
+        Options string for running the server process
 
     Returns
     -------
     int
-        Return code recieved after executing the command
+        return code of the command executed
     """
-    with Popen(shlex.split(cmd), stdout=stdout, stderr=stderr) as proc:
-        logger.trace(cmd)
-        try:
-            proc.communicate(timeout=timeout)
-        except subprocess.TimeoutExpired:
-            proc.kill()
-            stderr.write(b"Connection timeout")
-        return proc.returncode
+    # Here, the path to the current file being run `coap.py` is taken
+    # and used to run `coap_server.py` in the same directory. This is
+    # done using the `__file__` dunder variable and the `os` library.
+    path_to_curr_module = os.path.dirname(os.path.abspath(__file__))
+    path_to_server = path_to_curr_module + "/coap_server.py"
+
+    return exec_subprocess_in_background(
+        f"ip netns exec {ns_name} python3 -u {path_to_server} {server_options}",
+        shell=True,
+    )
```

### Comparing `nest-0.4.1/nest/engine/ip_address.py` & `nest-0.4.2/nest/engine/ip_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,40 @@
 """IP address commands"""
 
 from .exec import exec_subprocess
 
 
 def assign_ip(host_name, dev_name, ip_address):
     """
-    Assigns ip address to interface
+    Assigns(or adds) an ip address to interface
 
     Parameters
     ----------
     host_name : str
         name of the host namespace
     dev_name : str
         name of the interface
     ip_address : str
         ip address to be assigned to the interface
     """
-    # TODO: Support for IPv6
+
     exec_subprocess(
         f"ip netns exec {host_name} ip address add {ip_address} dev {dev_name}"
     )
+
+
+def delete_ip(host_name, dev_name, ip_address):
+    """
+    Deletes an ip address which was assigned to the interface
+
+    Parameters
+    ----------
+    host_name : str
+        name of the host namespace
+    dev_name : str
+        name of the interface
+    ip_address : str
+        ip address to be assigned to the interface
+    """
+    exec_subprocess(
+        f"ip netns exec {host_name} ip address del {ip_address} dev {dev_name}"
+    )
```

### Comparing `nest-0.4.1/nest/engine/ip_link.py` & `nest-0.4.2/nest/engine/ip_link.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/ip_mpls_route.py` & `nest-0.4.2/nest/engine/ip_mpls_route.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/ip_netns.py` & `nest-0.4.2/nest/engine/ip_netns.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/iperf3.py` & `nest-0.4.2/nest/engine/iperf3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """iperf commands"""
 
-from .exec import exec_subprocess, exec_exp_commands
+from .exec import exec_exp_commands
 
 
-def run_iperf_server(ns_name):
+def run_iperf_server(ns_name, server_options, out, err):
     """
     Run Iperf Server on a namesapce
 
     Parameters
     ----------
     ns_name : str
         name of the server namespace
+    server_options : str
+        Specific options (like port_no, interval ) to run iperf3 command with
+    out : File
+        temporary file to hold the stats
+    err : File
+        temporary file to hold any errors
+
+    Returns
+    -------
+    int
+        return code of the command executed
     """
-    # Runs server as a daemon
-    return exec_subprocess(f"ip netns exec {ns_name} iperf3 -s -D")
+    # Runs server
+    return_code = exec_exp_commands(
+        f"ip netns exec {ns_name} iperf3 -s {server_options}", stdout=out, stderr=err
+    )
+    # return code 1 denotes that server is terminated at the end of experiment by cleaning process
+    # so it is not an error.
+    if return_code == 1:
+        return_code = 0
+    return return_code
 
 
 # pylint: disable=too-many-arguments
 def run_iperf_client(ns_name, iperf3_options, destination_ip, ipv6, out, err):
     """
     Run Iperf Client
 
@@ -42,17 +60,17 @@
     Returns
     -------
     int
         return code of the command executed
     """
     if ipv6:
         return exec_exp_commands(
-            f"ip netns exec {ns_name} iperf3 -6 -u -c {destination_ip} {iperf3_options}",
+            f"ip netns exec {ns_name} iperf3 -6 -c {destination_ip} {iperf3_options}",
             stdout=out,
             stderr=err,
         )
 
     return exec_exp_commands(
-        f"ip netns exec {ns_name} iperf3 -u -c {destination_ip} {iperf3_options}",
+        f"ip netns exec {ns_name} iperf3 -c {destination_ip} {iperf3_options}",
         stdout=out,
         stderr=err,
     )
```

### Comparing `nest-0.4.1/nest/engine/ipv6_states.py` & `nest-0.4.2/nest/engine/ipv6_states.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: GPL-2.0-only
-# Copyright (c) 2019-2020 NITK Surathkal
+# Copyright (c) 2019-2022 NITK Surathkal
 
 """IPv6 States Check"""
 
 from .exec import exec_subprocess
 
 
 def check_ipv6_states(namespaces):
```

### Comparing `nest-0.4.1/nest/engine/iterators.py` & `nest-0.4.2/nest/engine/iterators.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/netperf.py` & `nest-0.4.2/nest/engine/netperf.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/ping.py` & `nest-0.4.2/nest/engine/ping.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """Ping command"""
 
 from .exec import exec_exp_commands, exec_subprocess, exec_subprocess_with_live_output
 
-
-def ping(ns_name, dest_addr, packets=1, ipv6=False, live_output=True):
+# pylint: disable=too-many-arguments
+def ping(ns_name, dest_addr, preload=1, packets=1, ipv6=False, live_output=True):
     """
     Send a ping packet from ns_name to dest_addr
     if possible
 
     Parameters
     ----------
     ns_name : str
         namespace name
     dest_addr : str
         address to ping to
+    preload: int (Default is 1)
+        Number of packets sent as fast as possible without
+        waiting for reply.
     packets : int
         Number of ping packets sent (default: 1)
     live_output : bool
         Show live output of ping packets
 
     Returns
     -------
     bool
         success of ping
     """
     if live_output:
         if ipv6:
             status = exec_subprocess_with_live_output(
-                f"ip netns exec {ns_name} ping -6 -c {packets} {dest_addr}"
+                f"ip netns exec {ns_name} ping -6 -l {preload} -c {packets} {dest_addr}"
             )
         else:
             status = exec_subprocess_with_live_output(
-                f"ip netns exec {ns_name} ping -c {packets} {dest_addr}"
+                f"ip netns exec {ns_name} ping -l {preload} -c {packets} {dest_addr}"
             )
     else:
         if ipv6:
             status = exec_subprocess(
-                f"ip netns exec {ns_name} ping -6 -c {packets} {dest_addr}"
+                f"ip netns exec {ns_name} ping -6 -l {preload} -c {packets} {dest_addr}"
             )
         else:
             status = exec_subprocess(
-                f"ip netns exec {ns_name} ping -c {packets} {dest_addr}"
+                f"ip netns exec {ns_name} ping -l {preload} -c {packets} {dest_addr}"
             )
     return status == 0
 
 
 # pylint: disable=too-many-arguments
 def run_exp_ping(ns_id, destination_ip, run_time, ipv6, out, err):
     """
```

### Comparing `nest-0.4.1/nest/engine/setns.py` & `nest-0.4.2/nest/engine/setns.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/sysctl.py` & `nest-0.4.2/nest/engine/sysctl.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/engine/tc.py` & `nest-0.4.2/nest/engine/tc.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/experiment.py` & `nest-0.4.2/nest/experiment/parser/netperf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,215 +1,199 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
-"""User API to setup and run experiments on a given topology"""
+"""
+Runs netperf commands to setup TCP flow
+and collect throughput data
+"""
 
+import re
 import copy
 import logging
-from nest.input_validator.metric import Bandwidth
-from nest.network_utilities import ipv6_dad_check
-from nest.input_validator import input_validator
-from nest.topology import Node, Address, Interface
-from .run_exp import run_experiment
-from .pack import Pack
+from time import sleep
+from functools import partial
+from nest.experiment.interrupts import handle_keyboard_interrupt
+from ..results import NetperfResults
+from .runnerbase import Runner
+from ...topology_map import TopologyMap
+from ...engine.netperf import run_netperf, run_netserver
 
 logger = logging.getLogger(__name__)
 
-# pylint: disable=too-many-instance-attributes
-# pylint: disable=too-few-public-methods
-class Flow:
-    """Defines a flow in the topology"""
+
+class NetperfRunner(Runner):
+    """
+    Runs netperf command and parses statistics from its output
+
+    Attributes
+    ----------
+    default_netperf_options : dict
+        default options to run netperf command with
+    netperf_tcp_options : dict
+        tcp related netperf options
+    netperf_udp_options : dict
+        udp related netperf options
+    ns_id : str
+        network namespace to run netperf from
+    destination_ip : str
+        ip address of the destination namespace
+    start_time : num
+        time at which netperf is to run
+    run_time : num
+        total time to run netperf for
+    """
+
+    tcp_output_options = [
+        "THROUGHPUT",
+        "LOCAL_CONG_CONTROL",
+        "REMOTE_CONG_CONTROL",
+        "TRANSPORT_MSS",
+        "LOCAL_SOCKET_TOS",
+        "REMOTE_SOCKET_TOS",
+    ]
+
+    # fmt: off
+
+    default_netperf_options = {
+        "banner": "-P 0",                   # Disable test banner
+        "testname": "-t TCP_STREAM",        # Test type (NOTE: TCP_STREAM only for now)
+        "fill_file": "-F /dev/urandom",     # File to transmit (NOTE: Inspired from flent)
+        "testlen": "-l 10",                 # Length of test (NOTE: Default 10s)
+        "interval": "-D -0.2",              # Generate interim results every INTERVAL secs
+        "debug": "-d",                      # Enable debug mode
+    }
+
+    netperf_tcp_options = {
+        "cong_algo": "-K cubic",            # Congestion algorithm
+        "stats": "-k THROUGHPUT",           # Stats required
+    }
+
+    netperf_udp_options = {
+        "routing": "-R 1",                  # Enable routing
+        "stats": "-k THROUGHPUT",           # Stats required
+    }
+
+    # fmt: on
 
     # pylint: disable=too-many-arguments
-    @input_validator
-    def __init__(
-        self,
-        source_node: Node,
-        destination_node: Node,
-        destination_address: Address,
-        start_time: int,
-        stop_time: int,
-        number_of_streams: int,
-    ):
+    def __init__(self, ns_id, destination_ip, start_time, run_time, dst_ns, **kwargs):
         """
-        'Flow' object in the topology
+        Constructor to initialize netperf runner
 
         Parameters
         ----------
-        source_node : Node
-            Source node of flow
-        destination_node : Node
-            Destination node of flow
-        destination_address : Address/str
-            Destination address of flow
-        start_time : int
-            Time to start flow (in seconds)
-        stop_time : int
-            Time to stop flow (in seconds)
-        number_of_streams : int
-            Number of streams in the flow
-        """
-        self.source_node = source_node
-        self.destination_node = destination_node
-        self.destination_address = destination_address
-        self.start_time = start_time
-        self.stop_time = stop_time
-        self.number_of_streams = number_of_streams
-
-        self._options = {"protocol": "TCP", "cong_algo": "cubic"}
-
-    @property
-    def destination_address(self):
-        """Getter for destination address"""
-        return self._destination_address
-
-    @destination_address.setter
-    def destination_address(self, destination_address):
-        """Setter for destination address"""
-        if isinstance(destination_address, str):
-            destination_address = Address(destination_address)
-        self._destination_address = destination_address
-
-    def _get_props(self):
-        """
-        Get flow properties.
-
-        NOTE: To be used internally
-        """
-
-        return [
-            self.source_node.id,
-            self.destination_node.id,
-            self.destination_address.get_addr(with_subnet=False),
-            self.start_time,
-            self.stop_time,
-            self.number_of_streams,
-            self._options,
-        ]
-
-    def __repr__(self):
-        classname = self.__class__.__name__
-        return (
-            f"{classname}({self.source_node!r}, {self.destination_node!r},"
-            f" {self.destination_address!r}), {self.start_time!r}, {self.stop_time!r}"
-            f" {self.number_of_streams!r})"
-        )
-
-
-class Experiment:
-    """Handles experiment to be run on topology"""
-
-    @input_validator
-    def __init__(self, name: str):
+        ns_id : str
+            network namespace to run netperf from
+        destination_ip : str
+            ip address of the destination namespace
+        start_time : num
+            time at which netperf is to run
+        run_time : num
+            total time to run netperf for
+        dst_ns : str
+            network namespace to run netperf server in
+        **kwargs
+            netperf options to override
         """
-        Create experiment
+        self.options = copy.deepcopy(kwargs)
+        super().__init__(ns_id, start_time, run_time, destination_ip, dst_ns)
 
-        Parameters
-        ----------
-        name : str
-            Name of experiment
+    # Should this be placed somewhere else?
+    @staticmethod
+    def run_netserver(ns_id):
         """
-        self.name = name
-        self.flows = []
-        self.node_stats = []
-        self.qdisc_stats = []
-
-    def add_flow(self, flow):
-        """
-        Add flow to experiment
-        By default, the flow is assumed to be
-        TCP with cubic congestion algorithm
+        Run netserver in `ns_id`
 
         Parameters
         ----------
-        flow : Flow
-            Add flow to experiment
+        ns_id : str
+            namespace to run netserver on
         """
-        self.flows.append(copy.deepcopy(flow))
+        return_code = run_netserver(ns_id)
+        if return_code != 0:
+            ns_name = TopologyMap.get_node(ns_id).name
+            logger.error("Error running netserver at %s.", ns_name)
 
-    @input_validator
-    def add_tcp_flow(self, flow: Flow, congestion_algorithm="cubic"):
+    def run(self):
         """
-        Add TCP flow to experiment. If no congestion control algorithm
-        is specified, then by default cubic is used.
-
-        Note: The congestion control algorithm specified in this API
-        overrides the congestion control algorithm specified in
-        `topology.Node.configure_tcp_param()` API.
-
-        Parameters
-        ----------
-        flow : Flow
-            Flow to be added to experiment
-        congestion_algorithm : str
-            TCP congestion algorithm (Default value = 'cubic')
+        Runs netperf at t=`self.start_time`
         """
+        netperf_options = copy.copy(NetperfRunner.default_netperf_options)
+        test_options = None
 
-        # TODO: Verify congestion algorithm
-
-        options = {"protocol": "TCP", "cong_algo": congestion_algorithm}
+        # Change the default run time
+        netperf_options["testlen"] = f"-l {self.run_time}"
 
-        flow._options = options  # pylint: disable=protected-access
-        self.add_flow(flow)
+        # Set test
+        netperf_options["testname"] = f"-t {self.options['testname']}"
+
+        if netperf_options["testname"] == "-t TCP_STREAM":
+            test_options = copy.copy(NetperfRunner.netperf_tcp_options)
+            test_options["cong_algo"] = f"-K {self.options['cong_algo']}"
+
+        elif netperf_options["testname"] == "-t UDP_STREAM":
+            test_options = copy.copy(NetperfRunner.netperf_udp_options)
+
+        netperf_options_list = list(netperf_options.values())
+        netperf_options_string = " ".join(netperf_options_list)
+        test_options_list = list(test_options.values())
+        test_options_string = " ".join(test_options_list)
+
+        if self.start_time > 0:
+            sleep(self.start_time)
+
+        super().run(
+            partial(
+                run_netperf,
+                self.ns_id,
+                netperf_options_string,
+                self.destination_address.get_addr(with_subnet=False),
+                test_options_string,
+                self.destination_address.is_ipv6(),
+            ),
+            error_string_prefix="Running netperf",
+        )
 
-    @input_validator
-    def add_udp_flow(
-        self, flow: Flow, target_bandwidth: Bandwidth = Bandwidth("1mbit")
-    ):
+    @handle_keyboard_interrupt
+    def parse(self):
         """
-        Add UDP flow to experiment
-
-        Parameters
-        ----------
-        flow : Flow
-            Flow to be added to experiment
-        target_bandwidth :
-            UDP bandwidth (in Mbits) (Default value = '1mbit')
-            This bandwidth limit is for each UDP stream in the flow
+        Parse netperf output from `self.out`
         """
-        options = {"protocol": "UDP", "target_bw": target_bandwidth.string_value}
+        self.out.seek(0)  # rewind to start of the temp file
+        raw_stats = self.out.read().decode()
 
-        flow._options = options  # pylint: disable=protected-access
-        self.add_flow(flow)
+        # pattern that matches the netperf output corresponding to throughput
+        throughput_pattern = r"NETPERF_INTERIM_RESULT\[\d+]=(?P<throughput>\d+\.\d+)"
+        throughputs = [
+            throughput.group("throughput")
+            for throughput in re.finditer(throughput_pattern, raw_stats)
+        ]
 
-    @input_validator
-    def require_qdisc_stats(self, interface: Interface, stats=""):
-        """
-        Stats to be obtained from qdisc in interface
+        # pattern that matches the netperf output corresponding to interval
+        timestamp_pattern = r"NETPERF_ENDING\[\d+]=(?P<timestamp>\d+\.\d+)"
+        timestamps = [
+            timestamp.group("timestamp")
+            for timestamp in re.finditer(timestamp_pattern, raw_stats)
+        ]
 
-        Parameters
-        ----------
-        interface : Interface
-            Interface containing the qdisc
-        stats : list(str)
-            Stats required (Default value = '') [NOT SUPPORTED]
-        """
-        # TODO: Leads to rewrite if the function is called
-        # twice with same 'interface'
-
-        # for stat in stats:
-        #     if stat not in Experiment.qdisc_stats:
-        #         raise ValueError('{} is not a valid Queue property.'.format(stat))
-
-        if interface.get_qdisc() is None:
-            raise ValueError("Given interface hasn't been assigned any qdisc.")
-
-        self.qdisc_stats.append(
-            {
-                "ns_id": interface.node_id,
-                "int_id": interface.ifb_id,
-                "qdisc": interface.get_qdisc().qdisc,
-                "stats": stats,
-            }
-        )
+        # pattern that gives the remote port
+        remote_port_pattern = r"remote port is (?P<remote>\d+)"
+        remote_port = re.search(remote_port_pattern, raw_stats).group("remote")
+
+        # List storing collected stats
+        # First item as "meta" item with user given information
+        stats_list = [self.get_meta_item()]
+
+        # Trim last result, since netperf typically gives unrealisticly high throughput
+        # towards the end
+        for i in range(len(throughputs) - 1):
+            stats_list.append(
+                {
+                    "timestamp": timestamps[i],
+                    # Netperf provides throughput as sending rate from sender's side
+                    "sending_rate": throughputs[i],
+                }
+            )
+        destination_ip = self.destination_address.get_addr(with_subnet=False)
+        stats_dict = {f"{destination_ip}:{remote_port}": stats_list}
 
-    @ipv6_dad_check
-    def run(self):
-        """Run the experiment"""
-        print()
-        logger.info("Running experiment %s ", self.name)
-        Pack.init(self.name)
-        run_experiment(self)
-
-    def __repr__(self):
-        classname = self.__class__.__name__
-        return f"{classname}({self.name!r})"
+        NetperfResults.add_result(self.ns_id, stats_dict)
```

### Comparing `nest-0.4.1/nest/experiment/info/README.txt` & `nest-0.4.2/nest/experiment/info/README.txt`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/interrupts.py` & `nest-0.4.2/nest/experiment/interrupts.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/pack.py` & `nest-0.4.2/nest/experiment/pack.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 
         Parameters
         ----------
         exp_name : str
             Name of experiment
         """
         timestamp = time.strftime("%d-%m-%Y-%H:%M:%S")
-        Pack.FOLDER = "{exp_name}({timestamp})_dump".format(
-            exp_name=exp_name, timestamp=timestamp
-        )
+        Pack.FOLDER = f"{exp_name}({timestamp})_dump"
         os.mkdir(Pack.FOLDER)
         Pack.set_owner(Pack.FOLDER)
 
     @staticmethod
     def dump_file(filename, content):
         """
         Dump a file into Pack.FOLDER
@@ -123,7 +121,30 @@
             dst_path = Pack.FOLDER
         else:
             dst_path = os.path.join(Pack.FOLDER, dst_path)
 
         shutil.copy(src_path, dst_path)
         filename = os.path.join(dst_path, os.path.basename(src_path))
         Pack.set_owner(filename)
+
+    @staticmethod
+    def move_files(src_path, dst_path=None):
+        """
+        Copies file from source to stats folder
+
+        Parameters
+        ----------
+        src_path : str
+            Path of source file
+        dst_path : str
+            Relative Path of destination inside the stats folder
+        """
+
+        if dst_path is None:
+            # Default destination path is stats folder
+            dst_path = Pack.FOLDER
+        else:
+            dst_path = os.path.join(Pack.FOLDER, dst_path)
+
+        shutil.move(src_path, dst_path)
+        filename = os.path.join(dst_path, os.path.basename(src_path))
+        Pack.set_owner(filename)
```

### Comparing `nest-0.4.1/nest/experiment/parser/iterators/ss.sh` & `nest-0.4.2/nest/experiment/parser/iterators/ss.sh`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/parser/ping.py` & `nest-0.4.2/nest/experiment/parser/ping.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/parser/runnerbase.py` & `nest-0.4.2/nest/experiment/parser/runnerbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,45 +65,43 @@
             engine function to be called
         """
         try:
             return_code = engine_func(out=self.out, err=self.err)
             if return_code != 0:
                 self.print_error(error_string_prefix)
         except KeyboardInterrupt:
-            ns_name = TopologyMap.get_namespace(self.ns_id)["name"]
+            ns_name = TopologyMap.get_node(self.ns_id).name
             self.logger.debug(
                 "%s at %s: Received KeyboardInterrupt, hence shutting down the process gracefully.",
                 error_string_prefix,
                 ns_name,
             )
 
     def print_error(self, error_string_prefix):
         """
         Method to print error from `self.err`
         """
         self.err.seek(0)  # rewind to start of file
         error = self.err.read().decode()
-        ns_name = TopologyMap.get_namespace(self.ns_id)["name"]
+        ns_name = TopologyMap.get_node(self.ns_id).name
         self.logger.error("%s at %s. %s", error_string_prefix, ns_name, error)
 
     def get_meta_item(self):
         """
         Return the meta item for the given flow.
         This "meta" information is required by plotter.
         """
         meta_item = {
             "meta": True,
             "start_time": str(self.start_time),
             "stop_time": str(self.start_time + self.run_time),
         }
 
         if self.dst_ns is not None:
-            meta_item["destination_node"] = TopologyMap.get_namespace(self.dst_ns)[
-                "name"
-            ]
+            meta_item["destination_node"] = TopologyMap.get_node(self.dst_ns).name
 
         return meta_item
 
     def __del__(self):
         """
         Close the temp files created
         """
```

### Comparing `nest-0.4.1/nest/experiment/parser/ss.py` & `nest-0.4.2/nest/experiment/parser/ss.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         self.filter = ss_filter
         super().__init__(ns_id, start_time, run_time, destination_ip, dst_ns)
 
     def run(self):
         """
         Runs the ss iterator
         """
-
         super().run(
             partial(
                 run_ss,
                 self.ns_id,
                 SsRunner.iterator,
                 self.destination_address.get_addr(with_subnet=False),
                 self.run_time,
@@ -87,72 +86,92 @@
                 self.start_time,
                 self.destination_address.is_ipv6(),
             ),
             error_string_prefix="Collecting socket stats",
         )
 
     # pylint: disable=too-many-locals
+    # pylint: disable=too-many-branches
     @handle_keyboard_interrupt
     def parse(self):
         """
         parses the required data from `self.out`
         """
         stats_dict_list = {}
 
         self.out.seek(0)  # rewind to start of the temp file
 
         # See `iterators/ss.h` for output format
         raw_stats = self.out.read().decode().split("---")
         destination_ip = self.destination_address.get_addr(with_subnet=False)
 
+        # iperf3 creates 1 additional connection (apart from the N connections
+        # for the N flows specified) every time you run the iperf3 command.
+        # This additional connection is used by iperf3 API iperf for collecting,
+        # sending, and printing intermediate results at specific intervals
+        # (https://github.com/esnet/iperf/blob/master/src/iperf_api.c#L3269).
+        # The ss parser will split each of the raw_stat data in new lines,
+        # and get rid of (ignore) the data from that 1 additional connection
+        # altogether based on the 'ato' parameter (which is present only in the
+        # additional connection that we do not want to collect stats from).
         for raw_stat in raw_stats[:-1]:
 
-            # Pattern to capture port numbers of flows to `destination ip`
-            if self.destination_address.is_ipv6():
-                port_pattern = re.escape(destination_ip) + r"]:(?P<port>\d+)"
-            else:
-                port_pattern = re.escape(destination_ip) + r":(?P<port>\d+)"
-            port_list = [
-                port.group("port") for port in re.finditer(port_pattern, raw_stat)
-            ]
-            timestamp_pattern = r"timestamp:(?P<timestamp>\d+\.\d+)"
-            timestamp = re.search(timestamp_pattern, raw_stat).group("timestamp")
-
-            for port in port_list:
-                # If port encountered first time
-                if port not in stats_dict_list:
-                    stats_dict_list[port] = [self.get_meta_item()]
-
-                stats_dict_list[port].append({"timestamp": timestamp})
-
-            for param in SsRunner.param_list:
-                pattern = (
-                    r"\s"
-                    + re.escape(param)
-                    + r"[\s:](?P<value>\w+\.?\w*(?:[\/\,]\w+\.?\w*)*)\s"
-                )
-                # result list stores all the string that is matched by the `pattern`
-                param_value_list = [
-                    value.group("value") for value in re.finditer(pattern, raw_stat)
-                ]
-                param_value = ""
-                for i in range(len(param_value_list)):
-                    param_value = param_value_list[i].strip()
-                    # remove the (rate) units at the end and convert
+            stats = raw_stat.strip().split("\n")
+            timestamp = stats[0].split(":")[-1]
+            ports_info = []
+            statistics_data = []
+
+            for i, row in enumerate(stats[2:]):
+                if i % 2 == 0:
+                    ports_info.append(row.strip())
+                else:
+                    statistics_data.append(row.strip())
+            assert len(ports_info) == len(statistics_data)
+
+            for i in range(len(ports_info)):
+                # means that this is additional info entries and this data isn't required
+                if "ato" in statistics_data[i]:
+                    continue
+                each_ports_info = ports_info[i].split()
+
+                # means that this entry was not meant for this stat collection
+                if each_ports_info[-1].split(":")[0] != destination_ip:
+                    continue
+
+                dst_port = each_ports_info[-1].split(":")[-1]
+
+                if dst_port not in stats_dict_list:
+                    stats_dict_list[dst_port] = [self.get_meta_item()]
+                stats_dict_list[dst_port].append({"timestamp": timestamp})
+
+                for param in SsRunner.param_list:
+                    pattern = (
+                        r"\s"
+                        + re.escape(param)
+                        + r"[\s:](?P<value>\w+\.?\w*(?:[\/\,]\w+\.?\w*)*)\s"
+                    )
+                    # result list stores all the string that is matched by the `pattern`
+                    try:
+                        param_value = (
+                            re.search(pattern, statistics_data[i]).group(1).strip()
+                        )
+                    except AttributeError:
+                        continue
+
                     if param_value.endswith("bps"):
                         param_value = self.convert_to(param_value)
                     try:
                         # RTT has both average and RTT deviation separated by a /
                         if param == "rtt":
                             avg_rtt = param_value.split("/")[0]
                             dev_rtt = param_value.split("/")[1]
-                            stats_dict_list[port_list[i]][-1]["rtt"] = avg_rtt
-                            stats_dict_list[port_list[i]][-1]["dev_rtt"] = dev_rtt
+                            stats_dict_list[dst_port][-1]["rtt"] = avg_rtt
+                            stats_dict_list[dst_port][-1]["dev_rtt"] = dev_rtt
                         else:
-                            stats_dict_list[port_list[i]][-1][param] = param_value
+                            stats_dict_list[dst_port][-1][param] = param_value
                     except TypeError:
                         pass
 
         destination_ip = self.destination_address.get_addr(with_subnet=False)
         SsResults.add_result(self.ns_id, {destination_ip: stats_dict_list})
 
     @staticmethod
```

### Comparing `nest-0.4.1/nest/experiment/parser/tc.py` & `nest-0.4.2/nest/experiment/parser/tc.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,18 +179,18 @@
         -------
         str
             string to replace the matched string
         """
         if match.group(1):
             if match.group(1).endswith(","):
                 value = repr(match.group(1))
-                return ':"{}",'.format(value)
+                return f':"{value}",'
 
             value = repr(match.group(1))
-            return ':"{}"'.format(value)
+            return f':"{value}"'
         return ""
 
     def clean_json(self, stats):
         """
         JSON formatted tc stats with invalid JSON keys
         and values are removed or fixed
 
@@ -328,14 +328,15 @@
 
         Returns
         -------
         struct_time
             current tc version as date
         """
         cur_tc_version = get_tc_version()
+        # pylint: disable=use-maxsplit-arg
         cur_tc_version = "20" + cur_tc_version.split(" ")[-1][-7:].strip()
         return strptime(cur_tc_version, "%Y%m%d")
 
     @handle_keyboard_interrupt
     def parse(self):
         """
         Parses the required data from tc-qdisc output
@@ -364,9 +365,9 @@
                 qdisc_param = self.get_qdisc_specific_params()
                 qdisc_re = self.get_qdisc_re()
                 aggregate_stats = self.parsing_helper_before_good_json_support(
                     raw_stats, qdisc_param, qdisc_re
                 )
 
         # Store parsed results
-        dev_name = TopologyMap.get_interface(self.ns_id, self.dev)["name"]
+        dev_name = TopologyMap.get_device(self.ns_id, self.dev).name
         TcResults.add_result(self.ns_id, {dev_name: aggregate_stats})
```

### Comparing `nest-0.4.1/nest/experiment/plotter/__init__.py` & `nest-0.4.2/nest/experiment/plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/plotter/common.py` & `nest-0.4.2/nest/experiment/plotter/common.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/plotter/iperf3.py` & `nest-0.4.2/nest/experiment/plotter/iperf3.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         timestamp,
         sending_rate,
         "Time (Seconds)",
         "Sending Rate (Mbps)",
         legend_string=f"{node} from port {local_port} to {destination_node} ({dest_ip})",
     )
 
-    filename = f"sending_rate_{node}_to_{destination_node}({dest_ip}).png"
+    filename = f"sending_rate_{node}({local_port})_to_{destination_node}({dest_ip}).png"
     Pack.dump_plot("iperf3", filename, fig)
     plt.close(fig)
 
 
 # pylint: disable=too-many-locals
 @handle_keyboard_interrupt
 def plot_iperf3(parsed_data):
```

### Comparing `nest-0.4.1/nest/experiment/plotter/netperf.py` & `nest-0.4.2/nest/experiment/plotter/netperf.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/plotter/ping.py` & `nest-0.4.2/nest/experiment/plotter/ping.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/experiment/plotter/ss.py` & `nest-0.4.2/nest/experiment/plotter/ss.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,19 +121,19 @@
     timestamp = []
     flow_params = {}
 
     for param in _get_list_of_ss_params():
         flow_params[param] = []
 
     for data in flow[1:]:
-        for stat in flow_params:
+        for stat, stat_data in flow_params.items():
             if stat in data:
-                flow_params[stat].append(float(data[stat]))
+                stat_data.append(float(data[stat]))
             else:
-                flow_params[stat].append(None)
+                stat_data.append(None)
         relative_time = float(data["timestamp"]) - start_time
         timestamp.append(relative_time)
 
     return {"destination_node": destination_node, "values": (timestamp, flow_params)}
 
 
 def _plot_ss_flow(flow, node, dest_ip, dest_port):
```

### Comparing `nest-0.4.1/nest/experiment/plotter/tc.py` & `nest-0.4.2/nest/experiment/plotter/tc.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     stats_params = {}
 
     for param in stats[0]:
         if param not in ("timestamp", "kind"):
             stats_params[param] = []
 
     for data in stats:
-        for param in stats_params:
-            stats_params[param].append(data[param])
+        for param, param_data in stats_params.items():
+            param_data.append(data[param])
         relative_time = float(data["timestamp"]) - start_time
         timestamp.append(relative_time)
 
     return (qdisc, timestamp, stats_params)
 
 
 def _plot_tc_stats(stats, node, interface):
```

### Comparing `nest-0.4.1/nest/experiment/results.py` & `nest-0.4.2/nest/experiment/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             Shared stats
         ns_id : string
             namespace id (internal name)
         result : dict
             parsed stats
         """
         # Convert nest's internal name to user given name
-        ns_name = TopologyMap.get_namespace(ns_id)["name"]
+        ns_name = TopologyMap.get_node(ns_id).name
 
         item = results_q.get()
         if ns_name not in item:
             item[ns_name] = [result]
         else:
             temp = item[ns_name]
             temp.append(result)
@@ -77,15 +77,15 @@
             Shared stats
         toolname : str
             Like ss, tc, netperf
         """
         results = Results.get_results(results_q)
         if results:
             json_stats = json.dumps(results, indent=4)
-            Pack.dump_file("{}.json".format(toolname), json_stats)
+            Pack.dump_file(f"{toolname}.json", json_stats)
 
 
 # Shared variables to aggregate results
 ss_results_q = Manager().Queue()
 ss_results_q.put({})
 
 
@@ -262,7 +262,80 @@
         """Get results obtained in the experiment so far"""
         return Results.get_results(ping_results_q)
 
     @staticmethod
     def output_to_file():
         """Outputs the aggregated ping stats to file"""
         Results.output_to_file(ping_results_q, "ping")
+
+
+coap_results_q = Manager().Queue()
+coap_results_q.put({})
+
+
+class CoAPResults:
+    """This class aggregates the CoAP stats from the entire experiment environment"""
+
+    @staticmethod
+    def add_result(ns_id, result):
+        """Adds the CoAP stats parse from a process to the shared `coap_results`
+
+        Parameters
+        ----------
+        ns_id : string
+            namespace id (internal name)
+        result : dict
+            parsed CoAP stats
+        """
+        Results.add_result(coap_results_q, ns_id, result)
+
+    @staticmethod
+    def remove_all_results():
+        """Remove all results obtained from the experiment"""
+        Results.remove_all_results(coap_results_q)
+
+    @staticmethod
+    def get_results():
+        """Get results obtained in the experiment so far"""
+        Results.get_results(coap_results_q)
+
+    @staticmethod
+    def output_to_file():
+        """Outputs the aggregated CoAP stats to file"""
+        Results.output_to_file(coap_results_q, "coap")
+
+
+# Shared variables to aggregate results
+iperf3_server_results_q = Manager().Queue()
+iperf3_server_results_q.put({})
+
+
+class Iperf3ServerResults:
+    """This class aggregates the iperf3 server stats from the entire experiment environment"""
+
+    @staticmethod
+    def add_result(ns_id, result):
+        """Adds the iperf3 server stats parsed from a process to the shared `iperf3_server_results`
+
+        Parameters
+        ----------
+        ns_id : string
+            namespace id (internal name)
+        result : dict
+            parsed iperf3 server stats
+        """
+        Results.add_result(iperf3_server_results_q, ns_id, result)
+
+    @staticmethod
+    def remove_all_results():
+        """Remove all results obtained from the experiment"""
+        Results.remove_all_results(iperf3_server_results_q)
+
+    @staticmethod
+    def get_results():
+        """Get results obtained in the experiment so far"""
+        return Results.get_results(iperf3_server_results_q)
+
+    @staticmethod
+    def output_to_file():
+        """Outputs the aggregated iperf3 stats to file"""
+        Results.output_to_file(iperf3_server_results_q, "iperf3Server")
```

### Comparing `nest-0.4.1/nest/experiment/run_exp.py` & `nest-0.4.2/nest/experiment/run_exp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,100 @@
 # SPDX-License-Identifier: GPL-2.0-only
-# Copyright (c) 2019-2020 NITK Surathkal
+# Copyright (c) 2019-2022 NITK Surathkal
 
 """Script to be run for running experiments on topology"""
 
 from multiprocessing import Process
 from collections import namedtuple, defaultdict
 import logging
 import os
 from time import sleep
+import copy
 from tqdm import tqdm
 
 from nest.logging_helper import DepedencyCheckFilter
 from nest import config
 from nest.topology_map import TopologyMap
-from nest.clean_up import kill_processes
+from nest.clean_up import kill_processes, tcp_modules_clean_up
+from nest import engine
 from .pack import Pack
 
 # Import results
-from .results import SsResults, NetperfResults, Iperf3Results, TcResults, PingResults
+from .results import (
+    Iperf3ServerResults,
+    SsResults,
+    NetperfResults,
+    Iperf3Results,
+    TcResults,
+    PingResults,
+    CoAPResults,
+)
 
 # Import parsers
 from .parser.ss import SsRunner
 from .parser.netperf import NetperfRunner
-from .parser.iperf3 import Iperf3Runner
+from .parser.iperf3 import Iperf3Runner, Iperf3ServerRunner
 from .parser.tc import TcRunner
 from .parser.ping import PingRunner
+from .parser.coap import CoAPRunner
 
 # Import plotters
 from .plotter.ss import plot_ss
 from .plotter.netperf import plot_netperf
 from .plotter.iperf3 import plot_iperf3
 from .plotter.tc import plot_tc
 from .plotter.ping import plot_ping
-from ..engine.util import is_dependency_installed
+from ..engine.util import is_dependency_installed, is_package_installed
 
 logger = logging.getLogger(__name__)
 if not any(isinstance(filter, DepedencyCheckFilter) for filter in logger.filters):
     # Duplicate filter is added to avoid logging of same error
     # messages incase any of the tools is not installed
     logger.addFilter(DepedencyCheckFilter())
 
-# pylint: disable=too-many-locals
-# pylint: disable=too-many-statements
+# pylint: disable=too-many-locals, too-many-branches
+# pylint: disable=too-many-statements, invalid-name
 def run_experiment(exp):
     """
     Run experiment
 
     Parameters
     -----------
     exp : Experiment
         The experiment attributes
     """
 
-    tools = ["netperf", "ss", "tc", "iperf3", "ping"]
+    tcp_modules_helper(exp)
+    tools = ["netperf", "ss", "tc", "iperf3", "ping", "coap", "server"]
     Runners = namedtuple("runners", tools)
     exp_runners = Runners(
-        netperf=[], ss=[], tc=[], iperf3=[], ping=[]
+        netperf=[], ss=[], tc=[], iperf3=[], ping=[], coap=[], server=[]
     )  # Runner objects
 
-    # Keep track of all destination nodes [to ensure netperf and iperf3
-    # server is run at most once]
-    destination_nodes = {"netperf": set(), "iperf3": set()}
+    # Keep track of all destination nodes [to ensure netperf, iperf3 and
+    # coap server is run at most once]
+    destination_nodes = {"netperf": set(), "iperf3": set(), "coap": set()}
 
     # Contains start time and end time to run respective command
     # from a source netns to destination address (in destination netns)
     ss_schedules = defaultdict(lambda: (float("inf"), float("-inf")))
     ping_schedules = defaultdict(lambda: (float("inf"), float("-inf")))
 
     # Overall experiment stop time considering all flows
     exp_end_t = float("-inf")
 
     dependencies = get_dependency_status(tools)
 
     ss_required = False
     ss_filters = set()
+    server_runner = []
 
     # Traffic generation
     for flow in exp.flows:
+        iperf3_options = {}
         # Get flow attributes
         [
             src_ns,
             dst_ns,
             dst_addr,
             start_t,
             stop_t,
@@ -94,48 +108,94 @@
         ping_schedules[(src_ns, dst_ns, dst_addr)] = (
             min(min_start, start_t),
             max(max_stop, stop_t),
         )
 
         # Setup TCP/UDP flows
         if options["protocol"] == "TCP":
-            # * Ignore netperf tcp control connections
-            # * Destination port of netperf control connection is 12865
-            # * We also have "sport" (source port) in the below condition since
-            #   there can be another flow in the reverse direction whose control
-            #   connection also we must ignore.
-            ss_filters.add("sport != 12865 and dport != 12865")
             ss_required = True
-            (tcp_runners, ss_schedules,) = setup_tcp_flows(
-                dependencies["netperf"],
-                flow,
-                ss_schedules,
-                destination_nodes["netperf"],
-            )
-
-            exp_runners.netperf.extend(tcp_runners)
 
-            # Update destination nodes
-            destination_nodes["netperf"].add(dst_ns)
+            if options["tool"] == "netperf":
+                # * Ignore netperf tcp control connections
+                # * Destination port of netperf control connection is 12865
+                # * We also have "sport" (source port) in the below condition since
+                #   there can be another flow in the reverse direction whose control
+                #   connection also we must ignore.
+                ss_filters.add("sport != 12865 and dport != 12865")
+
+                (tcp_runners, ss_schedules,) = setup_tcp_flows(
+                    dependencies["netperf"],
+                    flow,
+                    ss_schedules,
+                    destination_nodes["netperf"],
+                )
+                exp_runners.netperf.extend(tcp_runners)
+                # Update destination nodes
+                destination_nodes["netperf"].add(dst_ns)
+
+            elif options["tool"] == "iperf3":
+                ss_filters.add("sport != 5201 and dport != 5201")
+                (tcp_runners, ss_schedules,) = setup_tcp_flows(
+                    dependencies["iperf3"],
+                    flow,
+                    ss_schedules,
+                    destination_nodes["iperf3"],
+                )
+                exp_runners.iperf3.extend(tcp_runners)
+                # Update destination nodes
+                destination_nodes["iperf3"].add(dst_ns)
+
+                dst_port_options = {}
+                port_nos = options["port_nos"]
+                for port_no in port_nos:
+                    options["port_no"] = port_no
+                    dst_port_options[port_no] = copy.deepcopy(options)
+
+                if dst_ns in iperf3_options:
+                    dst_port_options.update(iperf3_options.get(dst_ns))
+                iperf3_options.update({dst_ns: dst_port_options})
 
-        elif options["protocol"] == "UDP":
+        elif options["protocol"] == "udp":
             # * Ignore iperf3 tcp control connections
             # * Destination port of iperf3  control connection is 5201
             # * We also have "sport" (source port) in the below condition since
             #   there can be another flow in the reverse direction whose control
             #   connection also we must ignore.
             ss_filters.add("sport != 5201 and dport != 5201")
-            udp_runners = setup_udp_flows(
-                dependencies["iperf3"], flow, destination_nodes["iperf3"]
-            )
+            udp_runners = setup_udp_flows(dependencies["iperf3"], flow)
 
             exp_runners.iperf3.extend(udp_runners)
 
             # Update destination nodes
             destination_nodes["iperf3"].add(dst_ns)
+            dst_port_options = {options["port_no"]: options}
+            if dst_ns in iperf3_options:
+                dst_port_options.update(iperf3_options.get(dst_ns))
+            iperf3_options.update({dst_ns: dst_port_options})
+
+        server_runner.extend(run_server(iperf3_options, exp_end_t, options["protocol"]))
+
+    for coap_application in exp.coap_applications:
+        [
+            src_ns,
+            dst_ns,
+            dst_addr,
+            _,
+            _,
+            _,
+        ] = coap_application._get_props()  # pylint: disable=protected-access
+
+        config.set_value("show_progress_bar", False)
+
+        # Setup runners for emulating CoAP traffic
+        coap_runners = setup_coap_runners(
+            dependencies["coap"], coap_application, destination_nodes["coap"]
+        )
+        exp_runners.coap.extend(coap_runners)
+        destination_nodes["coap"].add(dst_ns)
 
     if ss_required:
         ss_filter = " and ".join(ss_filters)
         ss_runners = setup_ss_runners(dependencies["ss"], ss_schedules, ss_filter)
         exp_runners.ss.extend(ss_runners)
 
     tc_runners = setup_tc_runners(dependencies["tc"], exp.qdisc_stats, exp_end_t)
@@ -146,14 +206,16 @@
 
     try:
         # Start traffic generation
         run_workers(setup_flow_workers(exp_runners, exp_end_t))
 
         logger.info("Parsing statistics...")
 
+        exp_runners.server.extend(server_runner)
+
         # Parse the stored statistics
         run_workers(setup_parser_workers(exp_runners))
 
         logger.info("Parsing statistics complete!")
         logger.info("Output results as JSON dump...")
 
         # Output results as JSON dumps
@@ -180,14 +242,78 @@
             "Experiment %s forcefully stopped. The results obtained maybe incomplete!",
             exp.name,
         )
     finally:
         cleanup()
 
 
+def tcp_modules_helper(exp):
+    """
+    This function is called at the beginning of run_experiment
+    to perform tcp modules related helper tasks
+
+    Parameters
+    -----------
+    exp : Experiment
+        The experiment attributes
+    """
+    if exp.tcp_module_params:
+        if (
+            not (config.get_value("show_tcp_module_parameter_confirmation"))
+            or input(
+                "Are you sure you want to modify TCP module parameters in Linux kernel? (y/n) : "
+            ).lower()
+            == "y"
+        ):
+            for cong_algo, params in exp.tcp_module_params.items():
+                flag = engine.is_module_loaded(cong_algo)
+                if flag:
+                    # the module is already loaded, so store the old parameters
+                    # during experiment set these parameters with new values (reset=False)
+                    # during cleanup reset these parameters with old values (reset=True)
+                    exp.old_cong_algos[cong_algo] = engine.get_current_params(cong_algo)
+                    engine.set_tcp_params(cong_algo, params, False)
+                else:
+                    # the module will be newly loaded
+                    # it should be removed during cleanup
+                    (exp.new_cong_algos).append(cong_algo)
+                    params_string = " ".join(
+                        {f"{key}={value}" for key, value in params.items()}
+                    )
+                    engine.load_tcp_module(cong_algo, params_string)
+
+
+def run_server(iperf3options, exp_end_t, protocol):
+    """
+    Run and wait for all server to start
+
+    Parameters
+    ----------
+    iperf3options: dict
+        start server with iperf3 server options
+    exp_end_t: int
+        experiment completion time
+    protocol: str
+        transport layer protocol, either "tcp" or "udp"
+    """
+    # Start server
+    server_list = []
+    for dst_ns in iperf3options:
+        for dst_port in iperf3options[dst_ns]:
+            runner_obj = Iperf3ServerRunner(dst_ns, exp_end_t, protocol)
+            runner_obj.setup_iperf3_server(iperf3options[dst_ns][dst_port])
+            server_list.append(runner_obj)
+
+    for server in server_list:
+        process = Process(target=server.run)
+        process.start()
+
+    return server_list
+
+
 def run_workers(workers):
     """
     Run and wait for processes to finish
 
     Parameters
     ----------
     workers: list[multiprocessing.Process]
@@ -227,14 +353,16 @@
     Outputs experiment results as json dumps
     """
     SsResults.output_to_file()
     NetperfResults.output_to_file()
     Iperf3Results.output_to_file()
     TcResults.output_to_file()
     PingResults.output_to_file()
+    CoAPResults.output_to_file()
+    Iperf3ServerResults.output_to_file()
 
 
 def setup_flow_workers(exp_runners, exp_stop_time):
     """
     Setup flow generation and stats collection processes(netperf, ss, tc, iperf3...).
 
     Also add a progress bar process for showing experiment progress.
@@ -291,14 +419,20 @@
 
     for tc_runner in exp_runners.tc:
         parsers.append(Process(target=tc_runner.parse))
 
     for ping_runner in exp_runners.ping:
         parsers.append(Process(target=ping_runner.parse))
 
+    for coap_runner in exp_runners.coap:
+        parsers.append(Process(target=coap_runner.parse))
+
+    for server_runner in exp_runners.server:
+        parsers.append(Process(target=server_runner.parse))
+
     return parsers
 
 
 def get_dependency_status(tools):
     """
     Checks for dependency
 
@@ -310,92 +444,133 @@
     Returns
     -------
     dict
         contains information as to whether `tools` are installed
     """
     dependencies = {}
     for dependency in tools:
+        # Check for the availability of aiocoap for CoAP emulation
+        if dependency == "coap":
+            dependencies[dependency] = is_package_installed("aiocoap")
+            continue
         dependencies[dependency] = is_dependency_installed(dependency)
     return dependencies
 
 
 def setup_tcp_flows(dependency, flow, ss_schedules, destination_nodes):
     """
-    Setup netperf to run tcp flows
+    Setup netperf/iperf3 to run tcp flows
     Parameters
     ----------
     dependency: int
-        whether netperf is installed
+        whether netperf/iperf3 is installed
     flow: Flow
         Flow parameters
     ss_schedules:
         ss_schedules so far
     destination_nodes:
-        Destination nodes so far already running netperf server
+        Destination nodes so far already running netperf/iperf3 server
 
     Returns
     -------
     dependency: int
-        updated dependency in case netperf is not installed
-    netperf_runners: List[NetperfRunner]
-        all the netperf flows generated
+        updated dependency in case netperf/iperf3 is not installed
+    tcp_runners: List[NetperfRunner] / List[Iperf3Runner]
+        all the netperf/iperf3 flows generated
     workers: List[multiprocessing.Process]
-        Processes to run netperf flows
+        Processes to run netperf/iperf3 flows
     ss_schedules: dict
         updated ss_schedules
     """
-    netperf_runners = []
+    tcp_runners = []
     if not dependency:
-        logger.warning("Netperf not found. Tcp flows cannot be generated")
+        logger.warning("Dependency not found. Tcp flows cannot be generated")
     else:
         # Get flow attributes
         [
             src_ns,
             dst_ns,
             dst_addr,
             start_t,
             stop_t,
             n_flows,
             options,
         ] = flow._get_props()  # pylint: disable=protected-access
 
-        # Run netserver if not already run before on given dst_node
-        if dst_ns not in destination_nodes:
-            NetperfRunner.run_netserver(dst_ns)
+        if options["tool"] == "netperf":
+            # Run netserver if not already run before on given dst_node
+            if dst_ns not in destination_nodes:
+                NetperfRunner.run_netserver(dst_ns)
+
+            src_name = TopologyMap.get_node(src_ns).name
+
+            netperf_options = {}
+            netperf_options["testname"] = "TCP_STREAM"
+            netperf_options["cong_algo"] = options["cong_algo"]
+            f_flow = "flow" if n_flows == 1 else "flows"
+            logger.info(
+                "Running %s netperf %s from %s to %s...",
+                n_flows,
+                f_flow,
+                src_name,
+                dst_addr,
+            )
 
-        src_name = TopologyMap.get_namespace(src_ns)["name"]
+            # Create new processes to be run simultaneously
+            for _ in range(n_flows):
+                runner_obj = NetperfRunner(
+                    src_ns,
+                    dst_addr,
+                    start_t,
+                    stop_t - start_t,
+                    dst_ns,
+                    **netperf_options,
+                )
+                tcp_runners.append(runner_obj)
+
+        elif options["tool"] == "iperf3":
+            src_name = TopologyMap.get_node(src_ns).name
+            f_flow = "flow" if n_flows == 1 else "flows"
+            iperf3_options = {}
+            iperf3_options["cong_algo"] = options["cong_algo"]
+            logger.info(
+                "Running %s tcp iperf3 %s from %s to %s...",
+                n_flows,
+                f_flow,
+                src_name,
+                dst_addr,
+            )
 
-        netperf_options = {}
-        netperf_options["testname"] = "TCP_STREAM"
-        netperf_options["cong_algo"] = options["cong_algo"]
-        f_flow = "flow" if n_flows == 1 else "flows"
-        logger.info(
-            "Running %s netperf %s from %s to %s...",
-            n_flows,
-            f_flow,
-            src_name,
-            dst_addr,
-        )
+            port_nos = options["port_nos"]
 
-        # Create new processes to be run simultaneously
-        for _ in range(n_flows):
-            runner_obj = NetperfRunner(
-                src_ns, dst_addr, start_t, stop_t - start_t, dst_ns, **netperf_options
-            )
-            netperf_runners.append(runner_obj)
+            # Create new processes to be run simultaneously
+            for i in range(n_flows):
+                runner_obj = Iperf3Runner(
+                    src_ns,
+                    dst_addr,
+                    options["target_bw"],
+                    1,
+                    start_t,
+                    stop_t - start_t,
+                    dst_ns,
+                    "tcp",
+                    **iperf3_options,
+                )
+                options["port_no"] = port_nos[i]
+                runner_obj.setup_iperf3_client(options)
+                tcp_runners.append(runner_obj)
 
         # Find the start time and stop time to run ss command in `src_ns` to a `dst_addr`
         ss_schedules = _get_start_stop_time_for_ss(
             src_ns, dst_ns, dst_addr, start_t, stop_t, ss_schedules
         )
+    return tcp_runners, ss_schedules
 
-    return netperf_runners, ss_schedules
 
-
-def setup_udp_flows(dependency, flow, destination_nodes):
+def setup_udp_flows(dependency, flow):
     """
     Setup iperf3 to run udp flows
 
     Parameters
     ----------
     dependency: int
         whether iperf3 is installed
@@ -424,33 +599,31 @@
             dst_addr,
             start_t,
             stop_t,
             n_flows,
             options,
         ] = flow._get_props()  # pylint: disable=protected-access
 
-        # Run iperf3 server if not already run before on given dst_node
-        if dst_ns not in destination_nodes:
-            Iperf3Runner.run_server(dst_ns)
-
-        src_name = TopologyMap.get_namespace(src_ns)["name"]
+        src_name = TopologyMap.get_node(src_ns).name
         f_flow = "flow" if n_flows == 1 else "flows"
         logger.info(
             "Running %s udp %s from %s to %s...", n_flows, f_flow, src_name, dst_addr
         )
 
         runner_obj = Iperf3Runner(
             src_ns,
             dst_addr,
             options["target_bw"],
             n_flows,
             start_t,
             stop_t - start_t,
             dst_ns,
+            "udp",
         )
+        runner_obj.setup_iperf3_client(options)
         iperf3_runners.append(runner_obj)
 
     return iperf3_runners
 
 
 def setup_ss_runners(dependency, ss_schedules, ss_filter):
     """
@@ -549,14 +722,78 @@
             )
             runners.append(ping_runner)
     else:
         logger.warning("ping not found.")
     return runners
 
 
+def setup_coap_runners(dependency, application, destination_nodes):
+    """
+    Setup CoAPRunner objects for generating CoAP traffic
+
+    Parameters
+    ----------
+    dependency : int
+        Whether aiocoap is installed
+    application : CoapApplication
+        The CoapApplication object
+    destination_nodes:
+        Destination nodes so far already running CoAP server
+
+    Returns
+    -------
+    runners : List[CoAPRunner]
+        List of CoAPRunner objects for the current flow object
+    """
+    runners = []
+
+    # If aiocoap is installed
+    if dependency:
+        # Get flow attributes
+        [
+            src_ns,
+            dst_ns,
+            dst_addr,
+            n_con_msgs,
+            n_non_msgs,
+            user_options,
+        ] = application._get_props()  # pylint: disable=protected-access
+
+        # Run CoAP server if not already run before on given dst_node
+        if dst_ns not in destination_nodes:
+
+            # If user has not supplied the user options
+            if user_options is not None:
+                # Creating the options string for running the CoAP server
+                if (
+                    "coap_server_content" in user_options.keys()
+                    and user_options["coap_server_content"] != ""
+                ):
+                    server_content = '"' + user_options["coap_server_content"] + '"'
+                    server_options = f"-c {server_content}"
+                else:
+                    server_options = None
+            else:
+                server_options = None
+
+            # Running the server
+            CoAPRunner.run_server(dst_ns, server_options)
+
+        # Create the CoAPRunner object
+        coap_runner = CoAPRunner(src_ns, dst_addr, user_options, n_con_msgs, n_non_msgs)
+        runners.append(coap_runner)
+
+    # If aiocoap is not installed
+    else:
+        logger.warning("aiocoap not found for CoAP emulation.")
+
+    # Return the list of runners
+    return runners
+
+
 def progress_bar(stop_time, precision=1):
     """
     Show a progress bar from from 0 `units` to `stop_time`
 
     The time unit is decided by `precision` in seconds. It is
     1s by default.
 
@@ -585,15 +822,20 @@
     Clean up
     """
     # Remove results of the experiment
     SsResults.remove_all_results()
     NetperfResults.remove_all_results()
     TcResults.remove_all_results()
     PingResults.remove_all_results()
+    CoAPResults.remove_all_results()
+    Iperf3Results.remove_all_results()
+    Iperf3ServerResults.remove_all_results()
 
+    # Clean up the configured TCP modules and kill processes
+    tcp_modules_clean_up()
     kill_processes()
 
 
 # Helper methods
 # pylint: disable=too-many-arguments
 def _get_start_stop_time_for_ss(
     src_ns, dst_ns, dst_addr, start_t, stop_t, ss_schedules
```

### Comparing `nest-0.4.1/nest/input_validator/__init__.py` & `nest-0.4.2/nest/input_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/input_validator/input_validator.py` & `nest-0.4.2/nest/input_validator/input_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,15 @@
                     arg_name,
                     func.__qualname__,
                 )
             casted_args.append(casted_arg_value)
 
         # Default values are not checked here, it is assumed that correct
         # values are passed for default parameters
-        for kwarg_name in kwargs:
-            kwarg_value = kwargs[kwarg_name]
+        for kwarg_name, kwarg_value in kwargs.items():
             casted_kwarg_value = kwarg_value
             if kwarg_name in annotations:
                 casted_kwarg_value = validate_input_and_cast(
                     func.__qualname__, kwarg_name, kwarg_value, annotations[kwarg_name]
                 )
             else:
                 logger.debug(
```

### Comparing `nest-0.4.1/nest/input_validator/typing_helper_methods.py` & `nest-0.4.2/nest/input_validator/typing_helper_methods.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/logging_helper.py` & `nest-0.4.2/nest/logging_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     5
 
     """
     if not method_name:
         method_name = level_name.lower()
 
     if hasattr(logging, level_name):
-        raise AttributeError("{} already defined in logging module".format(level_name))
+        raise AttributeError(f"{level_name} already defined in logging module")
     if hasattr(logging, method_name):
-        raise AttributeError("{} already defined in logging module".format(method_name))
+        raise AttributeError(f"{method_name} already defined in logging module")
     if hasattr(logging.getLoggerClass(), method_name):
-        raise AttributeError("{} already defined in logger class".format(method_name))
+        raise AttributeError(f"{method_name} already defined in logger class")
 
     def log_for_level(self, message, *args, **kwargs):
         if self.isEnabledFor(level_num):
             # pylint: disable=protected-access
             self._log(level_num, message, args, **kwargs)
 
     def log_to_root(message, *args, **kwargs):
@@ -76,15 +76,15 @@
 
     Parameters
     ----------
     level: str
         log level from config
     """
     nest_logger = logging.getLogger(
-        __name__.split(".")[0]
+        __name__.split(".", maxsplit=1)[0]
     )  # get the root's child logger
     nest_logger.setLevel(level)  # Update logger level
     # Update handler level
     nest_handler = nest_logger.handlers[0]
     nest_handler.setLevel(level)
     # pylint: disable=no-member
     if level == "TRACE" and not any(
```

### Comparing `nest-0.4.1/nest/network_utilities.py` & `nest-0.4.2/nest/network_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: GPL-2.0-only
-# Copyright (c) 2019-2020 NITK Surathkal
+# Copyright (c) 2019-2022 NITK Surathkal
 
 """Necessary checks before running utilities on experiment"""
 
 import functools
 from time import sleep
-import nest.config as config
+from nest import config
 import nest.global_variables as g_var
 from nest.topology_map import TopologyMap
 from nest.engine.ipv6_states import check_ipv6_states
 
 
 def ipv6_dad_check(func):
     """
@@ -36,15 +36,18 @@
 
         if (
             g_var.IS_IPV6 is True
             and config.get_value("disable_dad") is not True
             and g_var.IS_DAD_CHECKED is not True
         ):
 
-            namespaces = TopologyMap.get_namespaces()
+            nodes = TopologyMap.get_nodes()
+            namespaces = list(
+                map(lambda ns_id: {"id": ns_id, "name": nodes[ns_id].name}, nodes)
+            )
 
             # Verifies if IPv6 states are addressable or not
             while True:
                 status = check_ipv6_states(namespaces)
 
                 # IPv6 state will be both in tentative and dadfailed together
                 if status["dadfailed"][0] is True:
```

### Comparing `nest-0.4.1/nest/routing/isis.py` & `nest-0.4.2/nest/routing/isis.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,42 +10,45 @@
 
 
 class Isis(RoutingDaemonBase):
     """
     Handles IS-IS related functionalities.
     """
 
-    def __init__(self, router_ns_id, interfaces, conf_dir, **kwargs):
-        super().__init__(router_ns_id, interfaces, "isisd", conf_dir, **kwargs)
+    def __init__(self, router_ns_id, ipv6_routing, interfaces, conf_dir, **kwargs):
+        super().__init__(
+            router_ns_id, ipv6_routing, interfaces, "isisd", conf_dir, **kwargs
+        )
 
     def create_basic_config(self):
         """
         Creates a file with basic configuration for IS-IS.
         Use base `add_to_config` directly for more complex configurations
         """
 
         area_id = "00.0000.0000.0000.0000.0000.0000"
         system_id_hash = str(
             int(
                 hashlib.sha256(
                     self.interfaces[0]
-                    .address.get_addr(with_subnet=False)
+                    .get_address(not self.ipv6_routing, self.ipv6_routing, True)[0]
+                    .get_addr(with_subnet=False)
                     .encode("utf-8")
                 ).hexdigest(),
                 16,
             )
         )[:12]
-        system_id = ".".join(map("".join, zip(*[iter(system_id_hash)] * 4)))
 
+        system_id = ".".join(map("".join, zip(*[iter(system_id_hash)] * 4)))
         self.add_to_config(f"router isis {self.router_ns_id}")
         self.add_to_config("is-type level-1")
         self.add_to_config(f"net {area_id}.{system_id}.00")
         for interface in self.interfaces:
             self.add_to_config(f"interface {interface.id}")
-            if self.ipv6:
+            if self.ipv6_routing:
                 self.add_to_config(f" ipv6 router isis {self.router_ns_id}")
             else:
                 self.add_to_config(f" ip router isis {self.router_ns_id}")
 
         if self.log_file is not None:
             self.add_to_config(f"log file {self.log_file}")
```

### Comparing `nest-0.4.1/nest/routing/ldp.py` & `nest-0.4.2/nest/routing/ldp.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,45 @@
 
 
 class Ldp(RoutingDaemonBase):
     """
     Handles Ldp related functionalities for frr.
     """
 
-    def __init__(self, router_ns_id, interfaces, conf_dir, **kwargs):
-        super().__init__(router_ns_id, interfaces, "ldpd", conf_dir, **kwargs)
+    def __init__(self, router_ns_id, ipv6_routing, interfaces, conf_dir, **kwargs):
+        super().__init__(
+            router_ns_id, ipv6_routing, interfaces, "ldpd", conf_dir, **kwargs
+        )
 
     def create_basic_config(self):
         """
         Creates a file with basic configuration for ldp.
         Use base `add_to_config` directly for more complex configurations
         """
         self.add_to_config("mpls ldp")
+        router_ip = self.interfaces[0].get_address(
+            not self.ipv6_routing, self.ipv6_routing, True
+        )[0]
+        self.add_to_config(f" router-id {router_ip.get_addr(with_subnet=False)}")
+        if not self.ipv6_routing:
+            self.add_to_config(" address-family ipv4")
+        else:
+            self.add_to_config(" address-family ipv6")
         self.add_to_config(
-            f" router-id {self.interfaces[0].address.get_addr(with_subnet=False)}"
-        )
-        self.add_to_config(" address-family ipv4")
-        self.add_to_config(
-            f"discovery transport-address {self.interfaces[0].address.get_addr(with_subnet=False)}"
+            f"discovery transport-address {router_ip.get_addr(with_subnet=False)}"
         )
 
         for interface in self.interfaces:
-            self.add_to_config(f"  interface {interface.id}")
+            if self.ipv6_routing and len(interface.get_address(False, True, True)) > 0:
+                self.add_to_config(f"  interface {interface.id}")
+            elif (
+                not self.ipv6_routing
+                and len(interface.get_address(True, False, True)) > 0
+            ):
+                self.add_to_config(f"  interface {interface.id}")
 
         if self.log_file is not None:
             self.add_to_config(f"log file {self.log_file}")
 
         self.create_config()
 
     def run(self):
```

### Comparing `nest-0.4.1/nest/routing/rip.py` & `nest-0.4.2/nest/routing/zebra.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
-"""Class to handles RIP related functionalities"""
+"""Class to handle zebra"""
 
 from functools import partial
-from nest.engine.dynamic_routing import run_ripd
+from nest.exception import RequiredDependencyNotFound
 from nest.routing.route_daemons import RoutingDaemonBase
+from nest.engine.dynamic_routing import run_zebra
 
 
-class Rip(RoutingDaemonBase):
+class Zebra(RoutingDaemonBase):
     """
-    Handles RIP related functionalities.
+    Handles zebra related functionalities.
     Refer to `DaemonBase` for usage
     """
 
-    def __init__(self, router_ns_id, interfaces, conf_dir, **kwargs):
-        super().__init__(router_ns_id, interfaces, "ripd", conf_dir, **kwargs)
+    def __init__(self, router_ns_id, ipv6_routing, interfaces, conf_dir, **kwargs):
+        super().__init__(
+            router_ns_id, ipv6_routing, interfaces, "zebra", conf_dir, **kwargs
+        )
 
-    def add_rip(self):
+    def add_interface(self, interface):
         """
-        Add command to enable RIP on router to config file
+        Add interface command to config file
         """
-        if self.ipv6:
-            self.add_to_config("router ripng")
-        else:
-            self.add_to_config("router rip")
+        self.add_to_config(f"interface {interface}")
 
-    def add_network(self, network):
+    def add_ip_address(self, ip_address):
         """
-        Add command for subnet or interface to run RIP on to config file
-
-        Parameters
-        ----------
-        network : str
-            subnet or interface to run RIP on
+        Add IP address command to config file
         """
-        self.add_to_config(f" network {network}")
+        if self.ipv6_routing:
+            self.add_to_config(f" ipv6 address {ip_address}")
+        else:
+            self.add_to_config(f" ip address {ip_address}")
 
     def create_basic_config(self):
         """
-        Creates a file with basic configuration for RIP.
+        Creates a file with basic configuration for OSPF.
         Use base `add_to_config` directly for more complex configurations
         """
-        self.add_rip()
+
+        # Add loopback interface
+        self.add_interface("lo")
+        self.add_to_config(" no shutdown")
         for interface in self.interfaces:
-            self.add_network(interface.id)
+            self.add_interface(interface.id)
+            for addr in interface.get_address(
+                not self.ipv6_routing, self.ipv6_routing, True
+            ):
+                self.add_ip_address(addr.get_addr())
+
         if self.log_file is not None:
             self.add_to_config(f"log file {self.log_file}")
 
     def run(self):
         """
-        Runs the ripd command
+        Runs the zebra daemon
         """
         super().run(
             engine_func=partial(
-                run_ripd, self.router_ns_id, self.conf_file, self.pid_file, self.ipv6
+                run_zebra, self.router_ns_id, self.conf_file, self.pid_file
             )
         )
+
+    def handle_dependecy_error(self):
+        self.logger.error(
+            "Zebra not found. Routes from routing protocols cannot be added."
+        )
+        raise RequiredDependencyNotFound()
```

### Comparing `nest-0.4.1/nest/routing/route_daemons.py` & `nest-0.4.2/nest/routing/route_daemons.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """
 Base class for Routing daemons.
 """
-
+import os
 from abc import ABC, abstractmethod
 import io
 import logging
+import pwd
 import shutil
 from nest.engine.dynamic_routing import supports_dynamic_routing
 from nest import config
 from nest.logging_helper import DepedencyCheckFilter, DuplicateRoutingLogsFilter
 
 # pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
 
 
 class RoutingDaemonBase(ABC):
     """
     Abstract class for Dynamic routing related processes.
     This class should be inherited for adding other daemons
 
@@ -41,17 +43,22 @@
         daemon to run(one of ['zebra', 'ospf', 'isis'])
     conf_file : str
         config file path
     pid_file : str
         pid file path for the daemon process
     interfaces : List[Interface]
         interfaces present in the router
+    ipv6_routing: bool
+        True for routing IPv6 interfaces, False otherwise.
+        Default value is set to False.
     """
 
-    def __init__(self, router_ns_id, interfaces, daemon, conf_dir, **kwargs):
+    def __init__(
+        self, router_ns_id, ipv6_routing, interfaces, daemon, conf_dir, **kwargs
+    ):
         """
         Parameters
         ----------
         conf_dir : str
             Directory to store config files
         **kwargs
             Key worded arguments for other daemon specific parameters
@@ -76,24 +83,27 @@
         if not supports_dynamic_routing(daemon):
             self.handle_dependecy_error()
 
         self.conf = io.StringIO()
         self.router_ns_id = router_ns_id
         self.conf_file = f"{conf_dir}/{self.router_ns_id}_{daemon}.conf"
         self.pid_file = f"{conf_dir}/{self.router_ns_id}_{daemon}.pid"
+        self.socket_file = None
+        if config.get_value("routing_suite") == "bird":
+            self.socket_file = f"{conf_dir}/{self.router_ns_id}_{daemon}.ctl"
         self.log_file = None
         if kwargs["log_dir"] is not None:
             self.logger.info(
                 "%s logging enabled. Log files can found in %s directory",
                 config.get_value("routing_suite"),
                 kwargs["log_dir"],
             )
             self.log_file = f"{kwargs['log_dir']}/{self.router_ns_id}_{daemon}.log"
         self.interfaces = interfaces
-        self.ipv6 = interfaces[0].address.is_ipv6()
+        self.ipv6_routing = ipv6_routing
 
     @abstractmethod
     def create_basic_config(self):
         """
         Created minimum configuration for `daemon`
         """
 
@@ -117,15 +127,18 @@
         self.conf.write(f"{command}\n")
 
     def create_config(self):
         """
         Creates config file on disk from `self.conf`
         """
         with open(self.conf_file, "w") as conf:
-            shutil.chown(self.conf_file, user=config.get_value("routing_suite"))
+            if config.get_value("routing_suite") == "bird":
+                shutil.chown(self.conf_file, user=pwd.getpwuid(os.getuid())[0])
+            else:
+                shutil.chown(self.conf_file, user=config.get_value("routing_suite"))
             self.conf.seek(0)
             shutil.copyfileobj(self.conf, conf)
 
     def handle_dependecy_error(self):
         """
         Default error when routing daemon is not present
         """
```

### Comparing `nest-0.4.1/nest/routing/routing_helper.py` & `nest-0.4.2/nest/routing/routing_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """
 Helper class for routing
 """
-
+import os
+import pwd
 import time
 import logging
 import importlib
 from os import mkdir, kill, path, listdir
 import atexit
 from shutil import rmtree, chown
 from signal import SIGTERM
 from typing import List
-from nest.exceptions import RequiredDependencyNotFound
+from nest.exception import RequiredDependencyNotFound
 from nest.input_validator.input_validator import input_validator
 from nest.topology.id_generator import IdGen
+from nest.routing.static_routing import StaticRouting
 from nest.routing.zebra import Zebra
 from nest.routing.ldp import Ldp
 from nest.topology_map import TopologyMap
 from nest.user import User
 from nest import config
 from nest.topology import Node
 
 logger = logging.getLogger(__name__)
 
 # pylint:disable=too-few-public-methods
 # pylint:disable=too-many-instance-attributes
+# pylint:disable=too-many-arguments
 
 
 class RoutingHelper:
     """
     Handles basic routing requirements for the topology.
     Either inherit this class or use `Zebra` and other protocols
     for better customizations
@@ -45,65 +48,71 @@
         routers in the topology
     hosts : List[Node]
         hosts in the topology
     conf_dir : str
         path for config directory of daemons
     protocol_class : ABCMeta
         Protocol class which will later be instantiated
+    ipv6_routing: bool
+        True for routing IPv6 interfaces, False otherwise.
+        Default value is set to False.
     """
 
     _module_map = {
         "ospf": ["nest.routing.ospf", "Ospf"],
         "rip": ["nest.routing.rip", "Rip"],
         "isis": ["nest.routing.isis", "Isis"],
+        "static": ["nest.routing.static_routing", "StaticRouting"],
     }
 
     @input_validator
     def __init__(
         self,
         protocol: str,
+        ipv6_routing: bool = False,
         hosts: List[Node] = None,
         routers: List[Node] = None,
         ldp_routers: List[Node] = None,
     ):
         """
         Constructor for RoutingHelper.
         The dynamic routing daemons will be run only on nodes with more than
         one interface. Specify `hosts` & `routers` parameters to override this.
 
         Parameters
         ----------
         protocol: str
             routing protocol to be run. One of [ospf, rip, isis]
+        ipv6_routing: bool
+            True for routing IPv6 interfaces, False otherwise.
+            Default value is set to False.
         hosts: List[Node]
             List of hosts in the network. If `None`, considers the entire topology.
             Use this if your topology has disjoint networks
         routers: List[Node]
             List of routers in the network. If `None`, considers the entire topology.
             Use this if your topology has disjoint networks
         ldp_routers: List[Node]
             List of Routers which are to be used with mpls.
             Only enables ldp discovery on interfaces with mpls enabled
         """
-        if protocol == "static":
-            raise NotImplementedError(
-                "Static routing is yet to be implemented. Use rip, ospf or isis"
-            )
-        if protocol not in ["rip", "ospf", "isis"]:
+
+        if protocol not in ["rip", "ospf", "isis", "static"]:
             raise ValueError(
-                f"Supported routing protocols are rip, ospf and isis, "
+                f"Supported routing protocols are rip, ospf, isis and static, "
                 f"but got protocol {protocol}"
             )
         self.protocol = protocol
 
         # Validate hosts, routers and ldp_routers
         self._is_node_list("hosts", hosts)
         self._is_node_list("routers", routers)
         self._is_node_list("ldp_routers", ldp_routers)
 
+        self.ipv6_routing = ipv6_routing
         self.hosts = []
         self.routers = []
         if routers is None and hosts is None:
             all_nodes = TopologyMap.get_hosts() + TopologyMap.get_routers()
             for node in all_nodes:
                 num_interfaces = len(node.interfaces)
                 if num_interfaces == 1:
@@ -113,14 +122,15 @@
         else:
             self.hosts = hosts
             self.routers = routers
 
         self.ldp_routers = ldp_routers if ldp_routers is not None else []
         self.conf_dir = None
         self.log_dir = None
+        self.socket_dir = None
         module_str, class_str = RoutingHelper._module_map[self.protocol]
         module = importlib.import_module(module_str)
         self.protocol_class = getattr(module, class_str)
         self.zebra_list = []
         self.protocol_list = []
         self.ldp_list = []
 
@@ -129,32 +139,55 @@
     def populate_routing_tables(self):
         """
         Populate routing table using `self.protocol`
         """
         self._setup_default_routes()
 
         if self.protocol == "static":
-            pass  # TODO: add static routing
+            static_routing = StaticRouting()
+            static_routing.run_static_routing()
+        elif config.get_value("routing_suite") == "bird":
+            try:
+                self._run_dyn_routing_bird()
+            except RequiredDependencyNotFound:
+                return
         else:
             try:
+                # Warning for using ISIS daemons along with other daemons
+                # since they interfere with other routing daemons (which may
+                # or may not be of ISIS)
+                if (
+                    self.protocol == "isis"
+                    and config.get_value("routing_suite") == "quagga"
+                ):
+                    logger.warning(
+                        "ISIS routing protocol in quagga might overwrite "
+                        "previously assigned routes by other RoutingHelpers"
+                    )
                 self._run_dyn_routing()
             except RequiredDependencyNotFound:
                 return
 
     def _create_directory(self, dir_path):
         """
         Creates a quagga/frr owned directory at `dir_path`
 
         Parmeters
         ---------
         dir_path: path of the directory to be created
 
         """
-        mkdir(dir_path)
-        chown(dir_path, user=config.get_value("routing_suite"))
+        if path.exists(dir_path):
+            logger.warning("{dir_path} already exists")
+        else:
+            mkdir(dir_path)
+            if config.get_value("routing_suite") == "bird":
+                chown(dir_path, user=pwd.getpwuid(os.getuid())[0])
+            else:
+                chown(dir_path, user=config.get_value("routing_suite"))
 
     def _create_conf_directory(self):
         """
         Creates a directory for holding routing related config
         and pid files.
         Override this to create directory at a location other than /tmp
 
@@ -182,22 +215,56 @@
         self._create_directory(log_path)
         return log_path
 
     def _setup_default_routes(self):
         """
         Setup default routes in hosts
         """
-        for host in self.hosts:
-            host.add_route("DEFAULT", host.interfaces[0])
+        if config.get_value("routing_suite") == "bird":
+            for host in self.hosts:
+                host.add_route("DEFAULT", host.interfaces[0])
+            router_interfaces = set()
+            for router in self.routers:
+                for interface in router.interfaces:
+                    router_interfaces.add(interface)
+            for router in self.routers:
+                for interface in router.interfaces:
+                    if interface.pair not in router_interfaces:
+                        router.add_route(interface.pair.get_address(), interface)
+        else:
+            for host in self.hosts:
+                host.add_route(
+                    "DEFAULT",
+                    host.interfaces[0],
+                    host.interfaces[0].pair.get_address(
+                        not self.ipv6_routing, self.ipv6_routing, True
+                    )[0],
+                )
+
+    def _run_dyn_routing_bird(self):
+        """
+        to create config dir and run bird
+        """
+        logger.info("Running bird on routers")
+        self.socket_dir = ""
+        self.conf_dir = self._create_conf_directory()
+        if config.get_value("routing_logs"):
+            self.log_dir = self._create_log_directory()
+        for router in self.routers:
+            self._run_routing_protocol(router)
+        self._check_for_convergence()
 
     def _run_dyn_routing(self):
         """
         Run zebra and `self.protocol`
         """
-        logger.info("Running zebra and %s on routers", self.protocol)
+        if self.ipv6_routing:
+            logger.info("Running zebra and %s on routers (IPv6)", self.protocol)
+        else:
+            logger.info("Running zebra and %s on routers", self.protocol)
         self.conf_dir = self._create_conf_directory()
         if config.get_value("routing_logs"):
             self.log_dir = self._create_log_directory()
 
         for router in self.routers:
             self._run_zebra(router)
             self._run_routing_protocol(router)
@@ -205,41 +272,67 @@
                 self._run_ldp(router)
         self._check_for_convergence()
 
     def _run_zebra(self, router):
         """
         Create required config file and run zebra
         """
-        zebra = Zebra(router.id, router.interfaces, self.conf_dir, log_dir=self.log_dir)
+        zebra = Zebra(
+            router.id,
+            self.ipv6_routing,
+            router.interfaces,
+            self.conf_dir,
+            log_dir=self.log_dir,
+        )
         zebra.create_basic_config()
         zebra.run()
         self.zebra_list.append(zebra)
 
     def _run_routing_protocol(self, router):
         """
         Create required config file and run `self.protocol`
         """
-        protocol = self.protocol_class(
-            router.id, router.interfaces, self.conf_dir, log_dir=self.log_dir
-        )
+        if config.get_value("routing_suite") == "bird":
+            protocol = self.protocol_class(
+                router.id,
+                self.ipv6_routing,
+                router.interfaces,
+                self.conf_dir,
+                log_dir=self.log_dir,
+                socket_dir=self.socket_dir,
+            )
+        else:
+            protocol = self.protocol_class(
+                router.id,
+                self.ipv6_routing,
+                router.interfaces,
+                self.conf_dir,
+                log_dir=self.log_dir,
+            )
         protocol.create_basic_config()
         protocol.run()
         self.protocol_list.append(protocol)
 
     def _run_ldp(self, router):
         """
         Create required config file and run ldp
         """
         mpls_interfaces = []
         for interface in router.interfaces:
             if interface.is_mpls_enabled():
                 mpls_interfaces.append(interface)
         if len(mpls_interfaces) == 0:
             raise Exception("MPLS isn't enabled in any interface!")
-        ldp = Ldp(router.id, mpls_interfaces, self.conf_dir, log_dir=self.log_dir)
+        ldp = Ldp(
+            router.id,
+            self.ipv6_routing,
+            mpls_interfaces,
+            self.conf_dir,
+            log_dir=self.log_dir,
+        )
         ldp.create_basic_config()
         ldp.run()
         self.ldp_list.append(ldp)
 
     def _check_for_convergence(self):
         """
         Wait for the routing protocol to converge.
@@ -250,18 +343,23 @@
         converged = False
         # Ping between hosts until convergence
         while not converged:
             time.sleep(interval)
             converged = True
             for i in range(len(self.hosts)):
                 for j in range(i + 1, len(self.hosts)):
-                    if not self.hosts[i].ping(
-                        self.hosts[j].interfaces[0].address.get_addr(), verbose=False
+                    for k_addr in (
+                        self.hosts[j]
+                        .interfaces[0]
+                        .get_address(not self.ipv6_routing, self.ipv6_routing, True)
                     ):
-                        converged = False
+                        if not self.hosts[i].ping(k_addr.get_addr(), verbose=0):
+                            converged = False
+                            break
+                    if not converged:
                         break
                 if not converged:
                     break
 
         logger.info("Routing completed")
 
     def _is_node_list(self, arg_name, node_list):
@@ -311,15 +409,15 @@
                     pid = int(pid_file.read())
                     try:
                         kill(pid, SIGTERM)
                     except ProcessLookupError:
                         pass
 
         # Delete config directory
-        if path.isdir(self.conf_dir):
+        if self.conf_dir is not None and path.isdir(self.conf_dir):
             rmtree(self.conf_dir)
 
         # Change ownership of log files to current user
         if self.log_dir is not None and path.isdir(self.log_dir):
             chown(self.log_dir, user=User.user_id, group=User.group_id)
             for file in listdir(self.log_dir):
                 chown(
```

### Comparing `nest-0.4.1/nest/routing/zebra.py` & `nest-0.4.2/nest/tests/test_static_routing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,95 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
-"""Class to handle zebra"""
+"""Test APIs from static routing"""
 
-from functools import partial
-from nest.exceptions import RequiredDependencyNotFound
-from nest.routing.route_daemons import RoutingDaemonBase
-from nest.engine.dynamic_routing import run_zebra
+import unittest
+from nest.topology import Node, connect
+from nest.clean_up import delete_namespaces
+from nest.topology_map import TopologyMap
+from nest.routing.routing_helper import RoutingHelper
 
+# pylint: disable=missing-docstring
 
-class Zebra(RoutingDaemonBase):
-    """
-    Handles zebra related functionalities.
-    Refer to `DaemonBase` for usage
-    """
 
-    def __init__(self, router_ns_id, interfaces, conf_dir, **kwargs):
-        super().__init__(router_ns_id, interfaces, "zebra", conf_dir, **kwargs)
-
-    def add_interface(self, interface):
-        """
-        Add interface command to config file
+class TestStaticRouting(unittest.TestCase):
+    # pylint: disable=invalid-name
+    def setUp(self):
+        # create nodes
+        # pylint: disable=anomalous-backslash-in-string
         """
-        self.add_to_config(f"interface {interface}")
+        Topology is as follows:
 
-    def add_ip_address(self, ip_address):
-        """
-        Add IP address command to config file
+        n0            n2
+          \          /
+           \        /
+            r0----r1
+           /        \
+          /          \
+        n1            n3
         """
-        if self.ipv6:
-            self.add_to_config(f" ipv6 address {ip_address}")
-        else:
-            self.add_to_config(f" ip address {ip_address}")
 
-    def create_basic_config(self):
-        """
-        Creates a file with basic configuration for OSPF.
-        Use base `add_to_config` directly for more complex configurations
-        """
+        self.n0 = Node("n0")
+        self.n1 = Node("n1")
+        self.n2 = Node("n2")
+        self.n3 = Node("n3")
 
-        # Add loopback interface
-        self.add_interface("lo")
-        self.add_to_config(" no shutdown")
-        for interface in self.interfaces:
-            self.add_interface(interface.id)
-            self.add_ip_address(interface.address.get_addr())
-        if self.log_file is not None:
-            self.add_to_config(f"log file {self.log_file}")
+        self.r0 = Node("r0")
+        self.r1 = Node("r1")
+        self.r0.enable_ip_forwarding()
+        self.r1.enable_ip_forwarding()
 
-    def run(self):
-        """
-        Runs the zebra daemon
-        """
-        super().run(
-            engine_func=partial(
-                run_zebra, self.router_ns_id, self.conf_file, self.pid_file
-            )
-        )
-
-    def handle_dependecy_error(self):
-        self.logger.error(
-            "Zebra not found. Routes from routing protocols cannot be added."
-        )
-        raise RequiredDependencyNotFound()
+        # populated later when we set the addresses
+        # to be used for pairwise ping tests
+        self.nodes_addresses = []
+
+        (eth_n0_r0, eth_r0_n0) = connect(self.n0, self.r0, "eth-n0_r0", "eth-r0_n0")
+        (eth_n1_r0, eth_r0_n1) = connect(self.n1, self.r0, "eth-n1_r0", "eth-r0_n1")
+
+        (eth_r0_r1, eth_r1_r0) = connect(self.r0, self.r1, "eth-r0_r1", "eth-r1_r0")
+
+        (eth_n2_r1, eth_r1_n2) = connect(self.n2, self.r1, "eth-n2_r1", "eth-r1_n2")
+        (eth_n3_r1, eth_r1_n3) = connect(self.n3, self.r1, "eth-n3_r1", "eth-r1_n3")
+
+        ### Assign addresses to interfaces ###
+        eth_n0_r0.set_address("10.0.1.1/24")
+        eth_r0_n0.set_address("10.0.1.2/24")
+        self.nodes_addresses.append((self.n0, "10.0.1.1"))
+
+        eth_n1_r0.set_address("10.0.1.3/24")
+        eth_r0_n1.set_address("10.0.1.4/24")
+        self.nodes_addresses.append((self.n1, "10.0.1.3"))
+
+        eth_r0_r1.set_address("10.0.2.5/24")
+        eth_r1_r0.set_address("10.0.2.6/24")
+
+        eth_r1_n2.set_address("10.0.3.7/24")
+        eth_n2_r1.set_address("10.0.3.8/24")
+        self.nodes_addresses.append((self.n2, "10.0.3.8"))
+
+        eth_r1_n3.set_address("10.0.3.9/24")
+        eth_n3_r1.set_address("10.0.3.10/24")
+        self.nodes_addresses.append((self.n3, "10.0.3.10"))
+
+    def tearDown(self):
+        delete_namespaces()
+        TopologyMap.delete_all_mapping()
+
+        ### Create interfaces and connect nodes and routers ###
+
+    def test_routing(self):
+        # this runs a DFS algorithm and populates routing tables accordingly
+        # If the graph is a tree, there is only one path for each pair\
+        # for non-trees, this will use a spanning tree found by DFS
+        RoutingHelper("static").populate_routing_tables()
+
+        # Ping between each pair of nodes
+        for node1, address1 in self.nodes_addresses:
+            for _, address2 in self.nodes_addresses:
+                if address1 != address2:
+                    status = node1.ping(address2, verbose=2)
+                    self.assertTrue(status)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `nest-0.4.1/nest/tests/test_address_helper.py` & `nest-0.4.2/nest/tests/test_address_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,59 @@
 # Copyright (c) 2019-2021 NITK Surathkal
 
 """Test APIs from topology sub-package"""
 
 import unittest
 import subprocess
 
-from nest.topology import Node, connect
+from nest.topology import Node, connect, Switch, Router
 from nest.clean_up import delete_namespaces
 from nest.topology_map import TopologyMap
 from nest.routing.routing_helper import RoutingHelper
 from nest.topology.network import Network
 from nest.topology.address_helper import AddressHelper
 
 # pylint: disable=missing-docstring
 # pylint: disable=invalid-name
 # pylint: disable=unused-variable
 # pylint: disable=consider-using-with
+# pylint: disable=too-many-instance-attributes
 
 
 class TestIPv4AddressHelper(unittest.TestCase):
     def setUp(self):
         self.n0 = Node("n0")
         self.n1 = Node("n1")
+        self.n2 = Node("n2")
+        self.n3 = Node("n3")
+        self.n4 = Node("n4")
+        self.n5 = Node("n5")
         self.net1 = Network("10.0.1.0/24")
         self.net2 = Network("10.0.2.0/24")
         self.net3 = Network("2001:101::/122")
         self.net4 = Network("2002:101::/122")
 
     def tearDown(self):
         delete_namespaces()
         TopologyMap.delete_all_mapping()
 
     def test_p2p(self):
         (n0_n1, n1_n0) = connect(self.n0, self.n1, network=self.net1)
 
         AddressHelper.assign_addresses()
 
-        status = self.n0.ping(n1_n0.get_address(), verbose=False)
+        status = self.n0.ping(n1_n0.get_address(), verbose=0)
         self.assertTrue(status)
 
     def test_p2p_ipv6(self):
         (n0_n1, n1_n0) = connect(self.n0, self.n1, network=self.net3)
 
         AddressHelper.assign_addresses()
 
-        status = self.n0.ping(n1_n0.get_address(), verbose=False)
+        status = self.n0.ping(n1_n0.get_address(), verbose=0)
         self.assertTrue(status)
 
     def test_prp(self):
         # pylint: disable=invalid-name
         r = Node("r")
         r.enable_ip_forwarding()
 
@@ -60,15 +65,15 @@
             (r_n1, n1_r) = connect(r, self.n1, network=self.net2)
 
         AddressHelper.assign_addresses()
 
         self.n0.add_route("DEFAULT", n0_r)
         self.n1.add_route("DEFAULT", n1_r)
 
-        status = self.n0.ping(n1_r.get_address(), verbose=False)
+        status = self.n0.ping(n1_r.get_address(), verbose=0)
 
         self.assertTrue(status)
 
     def test_prp_ipv6(self):
         # pylint: disable=invalid-name
         r = Node("r")
         r.enable_ip_forwarding()
@@ -80,15 +85,15 @@
             (r_n1, n1_r) = connect(r, self.n1, network=self.net4)
 
         AddressHelper.assign_addresses()
 
         self.n0.add_route("DEFAULT", n0_r)
         self.n1.add_route("DEFAULT", n1_r)
 
-        status = self.n0.ping(n1_r.get_address(), verbose=False)
+        status = self.n0.ping(n1_r.get_address(), verbose=0)
 
         self.assertTrue(status)
 
     def test_prrp(self):
         # pylint: disable=invalid-name
         r1 = Node("r")
         r2 = Node("r")
@@ -103,15 +108,15 @@
 
         AddressHelper.assign_addresses()
         r2_n1.set_address("10.1.3.2/24")
         n1_r2.set_address("10.1.3.1/24")
 
         RoutingHelper(protocol="rip").populate_routing_tables()
 
-        status = self.n0.ping(n1_r2.get_address(), verbose=False)
+        status = self.n0.ping(n1_r2.get_address(), verbose=0)
 
         self.assertTrue(status)
 
     def test_prrp_ipv6(self):
         # pylint: disable=invalid-name
         r1 = Node("r")
         r2 = Node("r")
@@ -124,17 +129,17 @@
         (r1_r2, r2_r1) = connect(r1, r2, network=self.net4)
         (r2_n1, n1_r2) = connect(r2, self.n1)
 
         AddressHelper.assign_addresses()
         r2_n1.set_address("2003:101::10:1/122")
         n1_r2.set_address("2003:101::10:2/122")
 
-        RoutingHelper(protocol="rip").populate_routing_tables()
+        RoutingHelper(protocol="rip", ipv6_routing=True).populate_routing_tables()
 
-        status = self.n0.ping(n1_r2.get_address(), verbose=False)
+        status = self.n0.ping(n1_r2.get_address(False, True, False), verbose=0)
 
         self.assertTrue(status)
 
     def test_tcp_param(self):
         self.n0.configure_tcp_param("ecn", "1")
         ecn = self.n0.read_tcp_param("ecn")
         self.assertEqual(ecn, "1")
@@ -150,10 +155,46 @@
             proc = subprocess.Popen(
                 command.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
             (stdout, _) = proc.communicate()
 
         self.assertEqual(stdout[:4], b"PING", "Invalid ping output")
 
+    def test_ip_addr_to_switch(self):
+        # pylint: disable=too-many-locals
+        s1 = Switch("s1")
+        s2 = Switch("s2")
+        r1 = Router("r1")
+
+        with self.net1:
+            (n0_s1, s1_n0) = connect(self.n0, s1)
+            (n1_s1, s1_n1) = connect(self.n1, s1)
+            (n2_s1, s1_n2) = connect(self.n2, s1)
+            (s1_r1, r1_s1) = connect(s1, r1)
+
+        with self.net2:
+            (n3_s2, s2_n3) = connect(self.n3, s2)
+            (n4_s2, s2_n4) = connect(self.n4, s2)
+            (n5_s2, s2_n5) = connect(self.n5, s2)
+            (s2_r1, r1_s2) = connect(s2, r1)
+
+        AddressHelper.assign_addresses()
+
+        self.n0.add_route("DEFAULT", n0_s1, r1_s1.address)
+        self.n1.add_route("DEFAULT", n1_s1, r1_s1.address)
+        self.n2.add_route("DEFAULT", n2_s1, r1_s1.address)
+        self.n3.add_route("DEFAULT", n3_s2, r1_s2.address)
+        self.n4.add_route("DEFAULT", n4_s2, r1_s2.address)
+        self.n5.add_route("DEFAULT", n5_s2, r1_s2.address)
+
+        # `Ping` from `n0` to 'n3', `n1` to `n4`, and `n2` to `n5`
+        status_1 = self.n0.ping(n3_s2.address)
+        status_2 = self.n1.ping(n4_s2.address)
+        status_3 = self.n2.ping(n5_s2.address)
+
+        self.assertTrue(status_1)
+        self.assertTrue(status_2)
+        self.assertTrue(status_3)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nest-0.4.1/nest/tests/test_input_validator.py` & `nest-0.4.2/nest/tests/test_input_validator.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/tests/test_offload.py` & `nest-0.4.2/nest/tests/test_offload.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/tests/test_routing_frr.py` & `nest-0.4.2/nest/tests/test_routing_bird_ipv4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """Test APIs from routing sub-package"""
 import unittest
-from os.path import isfile
 from nest import config
 from nest.topology_map import TopologyMap
 from nest.topology import Node, connect
 from nest.routing.routing_helper import RoutingHelper
 from nest.clean_up import delete_namespaces
 
 # pylint: disable=missing-docstring
-class TestFrr(unittest.TestCase):
+class TestBird(unittest.TestCase):
 
     # pylint: disable=invalid-name
     def setUp(self):
 
-        self.assertTrue(isfile("/usr/lib/frr/zebra"), "Frrouting is not installed")
-
         self.n0 = Node("n0")
         self.n1 = Node("n1")
         self.r0 = Node("r0")
         self.r1 = Node("r1")
         self.r0.enable_ip_forwarding()
         self.r1.enable_ip_forwarding()
 
@@ -38,15 +35,15 @@
 
         eth_r1r2.set_address("10.0.2.2/24")
         eth_r2r1.set_address("10.0.2.3/24")
 
         eth_r2p2.set_address("10.0.3.3/24")
         eth_p2r2.set_address("10.0.3.4/24")
 
-        config.set_value("routing_suite", "frr")  # Use frr
+        config.set_value("routing_suite", "bird")  # Use bird
 
     def tearDown(self):
         delete_namespaces()
         TopologyMap.delete_all_mapping()
 
     def test_routing_helper(self):
```

### Comparing `nest-0.4.1/nest/tests/test_routing_frr_ipv6.py` & `nest-0.4.2/nest/tests/test_routing_frr_ipv6.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,35 +40,51 @@
         eth_r1r2.set_address("10::2:2/122")
         eth_r2r1.set_address("10::2:3/122")
 
         eth_r2p2.set_address("10::3:3/122")
         eth_p2r2.set_address("10::3:4/122")
 
         config.set_value("routing_suite", "frr")  # Use frr
+        self.routing_helper = None
 
     def tearDown(self):
         delete_namespaces()
         TopologyMap.delete_all_mapping()
+        if self.routing_helper:
+            # pylint: disable=protected-access
+            self.routing_helper._clean_up()
 
     def test_rip_ipv6(self):
 
-        RoutingHelper("rip").populate_routing_tables()
+        self.routing_helper = RoutingHelper("rip", ipv6_routing=True)
+        self.routing_helper.populate_routing_tables()
 
-        status = self.n0.ping("10::3:4", verbose=False)
+        status = self.n0.ping("10::3:4", verbose=0)
         self.assertTrue(status)
 
-        status = self.n1.ping("10::1:1", verbose=False)
+        status = self.n1.ping("10::1:1", verbose=0)
         self.assertTrue(status)
 
     def test_ospf_ipv6(self):
 
-        RoutingHelper("ospf").populate_routing_tables()
+        self.routing_helper = RoutingHelper("ospf", ipv6_routing=True)
+        self.routing_helper.populate_routing_tables()
 
-        status = self.n0.ping("10::3:4", verbose=False)
+        status = self.n0.ping("10::3:4", verbose=0)
         self.assertTrue(status)
 
-        status = self.n1.ping("10::1:1", verbose=False)
+        status = self.n1.ping("10::1:1", verbose=0)
+        self.assertTrue(status)
+
+    def test_isis_ipv6(self):
+        self.routing_helper = RoutingHelper("isis", ipv6_routing=True)
+        self.routing_helper.populate_routing_tables()
+
+        status = self.n0.ping("10::3:4", verbose=0)
+        self.assertTrue(status)
+
+        status = self.n1.ping("10::1:1", verbose=0)
         self.assertTrue(status)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nest-0.4.1/nest/tests/test_routing_quagga.py` & `nest-0.4.2/nest/tests/test_routing_frr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """Test APIs from routing sub-package"""
-
 import unittest
 from glob import glob
+from os.path import isfile
 from nest import config
 from nest.topology_map import TopologyMap
 from nest.topology import Node, connect
 from nest.routing.routing_helper import RoutingHelper
 from nest.clean_up import delete_namespaces
 
 # pylint: disable=missing-docstring
-
-
-class TestQuagga(unittest.TestCase):
+class TestFrr(unittest.TestCase):
 
     # pylint: disable=invalid-name
     def setUp(self):
+
+        self.assertTrue(isfile("/usr/lib/frr/zebra"), "Frrouting is not installed")
+
         self.n0 = Node("n0")
         self.n1 = Node("n1")
         self.r0 = Node("r0")
         self.r1 = Node("r1")
         self.r0.enable_ip_forwarding()
         self.r1.enable_ip_forwarding()
 
@@ -38,70 +39,81 @@
 
         eth_r1r2.set_address("10.0.2.2/24")
         eth_r2r1.set_address("10.0.2.3/24")
 
         eth_r2p2.set_address("10.0.3.3/24")
         eth_p2r2.set_address("10.0.3.4/24")
 
-        config.set_value("routing_suite", "quagga")  # Use quagga
+        config.set_value("routing_suite", "frr")  # Use frr
+
+        self.routing_helper = None
 
     def tearDown(self):
         delete_namespaces()
         TopologyMap.delete_all_mapping()
+        if self.routing_helper:
+            # pylint: disable=protected-access
+            self.routing_helper._clean_up()
 
     def test_routing_helper(self):
 
-        RoutingHelper("rip").populate_routing_tables()
+        self.routing_helper = RoutingHelper("rip")
+        self.routing_helper.populate_routing_tables()
 
-        status = self.n0.ping("10.0.3.4", verbose=False)
+        status = self.n0.ping("10.0.3.4", verbose=0)
         self.assertTrue(status)
 
-        status = self.n1.ping("10.0.1.1", verbose=False)
+        status = self.n1.ping("10.0.1.1", verbose=0)
         self.assertTrue(status)
 
     def test_ospf(self):
-        RoutingHelper("ospf").populate_routing_tables()
+        self.routing_helper = RoutingHelper("ospf")
+        self.routing_helper.populate_routing_tables()
 
-        status = self.n0.ping("10.0.3.4", verbose=False)
+        status = self.n0.ping("10.0.3.4", verbose=0)
         self.assertTrue(status)
 
-        status = self.n1.ping("10.0.1.1", verbose=False)
+        status = self.n1.ping("10.0.1.1", verbose=0)
         self.assertTrue(status)
 
     def test_isis(self):
-        RoutingHelper("isis").populate_routing_tables()
+        self.routing_helper = RoutingHelper("isis")
+        self.routing_helper.populate_routing_tables()
 
-        status = self.n0.ping("10.0.3.4", verbose=False)
+        status = self.n0.ping("10.0.3.4", verbose=0)
         self.assertTrue(status)
 
-        status = self.n1.ping("10.0.1.1", verbose=False)
+        status = self.n1.ping("10.0.1.1", verbose=0)
         self.assertTrue(status)
 
-    def test_logs(self):
-        config.set_value("routing_logs", True)
-
-        RoutingHelper("rip").populate_routing_tables()
+    def test_babel(self):
+        with self.assertRaises(ValueError) as ex:
+            RoutingHelper("babel").populate_routing_tables()
 
-        self.assertTrue(len(glob(f"{config.get_value('routing_suite')}-logs_*")) > 0)
-
-        config.set_value("routing_logs", False)
+        self.assertEqual(
+            str(ex.exception),
+            "Supported routing protocols are rip, ospf, isis and static, "
+            "but got protocol babel",
+        )
 
-    def test_custom_node_routers(self):
-        RoutingHelper(
-            "rip", [self.n0, self.n1], [self.r0, self.r1]
-        ).populate_routing_tables()
+    def test_static(self):
+        RoutingHelper("static").populate_routing_tables()
 
-        status = self.n0.ping("10.0.3.4", verbose=False)
+        status = self.n0.ping("10.0.3.4", verbose=0)
         self.assertTrue(status)
 
-        status = self.n1.ping("10.0.1.1", verbose=False)
+        status = self.n1.ping("10.0.1.1", verbose=0)
         self.assertTrue(status)
 
-        with self.assertRaises(TypeError):
-            RoutingHelper("rip", self.n1, self.r1).populate_routing_tables()
+    def test_logs(self):
+        config.set_value("routing_logs", True)
 
-        with self.assertRaises(ValueError):
-            RoutingHelper("rip", ["n1"], ["r1"]).populate_routing_tables()
+        self.routing_helper = RoutingHelper("rip")
+        self.routing_helper.populate_routing_tables()
+
+        self.assertTrue(len(glob(f"{config.get_value('routing_suite')}-logs_*")) > 0)
+
+        config.set_value("routing_logs", False)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nest-0.4.1/nest/tests/test_static_routing_mpls.py` & `nest-0.4.2/nest/tests/test_static_routing_mpls.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         self.r0.add_route_mpls_switch(101, eth_r1_r0.get_address(), 102)
         self.r1.add_route_mpls_pop(102, eth_n1_r1.get_address())
 
         self.n1.add_route_mpls_push("10.0.1.0/24", eth_r1_n1.get_address(), 201)
         self.r1.add_route_mpls_switch(201, eth_r0_r1.get_address(), 202)
         self.r0.add_route_mpls_pop(202, eth_n0_r0.get_address())
 
-        status = self.n0.ping("10.0.3.4", verbose=True)
+        status = self.n0.ping("10.0.3.4", verbose=2)
         self.assertTrue(status)
 
-        status = self.n1.ping("10.0.1.1", verbose=True)
+        status = self.n1.ping("10.0.1.1", verbose=2)
         self.assertTrue(status)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nest-0.4.1/nest/tests/test_topology_address.py` & `nest-0.4.2/nest/tests/test_topology_address.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/tests/test_topology_address_ipv6.py` & `nest-0.4.2/nest/tests/test_topology_address_ipv6.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/tests/test_topology_map.py` & `nest-0.4.2/nest/tests/test_topology_map.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,86 @@
 # SPDX-License-Identifier: GPL-2.0-only
-# Copyright (c) 2019-2020 NITK Surathkal
+# Copyright (c) 2019-2022 NITK Surathkal
 
 """Test topology map API"""
 
 import unittest
+from nest.topology.device.device import Device
 from nest.topology_map import TopologyMap
+from nest.topology import Node, connect
 
 # pylint: disable=missing-docstring
 # pylint: disable=too-many-instance-attributes
 
 
 class TestTopologyMap(unittest.TestCase):
     def setUp(self):
-        # Define namespace id and names
-        self.ns_id1 = "ns_id1"
-        self.ns_id2 = "ns_id2"
-        self.ns_name1 = "ns_name1"
-        self.ns_name2 = "ns_name2"
-
-        # Add namespaces
-        TopologyMap.add_namespace(self.ns_id1, self.ns_name1)
-        TopologyMap.add_namespace(self.ns_id2, self.ns_name2)
-
-        # Define interface id and names
-        self.int_id1 = "int_id1"
-        self.int_id2 = "int_id2"
-        self.int_name1 = "int_name1"
-        self.int_name2 = "int_name2"
-
-        # Add interfaces
-        TopologyMap.add_interface(self.ns_id1, self.int_id1, self.int_name1)
-        TopologyMap.add_interface(self.ns_id1, self.int_id2, self.int_name2)
+        # Create nodes
+        ns1 = Node("n1")
+        ns2 = Node("n2")
+
+        # Get their corresponding ids and names
+        self.ns_id1 = ns1.id
+        self.ns_name1 = ns1.name
+        self.ns_id2 = ns2.id
+        self.ns_name2 = ns2.name
+
+        # Create veth pairs (interfaces)
+        (eth1, eth2) = connect(ns1, ns2)
+
+        # Get their corresponding ids and names
+        self.int_id1 = eth1.id
+        self.int_name1 = eth1.name
+        self.int_id2 = eth2.id
+        self.int_name2 = eth2.name
 
     def tearDown(self):
         TopologyMap.delete_all_mapping()
 
-    def test_add_and_get_namespace(self):
-        self.assertEqual(TopologyMap.get_namespace(self.ns_id1)["name"], self.ns_name1)
-        self.assertEqual(TopologyMap.get_namespace(self.ns_id2)["name"], self.ns_name2)
+    def test_add_and_get_node(self):
+        self.assertEqual(TopologyMap.get_node(self.ns_id1).name, self.ns_name1)
+        self.assertEqual(TopologyMap.get_node(self.ns_id2).name, self.ns_name2)
 
-    def test_add_and_get_interface(self):
+    def test_add_and_get_device(self):
         self.assertEqual(
-            TopologyMap.get_interface(self.ns_id1, self.int_id1)["name"], self.int_name1
+            TopologyMap.get_device(self.ns_id1, self.int_id1).name, self.int_name1
         )
         self.assertEqual(
-            TopologyMap.get_interface(self.ns_id1, self.int_id2)["name"], self.int_name2
+            TopologyMap.get_device(self.ns_id2, self.int_id2).name, self.int_name2
         )
 
     def test_add_same_entity_again(self):
+        dummy_node = Node("nd")
+        dummy_device = Device("device", None)
+
+        with self.assertRaises(ValueError):
+            TopologyMap.add_node(self.ns_id1, dummy_node)
         with self.assertRaises(ValueError):
-            TopologyMap.add_namespace(self.ns_id1, self.ns_name1)
+            TopologyMap.add_device(self.ns_id1, self.int_id1, dummy_device)
+
+    def test_delete_device(self):
+        device = TopologyMap.get_device(self.ns_id1, self.int_id1)
+
+        TopologyMap.delete_device(self.ns_id1, self.int_id1)
+        with self.assertRaises(ValueError):
+            TopologyMap.get_device(self.ns_id1, self.int_id1)
+
+        TopologyMap.add_device(self.ns_id1, self.int_id1, device)
+        self.assertEqual(
+            TopologyMap.get_device(self.ns_id1, self.int_id1).name, self.int_name1
+        )
+
+    def test_move_device(self):
+        TopologyMap.move_device(self.ns_id1, self.ns_id2, self.int_id1)
+
         with self.assertRaises(ValueError):
-            TopologyMap.add_interface(self.ns_id1, self.int_id1, self.int_name1)
+            TopologyMap.get_device(self.ns_id1, self.int_id1)
+
+        self.assertEqual(
+            TopologyMap.get_device(self.ns_id2, self.int_id1).name, self.int_name1
+        )
+
+        TopologyMap.move_device(self.ns_id2, self.ns_id1, self.int_id1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nest-0.4.1/nest/topology/__init__.py` & `nest-0.4.2/nest/topology/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 * Qdiscs are installed
 """
 
 import uuid
 
 from . import id_generator
 from .address import Address, Subnet
+from .interface import Interface
 from .node import Node
 from .router import Router
-from .interface import Interface, connect
 from .switch import Switch
 
+# pylint: disable=cyclic-import
+from .connect import connect
+
 
 # Generate unique topology id for the *to be created* topology
 TOPOLOGY_ID = uuid.uuid4().hex[:10]  # TODO: First 10 seems hacky
 id_generator.IdGen(TOPOLOGY_ID)
```

### Comparing `nest-0.4.1/nest/topology/address.py` & `nest-0.4.2/nest/topology/address.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/topology/address_helper.py` & `nest-0.4.2/nest/topology/address_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2021 NITK Surathkal
 
 """API related to Address Helper"""
 
 import logging
+from nest.input_validator.input_validator import input_validator
+from nest.topology.network import Network
 from nest.topology_map import TopologyMap
 from .address import Subnet
 
 # pylint: disable=too-few-public-methods
 
 logger = logging.getLogger(__name__)
 
 
 class AddressHelper:
     """
     Abstraction for automatic address assignment to interfaces of the network.
     """
 
     @staticmethod
-    def assign_addresses(network=None):
+    @input_validator
+    def assign_addresses(network: Network = None):
         """
         Assignment of addresses to the interfaces.
 
         Parameters
         ----------
         network : Network
             Assigning the addresses to each interfaces of all network.
             It will assign addresses to specific network if network object is mentioned.
         """
         if network is None:
-            for net in TopologyMap.list_of_network:
+
+            networks = TopologyMap.get_networks()
+            for net in networks:
                 AddressHelper.__assign_addresses_to_network(net)
 
             # Warning for the assignment of the addresses to the interfaces,
             # which do not belong to any network
             if TopologyMap.orphan_interfaces != 0:
                 logger.warning(
                     "Interfaces not part of some network. The addresses to these orphaned "
                     "interfaces should be manually added.",
                 )
         else:
             AddressHelper.__assign_addresses_to_network(network)
 
     @staticmethod
-    def __assign_addresses_to_network(network):
+    def __assign_addresses_to_network(network: Network):
         """
         Assignment of addresses to all interfaces of specific network.
 
         Parameters
         ----------
         network : Network
             Assigning the addresses to each interfaces of the given network object.
         """
-        _interface = []
-        _interface = network.interface
+        _interfaces = []
+        _interfaces = network.interfaces
 
         _net_address = Subnet(network.net_address)
 
-        for inter in _interface:
+        for inter in _interfaces:
             inter.set_address(_net_address.get_next_addr())
```

### Comparing `nest-0.4.1/nest/topology/id_generator.py` & `nest-0.4.2/nest/topology/id_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """Generate unique id for topology entity"""
 
+from threading import Lock
 from .. import config
 
 
 class IdGen:  # pylint: disable=too-few-public-methods
     """Generate unique id for Topology entities
 
 
@@ -20,14 +21,15 @@
         If unique Id's should be used for entity names
         (default is True)
 
     """
 
     topology_id = ""
     counter = 0
+    lock = Lock()
 
     def __init__(self, topology_id):
         """Initialize `topology_id`
 
         Parameters
         ----------
         topology_id: str
@@ -47,12 +49,13 @@
         Returns
         -------
         str
             If `is_unique_id` is true, then an unique id is returned
             Else, `name` is returned back
 
         """
-        if config.get_value("assign_random_names"):
-            IdGen.counter += 1
-            return IdGen.topology_id + "-" + str(IdGen.counter)
+        with IdGen.lock:
+            if config.get_value("assign_random_names"):
+                IdGen.counter += 1
+                return IdGen.topology_id + "-" + str(IdGen.counter)
 
-        return name
+            return name
```

### Comparing `nest-0.4.1/nest/topology/ifb.py` & `nest-0.4.2/nest/topology/device/ifb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2021 NITK Surathkal
 
 """API related to creation of IFB for qdiscs in topology"""
 
 import logging
-import nest.config as config
+from nest import config
 from nest import engine
-from nest.topology.device import Device
+from .device import Device
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable=too-many-instance-attributes
 
 
 class Ifb(Device):
@@ -87,20 +87,20 @@
             "dev": self.id,
         }
 
         # NOTE: Use Filter API
         # Action mirred, redicting traffic, etc is needed since netem and
         # the user giver qdisc are both classless and cannot be added to
         # the same device
-        engine.add_filter(
-            self.node_id,
+        self.add_filter(
             self.veth_end_id,
-            "all",
             "1",
             "u32",
+            "",  # flow id
+            "all",
             parent="1:",
             **action_redirect,
         )
 
     def set_bandwidth(self, bandwidth):
         """
         Set a maximum bandwidth for the ifb
@@ -126,13 +126,11 @@
             The Queueing algorithm to be added
         bandwidth :
             Link bandwidth
         """
 
         current_bandwidth_parameter = {"rate": self.current_bandwidth}
 
-        engine.change_class(
-            self.node_id, self.id, "1:", "htb", "1:1", **current_bandwidth_parameter
-        )
+        self.change_class("1:", "htb", "1:1", **current_bandwidth_parameter)
 
         self.delete_qdisc("11:")
         self.add_qdisc(qdisc, "1:1", "11:", **kwargs)
```

### Comparing `nest-0.4.1/nest/topology/network.py` & `nest-0.4.2/nest/topology/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2021 NITK Surathkal
 
 """API related to Network"""
 
 import logging
+
+# pylint: disable=unused-import
+import nest
 from nest.input_validator import input_validator
 from nest.topology_map import TopologyMap
 from .address import Address
 
 logger = logging.getLogger(__name__)
 
 
@@ -33,15 +36,15 @@
         ----------
         network_address : str
             IP address of the network
 
         """
 
         self.net_address = network_address
-        self.interface = []
+        self.interfaces = []
 
         # Adding each network's object reference to the static list of networks in topology_map.
         TopologyMap.add_network(self)
 
     def __enter__(self):
         """
         Enter the context of this `Network`.
@@ -54,22 +57,26 @@
         """
         Exit the context of this `Network`.
         """
         Network.current_network = None
 
     # TODO: Handle the get interface request using the interface list
 
-    def add_interface(self, _interface=None):
+    @input_validator
+    def add_interface(self, interface: "nest.topology.interface.BaseInterface"):
         """
         Adding interface to the network.
 
         Parameters
         ----------
-        _interface : interface
+        interface : BaseInterface
             The interface which needs to be added to the Network.
         """
-        self.interface.append(_interface)
-        TopologyMap.decrement_orphan_interfaces()
+        if interface not in self.interfaces:
+            self.interfaces.append(interface)
+            TopologyMap.decrement_orphan_interfaces()
+        else:
+            logger.debug("Ignore adding duplicate %s in %s", interface, self)
 
     def __repr__(self):
         classname = self.__class__.__name__
         return f"{classname}({self.net_address!r})"
```

### Comparing `nest-0.4.1/nest/topology/node.py` & `nest-0.4.2/nest/topology/node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """API related to node creation in topology"""
 
 import logging
+from multiprocessing.dummy import Process
+import time
 
-# pylint: disable=unused-import
-# pylint: disable=cyclic-import
-from nest import topology
 from nest import engine
+from nest.topology.interface import BaseInterface, Interface
+from nest.engine.t_shark import capture_packets
+from nest.engine.util import is_dependency_installed
 from nest.topology_map import TopologyMap
-import nest.config as config
+from nest import config
 from nest.network_utilities import ipv6_dad_check
 import nest.global_variables as g_var
 from nest.input_validator import input_validator
 from .address import Address
 from .id_generator import IdGen
 
 logger = logging.getLogger(__name__)
@@ -56,22 +58,27 @@
                 "%s is longer than 3 characters. It's safer to use "
                 "node names with atmost 3 characters with the current config.",
                 name,
             )
 
         self._name = name
         self._id = IdGen.get_id(name)
+
+        # TODO: This list maynot be accurate. Better to refer TopologyMap
+        # for list of interfaces in a Node.
         self._interfaces = []
+
         # Global variable disables when any new node is created
         # to ensure DAD check (if applicable)
         g_var.IS_DAD_CHECKED = False
+        self._tshark_processes = []
 
         engine.create_ns(self.id)
         engine.set_interface_mode(self.id, "lo", "up")
-        TopologyMap.add_namespace(self.id, self.name)
+        TopologyMap.add_node(self.id, self)
         TopologyMap.add_host(self)
 
     def __enter__(self):
         """
         Enter the context of this `Node`.
         For eg., all commands in this context will only be able to see
         interfaces inside this `Node`
@@ -82,51 +89,82 @@
     def __exit__(self, *args):
         """
         Exit the context of this `Node`
         """
         # Switch back to default network namespace
         engine.set_ns(None)
 
+    def __del__(self):
+        """
+        Destructor for node objects
+        """
+        for process in self._tshark_processes:
+            process.join()
+
     @input_validator
     def add_route(
         self,
         dest_addr: Address,
-        via_interface: "topology.Interface",
+        via_interface: BaseInterface,
         next_hop_addr: Address = None,
     ):
         """
         Add a route to the routing table of `Node`.
 
         Parameters
         ----------
         dest_addr: Address/str
             Destination IP address of node to route to. 'DEFAULT' is
             for all addresses
-        via_interface: Interface
+        via_interface: BaseInterface
             `Interface` in `Node` to route via
         next_hop_addr: Address/str, optional
             IP address of next hop Node (or router), by default ''
         """
         if next_hop_addr is None:
-            next_hop_addr = via_interface.pair.address
+
+            if isinstance(via_interface, Interface) is False:
+                raise ValueError(
+                    "Unable to automatically determine the next_hop_addr. Please"
+                    " provide the parameter explicitly."
+                )
+
+            via_interface_addresses = via_interface.pair.get_address(True, True, True)
+            if len(via_interface_addresses) > 1:
+                raise ValueError(
+                    "Please provide the next_hop_addr parameter, since the other"
+                    " end of the interface has multiple addresses assigned to it."
+                )
+            next_hop_addr = via_interface_addresses[0]
 
         dest_addr_str = ""
         if dest_addr.is_subnet():
             dest_addr_str = dest_addr.get_addr()
         else:
             dest_addr_str = dest_addr.get_addr(with_subnet=False)
 
         engine.add_route(
             self.id,
             dest_addr_str,
             next_hop_addr.get_addr(with_subnet=False),
             via_interface.id,
         )
 
-    def get_interface(self, node, connection_number=1):
+    def print_routes_to_file(self, *args):
+        """
+        Get the routes from the routing table of a Node.
+
+        Parameters
+        *args: Interface object
+        """
+
+        engine.get_route(self.id, *args)
+
+    @input_validator
+    def get_interface(self, node: "Node", connection_number: int = 1):
         """
         Get the interface in `self` connected to `node`.
         By default, this returns a veth interface.
 
         `connection_number` is an optional argument used when there
         multiple connections between `self` and `node`.
 
@@ -142,14 +180,18 @@
         -------
         Interface
             Return the interface between `self` and `node`. Use
             `connection_number` to uniquly identify an interface if
             there are multiple connections.
             If no interface is found, then return None.
         """
+        logger.warning(
+            "Node.get_interface method will be deprecated soon. Please avoid using this method."
+        )
+
         if connection_number <= 0:
             raise ValueError("connection_number should be greater than 0")
 
         for interface in self.interfaces:
             if hasattr(interface.pair, "node"):  # True if interface is a `veth`
                 pair_node = interface.pair.node
                 if node == pair_node:
@@ -213,21 +255,21 @@
         next_hop_addr: IP address of the next hop
 
         """
         engine.add_mpls_route_pop(
             self.id, incoming_label, next_hop_addr.get_addr(with_subnet=False)
         )
 
-    def _add_interface(self, interface):
+    def _add_interface(self, interface: BaseInterface):
         """
         Add `interface` to `Node`
 
         Parameters
         ----------
-        interface: Interface
+        interface: BaseInterface
             `Interface` to be added to `Node`
         """
         self._interfaces.append(interface)
         interface.node_id = self.id
         engine.add_int_to_ns(self.id, interface.id)
 
     def configure_tcp_param(self, param, value):
@@ -307,54 +349,80 @@
             is returned.
         """
         return engine.read_kernel_param(self.id, "net.ipv4.udp_", param)
 
     @ipv6_dad_check
     @input_validator
     def ping(
-        self, destination_address: Address, packets: int = 5, verbose: bool = True
+        self,
+        destination_address: Address,
+        preload: int = 1,
+        packets: int = 5,
+        verbose: int = 2,
     ):
         """
         Ping from current `Node` to destination address
         if there is a route.
 
         Parameters
         ----------
         destination_address: Address/str
             IP address to ping to
+        preload: int (Default is 1)
+            Number of packets sent as fast as possible without
+            waiting for reply.
         packets: int
             Number of ping packets sent
-        verbose: bool
-            If `True`, output ping packet details
+        verbose: int
+            If verbose = '0', no output is printed to stdout.
+            If verbose = '1', output if ping succeeded or failed.
+            If verbose = '2', output details of each ping packet.
 
         Returns
         -------
         bool
             `True` if `Node` can successfully ping `destination_address`.
             Else `False`.
         """
-        if isinstance(destination_address, str):
-            destination_address = Address(destination_address)
+        if verbose not in [0, 1, 2]:
+            raise ValueError(
+                f"Verbose parameter value is {verbose}. It should be 0, 1 or 2."
+            )
 
-        if verbose:
+        if verbose == 2:
             print()
             print(
                 f"=== PING from {self.name} to "
                 f"{destination_address.get_addr(with_subnet=False)} ==="
             )
             print()
 
         status = engine.ping(
             self.id,
             destination_address.get_addr(with_subnet=False),
+            preload,
             packets,
             destination_address.is_ipv6(),
-            live_output=verbose,
+            verbose == 2,
         )
 
+        if verbose == 1:
+            print()
+            if status is True:
+                print(
+                    f"SUCCESS : === PING from {self.name} to "
+                    f"{destination_address.get_addr(with_subnet=False)} ==="
+                )
+            elif status is False:
+                print(
+                    f"FAILURE: === PING from {self.name} to "
+                    f"{destination_address.get_addr(with_subnet=False)} ==="
+                )
+            print()
+
         return status
 
     def enable_ip_forwarding(self, ipv4=True, ipv6=True):
         """
         Enable IP forwarding in `Node`.
 
         After this method runs, the `Node` can be used as a router.
@@ -371,14 +439,69 @@
         """
         Disables Duplicate addresses Detection (DAD) for all interfaces of `Node`.
         """
         for i in range(len(self._interfaces)):
             interface_name = self._interfaces[i]
             interface_name.disable_ip_dad()
 
+    # pylint: disable=too-many-arguments
+    @input_validator
+    def capture_packets(
+        self,
+        interface: BaseInterface = None,
+        packet_count: int = None,
+        timeout: int = None,
+        output_file: str = None,
+        output_format: str = None,
+        **kwargs,
+    ):
+        """
+        Packets are captured from this node
+
+        Parameters
+        ----------
+        interface: BaseInterface
+            If the packets need to be captured from only one specific interface
+        """
+
+        install_status = is_dependency_installed("tshark")
+
+        if install_status is False:
+            logger.error(
+                "The system doesn't have tshark installed\n"
+                "Packet capture method requires this tool"
+            )
+
+        timestamp = time.strftime("%d-%m-%Y-%H:%M:%S")
+
+        if interface is not None:
+            kwargs["-i"] = interface.id
+
+        if packet_count is not None:
+            kwargs["-c"] = str(packet_count)
+
+        if timeout is not None:
+            kwargs["-a"] = f"duration:{timeout}"
+
+        if output_file is None:
+            if interface is None:
+                output_file = f"{self.name}_{timestamp}"
+            else:
+                output_file = f"{self.name}_{interface.name}_{timestamp}"
+        kwargs["-w"] = output_file
+
+        if output_format is not None:
+            kwargs["-T"] = output_format
+
+        t_shark_process = Process(
+            target=capture_packets, args=(self.id,), kwargs=kwargs
+        )
+        self._tshark_processes.append(t_shark_process)
+        t_shark_process.start()
+
     @property
     def id(self):
         """
         str: Value used by `engine` to create the emulated `Node` entity
         """
         return self._id
```

### Comparing `nest-0.4.1/nest/topology/router.py` & `nest-0.4.2/nest/topology/router.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest/topology/switch.py` & `nest-0.4.2/nest/topology/switch.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,47 +2,50 @@
 # Copyright (c) 2019-2021 NITK Surathkal
 
 """API related to switch creation in topology"""
 
 import logging
 
 from nest import engine
+from nest.topology.device.bridge import Bridge
+from nest.topology.interface import BaseInterface
 from nest.topology.node import Node
 
 logger = logging.getLogger(__name__)
 
 
-class Switch(Node):
+class Switch(Node, BaseInterface):
     """
     Abstraction for a switch.
 
     Attributes
     ----------
     name: str
         User given name for the switch.
     """
 
     def __init__(self, name):
         """
         Create a switch with given `name` inside a 'Node'.
 
         A namespace is created by inheriting the "Node" class and unique id is given
-        to the namespace. Then a switch with the same name and unique id as namespace
+        to the namespace. Then a bridge with the same name and unique id as namespace
         is created inside the created namespace.
 
         Parameters
         ----------
         name: str
             The name of the switch to be created
         """
-        super().__init__(name)
-        engine.create_switch(self.id, self.id)
-        engine.set_switch_mode(self.id, "up")
 
-    def _add_interface(self, interface):
+        Node.__init__(self, name)
+        _bridge = Bridge(name, self._id)
+        BaseInterface.__init__(self, name, _bridge)
+
+    def _add_interface(self, interface: BaseInterface):
         """
         Add `interface` to `Switch`
 
         Parameters
         ----------
         interface: Interface
             `Interface` to be added to `Switch`
```

### Comparing `nest-0.4.1/nest/topology/traffic_control.py` & `nest-0.4.2/nest/topology/device/traffic_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # Copyright (c) 2019-2020 NITK Surathkal
 
 """Handle traffic control entities"""
 
-from nest.topology_map import TopologyMap
-from .. import engine
+from nest import engine
 
 # TODO: Improve this module such that the below pylint disables are no
 # longer required
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-instance-attributes
@@ -63,17 +62,14 @@
         handle : string
             id of the filter (Default value = '')
         """
         self.qdisc_list.append(
             Qdisc(self.node_id, self.dev_id, qdisc, parent, handle, **kwargs)
         )
 
-        # Add qdisc to TopologyMap
-        TopologyMap.add_qdisc(self.node_id, self.dev_id, qdisc, handle, parent=parent)
-
     def change_qdisc(self, handle, qdisc="", **kwargs):
         """
         Change a qdisc that is already present in the device
 
         Parameters
         ----------
         handle : string
@@ -84,15 +80,14 @@
 
         for qdisc_member in self.qdisc_list:
             if qdisc_member.handle == handle:
                 # In case you want to just change kwargs
                 if qdisc == "":
                     qdisc = qdisc_member.qdisc
                 else:
-                    TopologyMap.change_qdisc(self.node_id, self.dev_id, qdisc, handle)
                     qdisc_member.qdisc = qdisc
                 engine.change_qdisc(
                     self.node_id,
                     self.dev_id,
                     qdisc,
                     qdisc_member.parent,
                     handle,
@@ -111,15 +106,14 @@
         # TODO: Handle this better by using the destructor in traffic-control
         counter = 0
         for qdisc in self.qdisc_list:
             if qdisc.handle == handle:
                 engine.delete_qdisc(
                     qdisc.node_id, qdisc.dev_id, qdisc.parent, qdisc.handle
                 )
-                TopologyMap.delete_qdisc(self.node_id, self.dev_id, handle)
                 del self.qdisc_list[counter]
                 break
             counter += 1
 
     def add_class(self, qdisc, parent="root", classid="", **kwargs):
         """
         Create an object that represents a class
@@ -181,14 +175,15 @@
                 del self.class_list[counter]
                 break
             counter += 1
 
     # pylint: disable=too-many-arguments
     def add_filter(
         self,
+        dev_id,
         priority,
         filtertype,
         flowid,
         protocol="ip",
         parent="root",
         handle="",
         **kwargs,
@@ -216,15 +211,15 @@
         """
         # TODO: Verify type of parameters
         # TODO: Reduce arguments to the engine functions by finding parent and handle automatically
 
         self.filter_list.append(
             Filter(
                 self.node_id,
-                self.dev_id,
+                dev_id,
                 protocol,
                 priority,
                 filtertype,
                 flowid,
                 parent,
                 handle,
                 **kwargs,
@@ -286,14 +281,22 @@
         self.dev_id = dev_id
         self.qdisc = qdisc
         self.parent = parent
         self.handle = handle
 
         engine.add_qdisc(node_id, dev_id, qdisc, parent, handle, **kwargs)
 
+    def __repr__(self):
+        classname = self.__class__.__name__
+        return (
+            f"{classname} node_id={self.node_id} "
+            + f"dev_id={self.dev_id} qdisc={self.qdisc} "
+            + f"parent={self.parent} handle={self.handle}"
+        )
+
 
 class Class:
     """Handle classes associated to qdisc"""
 
     def __init__(self, node_id, dev_id, qdisc, parent="root", classid="", **kwargs):
         """
         Constructor to create an object that represents a class
@@ -317,14 +320,21 @@
         self.dev_id = dev_id
         self.qdisc = qdisc  # NOTE: should be renamed to knid
         self.parent = parent
         self.classid = classid
 
         engine.add_class(node_id, dev_id, parent, qdisc, classid, **kwargs)
 
+    def __repr__(self):
+        classname = self.__class__.__name__
+        return (
+            f"{classname} node_id={self.node_id} dev_id={self.dev_id} "
+            + f"qdisc={self.qdisc} parent={self.parent} class_id={self.classid}"
+        )
+
 
 class Filter:
     """Handle filters to assign to class/qdisc"""
 
     def __init__(
         self,
         node_id,
@@ -370,7 +380,15 @@
         self.flowid = flowid
         self.parent = parent
         self.handle = handle
 
         engine.add_filter(
             node_id, dev_id, protocol, priority, filtertype, parent, handle, **kwargs
         )
+
+    def __repr__(self):
+        classname = self.__class__.__name__
+        return (
+            f"{classname} node_id={self.node_id} dev_id={self.dev_id} "
+            + f"protocol={self.protocol} priority={self.priority} filter_type={self.filtertype} "
+            + f"flow_id={self.flowid} parent={self.parent} handle={self.handle}"
+        )
```

### Comparing `nest-0.4.1/nest/user.py` & `nest-0.4.2/nest/user.py`

 * *Files identical despite different names*

### Comparing `nest-0.4.1/nest.egg-info/PKG-INFO` & `nest-0.4.2/nest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: nest
-Version: 0.4.1
+Version: 0.4.2
 Summary: NeST: Network Stack Tester
 Home-page: https://nest.nitk.ac.in/
 Author: NITK
 Author-email: nest@nitk.edu.in
-License: UNKNOWN
 Project-URL: Source, https://gitlab.com/nitk-nest/nest
 Keywords: network,namespace,linux
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
@@ -70,9 +68,7 @@
 ```
 
 **NOTE**: NeST requires **root** access currently to create and manage network namespaces.
 
 ## Contributing
 
 To contribute, read [CONTRIBUTING.md](https://gitlab.com/nitk-nest/nest/-/blob/master/CONTRIBUTING.md)
-
-
```

### Comparing `nest-0.4.1/nest.egg-info/SOURCES.txt` & `nest-0.4.2/nest.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 README.md
 setup.py
 nest/__init__.py
 nest/clean_up.py
 nest/config.json
 nest/config.py
 nest/exception.py
-nest/exceptions.py
 nest/global_variables.py
 nest/logging_helper.py
 nest/network_utilities.py
 nest/topology_map.py
 nest/user.py
 nest/version.py
 nest.egg-info/PKG-INFO
 nest.egg-info/SOURCES.txt
 nest.egg-info/dependency_links.txt
 nest.egg-info/requires.txt
 nest.egg-info/top_level.txt
 nest/engine/__init__.py
+nest/engine/coap.py
+nest/engine/coap_client.py
+nest/engine/coap_server.py
 nest/engine/dynamic_routing.py
 nest/engine/ethtool.py
 nest/engine/exec.py
 nest/engine/ip_address.py
 nest/engine/ip_link.py
 nest/engine/ip_mpls_route.py
 nest/engine/ip_netns.py
@@ -31,25 +33,29 @@
 nest/engine/iperf3.py
 nest/engine/ipv6_states.py
 nest/engine/iterators.py
 nest/engine/netperf.py
 nest/engine/ping.py
 nest/engine/setns.py
 nest/engine/sysctl.py
+nest/engine/t_shark.py
 nest/engine/tc.py
+nest/engine/tcp_modules.py
 nest/engine/uname.py
 nest/engine/util.py
 nest/experiment/__init__.py
 nest/experiment/experiment.py
 nest/experiment/interrupts.py
 nest/experiment/pack.py
 nest/experiment/results.py
 nest/experiment/run_exp.py
+nest/experiment/tools.py
 nest/experiment/info/README.txt
 nest/experiment/parser/__init__.py
+nest/experiment/parser/coap.py
 nest/experiment/parser/iperf3.py
 nest/experiment/parser/netperf.py
 nest/experiment/parser/ping.py
 nest/experiment/parser/runnerbase.py
 nest/experiment/parser/ss.py
 nest/experiment/parser/tc.py
 nest/experiment/parser/iterators/ss.sh
@@ -68,35 +74,49 @@
 nest/routing/__init__.py
 nest/routing/isis.py
 nest/routing/ldp.py
 nest/routing/ospf.py
 nest/routing/rip.py
 nest/routing/route_daemons.py
 nest/routing/routing_helper.py
+nest/routing/static_routing.py
 nest/routing/zebra.py
 nest/tests/__init__.py
 nest/tests/test_address_helper.py
 nest/tests/test_experiment.py
 nest/tests/test_input_validator.py
+nest/tests/test_iperf3_server_options.py
 nest/tests/test_offload.py
+nest/tests/test_routing_bird_ipv4.py
 nest/tests/test_routing_frr.py
 nest/tests/test_routing_frr_ipv6.py
+nest/tests/test_routing_frr_multi_address.py
 nest/tests/test_routing_quagga.py
 nest/tests/test_routing_quagga_ipv6.py
+nest/tests/test_routing_quagga_multi_address.py
+nest/tests/test_static_routing.py
 nest/tests/test_static_routing_mpls.py
 nest/tests/test_topology.py
 nest/tests/test_topology_address.py
 nest/tests/test_topology_address_ipv6.py
 nest/tests/test_topology_map.py
+nest/tests/test_topology_map_thread_safety.py
+nest/tests/test_topology_packet_ops.py
+nest/tests/test_topology_ping_preload.py
 nest/topology/__init__.py
 nest/topology/address.py
 nest/topology/address_helper.py
-nest/topology/device.py
+nest/topology/connect.py
 nest/topology/id_generator.py
-nest/topology/ifb.py
-nest/topology/interface.py
 nest/topology/network.py
 nest/topology/node.py
 nest/topology/router.py
 nest/topology/switch.py
-nest/topology/traffic_control.py
-nest/topology/veth_end.py
+nest/topology/device/__init__.py
+nest/topology/device/bridge.py
+nest/topology/device/device.py
+nest/topology/device/ifb.py
+nest/topology/device/traffic_control.py
+nest/topology/device/veth_end.py
+nest/topology/interface/__init__.py
+nest/topology/interface/base_interface.py
+nest/topology/interface/interface.py
```

### Comparing `nest-0.4.1/setup.py` & `nest-0.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,12 +47,12 @@
     packages=find_packages(),
     package_data={
         "nest.experiment": ["info/README.txt"],
         "nest.experiment.parser": ["iterators/*.sh"],
         "nest": ["config.json"],
     },
     python_requires=">=3.6, <4",
-    install_requires=["matplotlib", "numpy", "packaging", "tqdm"],
+    install_requires=["matplotlib", "numpy", "packaging", "tqdm", "aiocoap"],
     project_urls={
         "Source": "https://gitlab.com/nitk-nest/nest",
     },
 )
```

