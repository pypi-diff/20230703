# Comparing `tmp/p4p-4.1.8a1.tar.gz` & `tmp/p4p-4.1.8a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4p-4.1.8a1.tar", last modified: Tue Jun 27 02:03:30 2023, max compression
+gzip compressed data, was "p4p-4.1.8a2.tar", last modified: Mon Jul  3 00:24:09 2023, max compression
```

## Comparing `p4p-4.1.8a1.tar` & `p4p-4.1.8a2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.094581 p4p-4.1.8a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-27 02:02:50.000000 p4p-4.1.8a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-27 02:02:50.000000 p4p-4.1.8a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-27 02:03:30.094581 p4p-4.1.8a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-27 02:02:50.000000 p4p-4.1.8a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-27 02:02:50.000000 p4p-4.1.8a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 02:03:30.094581 p4p-4.1.8a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-06-27 02:02:50.000000 p4p-4.1.8a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.086581 p4p-4.1.8a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/_gw.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/_p4p.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/_p4p.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p/asLib/
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/asLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/asLib/lex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/asLib/pvlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/asLib/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p/client/
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/Qt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/client/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/disect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/example.conf
--rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/gw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p/nt/
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/nt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/nt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/nt/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/nt/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/nt/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvagw@.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p/pvxs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/client.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/log.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/nt.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/server.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/sharedArray.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/sharedpv.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/source.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/pvxs/version.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p/server/
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/server/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/server/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/server/cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/server/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/server/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/set.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.094581 p4p-4.1.8a1/src/p4p/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/asynciotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/cothreadtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/qttest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_asLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_client_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_client_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_gw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_sharedpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/test_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:03:30.090581 p4p-4.1.8a1/src/p4p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 02:03:30.000000 p4p-4.1.8a1/src/p4p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/p4p.h
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30046 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_gw.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_gw.h
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_odometer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_sharedpv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_source.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_type.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-27 02:02:50.000000 p4p-4.1.8a1/src/pvxs_value.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.315979 p4p-4.1.8a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 00:23:12.000000 p4p-4.1.8a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 00:23:12.000000 p4p-4.1.8a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-03 00:24:09.315979 p4p-4.1.8a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-03 00:23:12.000000 p4p-4.1.8a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 00:23:12.000000 p4p-4.1.8a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 00:24:09.315979 p4p-4.1.8a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-07-03 00:23:12.000000 p4p-4.1.8a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.303979 p4p-4.1.8a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.303979 p4p-4.1.8a2/src/p4p/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/_gw.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/_p4p.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/_p4p.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p/asLib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/pvlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/Qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/disect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/example.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/gw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p/nt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvagw@.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.311978 p4p-4.1.8a2/src/p4p/pvxs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/client.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/log.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/nt.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/server.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/sharedArray.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/sharedpv.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/source.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/version.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.311978 p4p-4.1.8a2/src/p4p/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/set.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.315979 p4p-4.1.8a2/src/p4p/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/asynciotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/cothreadtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/qttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_asLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_client_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_client_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_sharedpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30817 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_gw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_gw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_odometer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_sharedpv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_source.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_value.cpp
```

### Comparing `p4p-4.1.8a1/LICENSE` & `p4p-4.1.8a2/LICENSE`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/PKG-INFO` & `p4p-4.1.8a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4p
-Version: 4.1.8a1
+Version: 4.1.8a2
 Summary: Python interface to PVAccess protocol client
 Home-page: https://mdavidsaver.github.io/p4p
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `p4p-4.1.8a1/setup.py` & `p4p-4.1.8a2/setup.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/__init__.py` & `p4p-4.1.8a2/src/p4p/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/_gw.pyx` & `p4p-4.1.8a2/src/p4p/_gw.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -287,17 +287,17 @@
         cdef Report report
         cdef double cnorm = norm
         with nogil:
             report = self.provider.get().upstream.report()
 
         usinfo = []
         for conn in report.connections:
-            peer = conn.peer.decode()
+            peer = conn.peer.decode('utf-8', 'replace')
             for chan in conn.channels:
-                usinfo.append((chan.name.decode(), chan.tx/cnorm, chan.rx/cnorm, peer, conn.tx/cnorm, conn.rx/cnorm))
+                usinfo.append((chan.name.decode('utf-8', 'replace'), chan.tx/cnorm, chan.rx/cnorm, peer, conn.tx/cnorm, conn.rx/cnorm))
 
         return usinfo
 
     def use_count(self):
         return self.provider.use_count()
 
 def Server_report(_p4p.Server serv, float norm=1.0):
@@ -310,29 +310,29 @@
     cdef Report report
     cdef double cnorm = norm
     with nogil:
         report = serv.serv.report()
 
     dsinfo = []
     for conn in report.connections:
-        peer = conn.peer.decode()
+        peer = conn.peer.decode('utf-8', 'replace')
         if <bool>conn.credentials:
-            account = conn.credentials.get().account.decode()
+            account = conn.credentials.get().account.decode('utf-8', 'replace')
         else:
             account = ''
 
         for chan in conn.channels:
             info = dynamic_cast[GWChanInfoCP](chan.info.get())
 
             if info:
-                usname = info.usname.decode()
+                usname = info.usname.decode('utf-8', 'replace')
             else:
                 usname = ''
 
-            dsinfo.append((usname, chan.name.decode(), chan.tx/cnorm, chan.rx/cnorm, account, peer, conn.tx/cnorm, conn.rx/cnorm))
+            dsinfo.append((usname, chan.name.decode('utf-8', 'replace'), chan.tx/cnorm, chan.rx/cnorm, account, peer, conn.tx/cnorm, conn.rx/cnorm))
 
     return dsinfo
 
 # Allow GC to find handler stored in GWProvider
 #   https://github.com/cython/cython/issues/2737
 cdef traverseproc Provider_base_traverse
```

### Comparing `p4p-4.1.8a1/src/p4p/_p4p.pyx` & `p4p-4.1.8a2/src/p4p/_p4p.pyx`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/asLib/__init__.py` & `p4p-4.1.8a2/src/p4p/asLib/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/asLib/lex.py` & `p4p-4.1.8a2/src/p4p/asLib/lex.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/asLib/pvlist.py` & `p4p-4.1.8a2/src/p4p/asLib/pvlist.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/asLib/yacc.py` & `p4p-4.1.8a2/src/p4p/asLib/yacc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/client/Qt.py` & `p4p-4.1.8a2/src/p4p/client/Qt.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/client/asyncio.py` & `p4p-4.1.8a2/src/p4p/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/client/cli.py` & `p4p-4.1.8a2/src/p4p/client/cli.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/client/cothread.py` & `p4p-4.1.8a2/src/p4p/client/cothread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/client/raw.py` & `p4p-4.1.8a2/src/p4p/client/raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/client/thread.py` & `p4p-4.1.8a2/src/p4p/client/thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/disect.py` & `p4p-4.1.8a2/src/p4p/disect.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/example.conf` & `p4p-4.1.8a2/src/p4p/example.conf`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/gw.py` & `p4p-4.1.8a2/src/p4p/gw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/nt/__init__.py` & `p4p-4.1.8a2/src/p4p/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/nt/common.py` & `p4p-4.1.8a2/src/p4p/nt/common.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/nt/enum.py` & `p4p-4.1.8a2/src/p4p/nt/enum.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/nt/ndarray.py` & `p4p-4.1.8a2/src/p4p/nt/ndarray.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/nt/scalar.py` & `p4p-4.1.8a2/src/p4p/nt/scalar.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvagw@.service` & `p4p-4.1.8a2/src/p4p/pvagw@.service`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvxs/client.pxd` & `p4p-4.1.8a2/src/p4p/pvxs/client.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvxs/data.pxd` & `p4p-4.1.8a2/src/p4p/pvxs/data.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvxs/server.pxd` & `p4p-4.1.8a2/src/p4p/pvxs/server.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvxs/sharedArray.pxd` & `p4p-4.1.8a2/src/p4p/pvxs/sharedArray.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvxs/sharedpv.pxd` & `p4p-4.1.8a2/src/p4p/pvxs/sharedpv.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/pvxs/source.pxd` & `p4p-4.1.8a2/src/p4p/pvxs/source.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/rpc.py` & `p4p-4.1.8a2/src/p4p/rpc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/server/__init__.py` & `p4p-4.1.8a2/src/p4p/server/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/server/asyncio.py` & `p4p-4.1.8a2/src/p4p/server/asyncio.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/server/cli.py` & `p4p-4.1.8a2/src/p4p/server/cli.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/server/cothread.py` & `p4p-4.1.8a2/src/p4p/server/cothread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/server/raw.py` & `p4p-4.1.8a2/src/p4p/server/raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/server/thread.py` & `p4p-4.1.8a2/src/p4p/server/thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/set.pxd` & `p4p-4.1.8a2/src/p4p/set.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/asynciotest.py` & `p4p-4.1.8a2/src/p4p/test/asynciotest.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/cothreadtest.py` & `p4p-4.1.8a2/src/p4p/test/cothreadtest.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/qttest.py` & `p4p-4.1.8a2/src/p4p/test/qttest.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_asLib.py` & `p4p-4.1.8a2/src/p4p/test/test_asLib.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_client_raw.py` & `p4p-4.1.8a2/src/p4p/test/test_client_raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_client_thread.py` & `p4p-4.1.8a2/src/p4p/test/test_client_thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_gw.py` & `p4p-4.1.8a2/src/p4p/test/test_gw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_nt.py` & `p4p-4.1.8a2/src/p4p/test/test_nt.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_rpc.py` & `p4p-4.1.8a2/src/p4p/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_server.py` & `p4p-4.1.8a2/src/p4p/test/test_server.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_sharedpv.py` & `p4p-4.1.8a2/src/p4p/test/test_sharedpv.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_type.py` & `p4p-4.1.8a2/src/p4p/test/test_type.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/test_value.py` & `p4p-4.1.8a2/src/p4p/test/test_value.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/test/utils.py` & `p4p-4.1.8a2/src/p4p/test/utils.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/util.py` & `p4p-4.1.8a2/src/p4p/util.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p/version.py` & `p4p-4.1.8a2/src/p4p/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,8 +63,8 @@
     def __eq__(self, o):
         return self._cmp(o)==0
     def __ge__(self, o):
         return self._cmp(o)>=0
     def __gt__(self, o):
         return self._cmp(o)>0
 
-version = Version('4.1.8a1')
+version = Version('4.1.8a2')
```

### Comparing `p4p-4.1.8a1/src/p4p/wrapper.py` & `p4p-4.1.8a2/src/p4p/wrapper.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p.egg-info/PKG-INFO` & `p4p-4.1.8a2/src/p4p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4p
-Version: 4.1.8a1
+Version: 4.1.8a2
 Summary: Python interface to PVAccess protocol client
 Home-page: https://mdavidsaver.github.io/p4p
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `p4p-4.1.8a1/src/p4p.egg-info/SOURCES.txt` & `p4p-4.1.8a2/src/p4p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/p4p.h` & `p4p-4.1.8a2/src/p4p.h`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_client.cpp` & `p4p-4.1.8a2/src/pvxs_client.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_gw.cpp` & `p4p-4.1.8a2/src/pvxs_gw.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -329,71 +329,80 @@
             log_debug_printf(_logget, "'%s' GET exec issue %.03f\n", us->usname.c_str(), delay);
 
             // avoid ref loop GWGet::delay -> client::Operation -> GWChan -> GWUpstream -> GWGet
             std::weak_ptr<GWGet> wget(get);
             std::weak_ptr<client::Operation> wcliop(cliop);
             std::weak_ptr<GWUpstream> wus(us);
 
-            get->delay = sop->timerOneShot(delay, [wget, wus, wcliop](){
-                // on server worker
-                // 4. holdoff timer expires
-
-                auto get(wget.lock());
-                auto cliop(wcliop.lock());
-                auto us(wus.lock());
-                if(!get || !cliop || !us)
-                    return; // all downstream disconnect/cancel while holdoff running, and timer somehow not canceled.  Probably can't happen.
-
-                log_debug_printf(_logget, "'%s' GET holdoff expires\n", us->usname.c_str());
-
-                cliop->reExecGet([get, us](client::Result&& result) {
-                    // on client worker
-                    // 5. upstream provides result
-
-
-                    decltype (get->ops) ops;
-                    {
-                        Guard G(us->lock);
-                        assert(get->state==GWGet::Exec);
-                        get->state = GWGet::Idle;
-
-                        ops = std::move(get->ops);
-                    }
-
-                    try {
-                        auto value(result());
-                        log_debug_printf(_logget, "'%s' GET exec complete\n", us->usname.c_str());
-                        for(auto& op : ops) {
-                            op->reply(value);
+            pvxs::Timer dly;
+            {
+                UnGuard U(G);
+                dly = sop->timerOneShot(delay, [wget, wus, wcliop](){
+                    // on server worker
+                    // 4. holdoff timer expires
+
+                    auto get(wget.lock());
+                    auto cliop(wcliop.lock());
+                    auto us(wus.lock());
+                    if(!get || !cliop || !us)
+                        return; // all downstream disconnect/cancel while holdoff running, and timer somehow not canceled.  Probably can't happen.
+
+                    log_debug_printf(_logget, "'%s' GET holdoff expires\n", us->usname.c_str());
+
+                    cliop->reExecGet([get, us](client::Result&& result) {
+                        // on client worker
+                        // 5. upstream provides result
+
+
+                        decltype (get->ops) ops;
+                        {
+                            Guard G(us->lock);
+                            assert(get->state==GWGet::Exec);
+                            get->state = GWGet::Idle;
+
+                            ops = std::move(get->ops);
                         }
-                    }catch(std::exception& e){
-                        log_debug_printf(_logget, "'%s' GET exec complete err='%s'\n", us->usname.c_str(), e.what());
-                        for(auto& op : ops) {
-                            op->error(e.what());
+
+                        try {
+                            auto value(result());
+                            log_debug_printf(_logget, "'%s' GET exec complete\n", us->usname.c_str());
+                            for(auto& op : ops) {
+                                op->reply(value);
+                            }
+                        }catch(std::exception& e){
+                            log_debug_printf(_logget, "'%s' GET exec complete err='%s'\n", us->usname.c_str(), e.what());
+                            for(auto& op : ops) {
+                                op->error(e.what());
+                            }
                         }
-                    }
-                });
+                    });
 
-                // note time at which upstream GET is issued
-                get->lastget = epicsTime::getCurrent();
-                get->firstget = false;
-            });
+                    // note time at which upstream GET is issued
+                    get->lastget = epicsTime::getCurrent();
+                    get->firstget = false;
+                });
+            }
 
+            get->delay = std::move(dly);
             get->state = GWGet::Exec;
             get->ops.emplace_back(std::move(sop));
             break;
         }
         case GWGet::Exec:
             // combine with in progress upstream GET
             log_debug_printf(_logget, "'%s' GET exec combine\n", us->usname.c_str());
             get->ops.emplace_back(std::move(sop));
             break;
         case GWGet::Error:
             log_debug_printf(_logget, "'%s' GET exec error: %s\n", us->usname.c_str(), get->error.c_str());
-            sop->error(get->error);
+        {
+            auto msg(get->error);
+            UnGuard U(G);
+            sop->error(msg);
+        }
             break;
         }
     });
 }
 
 static
 void onGetPut(const std::shared_ptr<GWChan>& pv, const std::shared_ptr<server::ConnectOp>& ctrl)
@@ -570,19 +579,26 @@
 
             for(auto& ctrl : sub->controls)
                 ctrl->post(val);
 
          } catch(client::Finished&) {
             log_debug_printf(_logmon, "'%s' MONITOR finish\n", cli->name().c_str());
 
-            Guard G(pv->us->lock);
-            pv->us->subscription.reset();
-            for(auto& ctrl : sub->setups)
+            decltype (pv->us->subscription) trash;
+            decltype (sub->setups) setups;
+            decltype (sub->controls) controls;
+            {
+                Guard G(pv->us->lock);
+                trash = std::move(pv->us->subscription);
+                setups = std::move(sub->setups);
+                controls = std::move(sub->controls);
+            }
+            for(auto& ctrl : setups)
                 ctrl->error("Shared monitor finished before starting");
-            for(auto& ctrl : sub->controls)
+            for(auto& ctrl : controls)
                 ctrl->finish();
 
          } catch(std::exception& e) {
             log_warn_printf(_logmon, "'%s' MONITOR error: %s\n",
                             cli->name().c_str(), e.what());
          }
     }
@@ -659,18 +675,22 @@
 
             try {
                 cli.pop(); // expected to throw
                 throw std::runtime_error("not error??");
             }catch(std::exception& e){
                 log_warn_printf(_logmon, "'%s' MONITOR setup error: %s\n", cli.name().c_str(), e.what());
 
-                Guard G(pv->us->lock);
-                pv->us->subscription.reset();
-                sub->state = GWSubscription::Error;
-                for(auto& op : sub->setups)
+                decltype (pv->us->subscription) trash;
+                decltype (sub->setups) setups;
+                {
+                    Guard G(pv->us->lock);
+                    trash = std::move(pv->us->subscription);
+                    setups = std::move(sub->setups);
+                }
+                for(auto& op : setups)
                     op->error(e.what());
             }
         })
                 .onInit([sub, pv](client::Subscription& cli, const Value& prototype)
         {
             // on client worker
```

### Comparing `p4p-4.1.8a1/src/pvxs_gw.h` & `p4p-4.1.8a2/src/pvxs_gw.h`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_odometer.cpp` & `p4p-4.1.8a2/src/pvxs_odometer.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_sharedpv.cpp` & `p4p-4.1.8a2/src/pvxs_sharedpv.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_source.cpp` & `p4p-4.1.8a2/src/pvxs_source.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_type.cpp` & `p4p-4.1.8a2/src/pvxs_type.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a1/src/pvxs_value.cpp` & `p4p-4.1.8a2/src/pvxs_value.cpp`

 * *Files identical despite different names*

