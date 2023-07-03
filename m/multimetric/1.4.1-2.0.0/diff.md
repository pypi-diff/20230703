# Comparing `tmp/multimetric-1.4.1.tar.gz` & `tmp/multimetric-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimetric-1.4.1.tar", last modified: Fri Jun  9 19:33:56 2023, max compression
+gzip compressed data, was "multimetric-2.0.0.tar", last modified: Mon Jul  3 14:01:30 2023, max compression
```

## Comparing `multimetric-1.4.1.tar` & `multimetric-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,86 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/
--rw-r--r--   0 jason     (1000) jason     (1000)     1455 2023-03-27 09:19:53.000000 multimetric-1.4.1/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)       59 2023-03-27 09:12:10.000000 multimetric-1.4.1/MANIFEST.in
--rw-r--r--   0 jason     (1000) jason     (1000)     1008 2023-06-09 19:33:56.156608 multimetric-1.4.1/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     7393 2023-03-27 09:12:25.000000 multimetric-1.4.1/README.md
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/
--rw-r--r--   0 jason     (1000) jason     (1000)       18 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4386 2023-03-27 09:12:25.000000 multimetric-1.4.1/multimetric/__main__.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)      722 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/base.py
--rw-r--r--   0 jason     (1000) jason     (1000)      278 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/base_calc.py
--rw-r--r--   0 jason     (1000) jason     (1000)      284 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/base_stats.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/calc/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3377 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/halstead.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1967 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/maintenance.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2192 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/pylint.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4628 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/calc/tiobe.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/importer/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1061 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/base.py
--rw-r--r--   0 jason     (1000) jason     (1000)      375 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/filtered.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/importer/mods/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/mods/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)      534 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/mods/csv.py
--rw-r--r--   0 jason     (1000) jason     (1000)      686 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/mods/json.py
--rw-r--r--   0 jason     (1000) jason     (1000)      553 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/importer/pick.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/metric/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1714 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/comments.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1681 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/cyclomatic.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4257 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/fanout.py
--rw-r--r--   0 jason     (1000) jason     (1000)      907 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/loc.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2394 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/operands.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1583 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/metric/operators.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2107 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/modules.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric/cls/stats/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/stats/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1357 2023-03-27 09:12:10.000000 multimetric-1.4.1/multimetric/cls/stats/stats.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1680 2023-03-27 09:12:25.000000 multimetric-1.4.1/multimetric/fp.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-09 19:33:56.156608 multimetric-1.4.1/multimetric.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)     1008 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     1197 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       58 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/entry_points.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/requires.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       12 2023-06-09 19:33:56.000000 multimetric-1.4.1/multimetric.egg-info/top_level.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       32 2023-06-09 19:24:40.000000 multimetric-1.4.1/requirements.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-06-09 19:33:56.156608 multimetric-1.4.1/setup.cfg
--rw-r--r--   0 jason     (1000) jason     (1000)     1757 2023-06-09 19:30:02.000000 multimetric-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.399713 multimetric-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-03 14:01:10.000000 multimetric-2.0.0/LICENSE.Zlib
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 14:01:10.000000 multimetric-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 14:01:30.399713 multimetric-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-03 14:01:10.000000 multimetric-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/cls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/base_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/base_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/cls/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/calc/halstead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/calc/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/calc/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/calc/tiobe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/cls/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/filtered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/cls/importer/mods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/mods/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/mods/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/importer/pick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/cls/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/cyclomatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/metric/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric/cls/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-03 14:01:10.000000 multimetric-2.0.0/multimetric/cls/tokentree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.395713 multimetric-2.0.0/multimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 14:01:30.000000 multimetric-2.0.0/multimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-03 14:01:30.000000 multimetric-2.0.0/multimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:01:30.000000 multimetric-2.0.0/multimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 14:01:30.000000 multimetric-2.0.0/multimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 14:01:30.000000 multimetric-2.0.0/multimetric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 14:01:30.000000 multimetric-2.0.0/multimetric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 14:01:10.000000 multimetric-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 14:01:30.399713 multimetric-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 14:01:30.000000 multimetric-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:01:30.399713 multimetric-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_calc_halstead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_calc_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_coffeescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_cornercases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_csharp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_dart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_groovy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_haskell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_import_cornercases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_import_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_import_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_kotlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_lua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_objective_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_perl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_tcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-03 14:01:10.000000 multimetric-2.0.0/tests/test_zig.py
```

### Comparing `multimetric-1.4.1/PKG-INFO` & `multimetric-2.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 1.4.1
+Version: 2.0.0
 Summary: Calculate code metrics in various languages
-Home-page: https://github.com/startupos/multimetric
-Author: Jason Nichols
-Author-email: jn@ayl.us
+Home-page: https://github.com/priv-kweihmann/multimetric
+Author: Konrad Weihmann
+Author-email: kweihmann@outlook.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.10
 Description-Content-Type: text/plain
-License-File: LICENSE
+License-File: LICENSE.Zlib
+
+See https://github.com/priv-kweihmann/multimetric for documentation
 
-See https://github.com/startupos/multimetric for documentation
```

### Comparing `multimetric-1.4.1/multimetric/cls/calc/halstead.py` & `multimetric-2.0.0/multimetric/cls/calc/halstead.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
+import math
+
 from multimetric.cls.base_calc import MetricBaseCalc
 from multimetric.cls.metric.operands import MetricBaseOperands
 from multimetric.cls.metric.operators import MetricBaseOperator
-import math
 
 
 class MetricBaseCalcHalstead(MetricBaseCalc):
 
-    BUGPRED_METHOD = {
-        "old": "(self._effort * (2.0 / 3.0)) / 3000.0",
-        "new": "self._volume / 3000.0"
-    }
-
-    BUGPRED_DEFAULT = "new"
-
     METRIC_HALSTEAD_VOLUME = "halstead_volume"
     METRIC_HALSTEAD_EFFORT = "halstead_effort"
     METRIC_HALSTEAD_DIFFICULTY = "halstead_difficulty"
     METRIC_HALSTEAD_BUGS = "halstead_bugprop"
     METRIC_HALSTEAD_TIMEREQ = "halstead_timerequired"
 
+    @staticmethod
+    def _bugpred_old(obj):
+        return (obj._effort * (2.0 / 3.0)) / 3000.0
+
+    @staticmethod
+    def _bugpred_new(obj):
+        return obj._volume / 3000.0
+
+    BUGPRED_DEFAULT = "new"
+    BUGPRED_METHOD = {
+        "old": _bugpred_old,
+        "new": _bugpred_new,
+    }
+
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
-        try:
-            self.__bugPredicMethod = args.halstead_bug_predict_method
-        except AttributeError:
-            self.__bugPredicMethod = MetricBaseCalcHalstead.BUGPRED_DEFAULT
+        self.__bugPredicMethod = args.halstead_bug_predict_method
 
     def _getNs(self, metrics):
         self._N2 = float(metrics[MetricBaseOperands.METRIC_OPERANDS_SUM])
         self._N1 = float(metrics[MetricBaseOperator.METRIC_OPERATORS_SUM])
         self._n2 = float(metrics[MetricBaseOperands.METRIC_OPERANDS_UNIQUE])
         self._n1 = float(metrics[MetricBaseOperator.METRIC_OPERATORS_UNIQUE])
         # to avoid any Divbyzero bugs set the minimum to 1
@@ -71,15 +78,15 @@
     def _getTime(self, metrics):
         self._getEffort(metrics)
         self._timeRequired = self._effort / 18.0
         return self._timeRequired
 
     def _getBug(self, metrics):
         self._getEffort(metrics)
-        self._bug = eval(MetricBaseCalcHalstead.BUGPRED_METHOD[self.__bugPredicMethod])
+        self._bug = MetricBaseCalcHalstead.BUGPRED_METHOD[self.__bugPredicMethod](self)
         return self._bug
 
     def get_results(self, metrics):
         metrics[MetricBaseCalcHalstead.METRIC_HALSTEAD_VOLUME] = self._getVolume(metrics)
         metrics[MetricBaseCalcHalstead.METRIC_HALSTEAD_DIFFICULTY] = self._getDifficulty(metrics)
         metrics[MetricBaseCalcHalstead.METRIC_HALSTEAD_EFFORT] = self._getEffort(metrics)
         metrics[MetricBaseCalcHalstead.METRIC_HALSTEAD_TIMEREQ] = self._getTime(metrics)
```

### Comparing `multimetric-1.4.1/multimetric/cls/calc/maintenance.py` & `multimetric-2.0.0/multimetric/cls/calc/maintenance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,65 @@
-from multimetric.cls.base_calc import MetricBaseCalc
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
+import math
 
-import math  # noqa: F401
+from multimetric.cls.base_calc import MetricBaseCalc
 
 
 class MetricBaseCalcMaintenanceIndex(MetricBaseCalc):
 
-    MI_METHOD = {
-        "sei": '171.0 \
-             - (5.2 * math.log2(metrics["halstead_volume"])) \
-             - (0.23 * metrics["cyclomatic_complexity"]) \
-             - (16.2 * math.log2(metrics["loc"])) \
-             + (50.0 * math.sin(math.sqrt(2.4 * metrics["comment_ratio"])))',
-        "classic": '171.0 \
-            - (5.2 * math.log(metrics["halstead_volume"])) \
-            - (0.23 * metrics["cyclomatic_complexity"]) \
-            - (16.2 * math.log(metrics["loc"]))',
-        "microsoft": 'max(0, \
-                171.0 \
-                - (5.2 * math.log(metrics["halstead_volume"])) \
-                - (0.23 * metrics["cyclomatic_complexity"]), \
-                - (16.2 * math.log(metrics["loc"]) * 100.0 / 171.0))'
-    }
-
     MI_DEFAULT = "classic"
 
     METRIC_MAINTAINABILITY_INDEX = "maintainability_index"
 
+    @staticmethod
+    def _mi_sei(metrics):
+        try:
+            res = 171.0 - (5.2 * math.log2(metrics["halstead_volume"]))
+            res -= (0.23 * metrics["cyclomatic_complexity"])
+            res -= (16.2 * math.log2(metrics["loc"]))
+            res += (50.0 * abs(math.sin(math.sqrt(2.4 * metrics["comment_ratio"]))))
+            return res
+        except ValueError:  # pragma: no cover
+            return 0  # pragma: no cover
+
+    @staticmethod
+    def _mi_microsoft(metrics):
+        try:
+            res = 171.0
+            res -= (5.2 * math.log(metrics["halstead_volume"]))
+            res -= (0.23 * metrics["cyclomatic_complexity"])
+            res -= (16.2 * math.log(metrics["loc"]) * 100.0 / 171.0)
+            return max(0, res)
+        except ValueError:
+            return 0
+
+    @staticmethod
+    def _mi_classic(metrics):
+        try:
+            res = 171.0
+            res -= (5.2 * math.log(metrics["halstead_volume"]))
+            res -= (0.23 * metrics["cyclomatic_complexity"])
+            res -= (16.2 * math.log(metrics["loc"]))
+            return max(0, res)
+        except ValueError:  # pragma: no cover
+            return 0  # pragma: no cover
+
+    MI_METHOD = {
+        "sei": _mi_sei,
+        "classic": _mi_microsoft,
+        "microsoft": _mi_classic,
+    }
+
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
-        try:
-            self.__miMethod = args.maintenance_index_calc_method
-        except AttributeError:
-            self.__miMethod = MetricBaseCalcMaintenanceIndex.MI_DEFAULT
+        self.__miMethod = args.maintenance_index_calc_method
 
     def get_results(self, metrics):
-        try:
-            metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX] = eval(
-                MetricBaseCalcMaintenanceIndex.MI_METHOD[self.__miMethod])
-        except Exception as e:
-            metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX]=0
+        metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX] = MetricBaseCalcMaintenanceIndex.MI_METHOD[self.__miMethod](
+            metrics)
         # Sanity
         metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX] = max(
             metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX], 0)
         metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX] = min(
             metrics[MetricBaseCalcMaintenanceIndex.METRIC_MAINTAINABILITY_INDEX], 100)
         return super().get_results(metrics)
```

### Comparing `multimetric-1.4.1/multimetric/cls/calc/pylint.py` & `multimetric-2.0.0/multimetric/cls/calc/pylint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,48 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.base_calc import MetricBaseCalc
 from multimetric.cls.metric.operators import MetricBaseOperator
 from multimetric.cls.metric.operands import MetricBaseOperands
 
 
 class MetricBaseCalcPylint(MetricBaseCalc):
 
     METRIC_PYLINT = "pylint"
 
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
         self.__addArgs = kwargs
 
     def __getFromImporter(self, section, severity, _default=0.0):
-        if "import_{}".format(section) in self.__addArgs:
-            return self.__addArgs["import_{}".format(section)].getSumItems(
-                _filter={"severity": severity}
+        if f"import_{section}" in self.__addArgs:
+            return self.__addArgs[f"import_{section}"].getSumItems(
+                _filter={"severity": severity},
             )
         return _default
 
     def __getError(self, metrics):
         return (self.__getFromImporter("compiler", "error") +
                 self.__getFromImporter("functional", "error") +
                 self.__getFromImporter("standard", "error") +
                 self.__getFromImporter("security", "error")) * 5.0
 
     def __getWarning(self, metrics):
-        return self.__getFromImporter("compiler", "warning") + \
-            self.__getFromImporter("functional", "warning") + \
-            self.__getFromImporter("standard", "warning") + \
-            self.__getFromImporter("security", "warning")
+        return (self.__getFromImporter("compiler", "warning") +
+                self.__getFromImporter("functional", "warning") +
+                self.__getFromImporter("standard", "warning") +
+                self.__getFromImporter("security", "warning"))
 
     def __getInfo(self, metrics):
-        return self.__getFromImporter("compiler", "info") + \
-            self.__getFromImporter("functional", "info") + \
-            self.__getFromImporter("standard", "info") + \
-            self.__getFromImporter("security", "info")
+        return (self.__getFromImporter("compiler", "info") +
+                self.__getFromImporter("functional", "info") +
+                self.__getFromImporter("standard", "info") +
+                self.__getFromImporter("security", "info"))
 
     def __getScore(self, metrics):
-        # 100.0 - ((float(5 * error + warning + refactor + convention) / statement) * 100.0)
         _statements = (metrics[MetricBaseOperands.METRIC_OPERANDS_SUM] +
                        metrics[MetricBaseOperator.METRIC_OPERATORS_SUM]) or 1.0
         return max(100.0 - ((float(self.__getError(metrics) +
                                    self.__getWarning(metrics) +
                                    self.__getInfo(metrics)) /
                             _statements) * 100.0), 0.0)
```

### Comparing `multimetric-1.4.1/multimetric/cls/calc/tiobe.py` & `multimetric-2.0.0/multimetric/cls/calc/tiobe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,16 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 import math
 
 from multimetric.cls.base_calc import MetricBaseCalc
 from multimetric.cls.metric.cyclomatic import MetricBaseCyclomaticComplexity
 from multimetric.cls.metric.fanout import MetricBaseFanout
 from multimetric.cls.metric.loc import MetricBaseLOC
 
-def fail_safe(fn):
-    def wrapper(*args, **kwargs):
-        try:
-            return fn(*args, **kwargs)
-        except Exception as e:
-            return 0
-    return wrapper
-
-
 
 class MetricBaseCalcTIOBE(MetricBaseCalc):
 
     METRIC_TIOBE_COVERAGE = "tiobe_coverage"
     METRIC_TIOBE_FUNCTIONAL = "tiobe_functional"
     METRIC_TIOBE_COMPLEXITY = "tiobe_complexity"
     METRIC_TIOBE_COMPILER = "tiobe_compiler"
@@ -26,78 +19,67 @@
     METRIC_TIOBE_FANOUT = "tiobe_fanout"
     METRIC_TIOBE_SECURITY = "tiobe_security"
     METRIC_TIOBE = "tiobe"
 
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
         self.__addArgs = kwargs
-    
-    @fail_safe
+
     def __getScaledValue(self, metrics, value):
-        return 100.0 / ((value) / (metrics[MetricBaseLOC.METRIC_LOC] / 1000.0) + 1.0)
+        try:
+            return 100.0 / ((value) / (metrics[MetricBaseLOC.METRIC_LOC] / 1000.0) + 1.0)
+        except ZeroDivisionError:
+            return 0.0
 
-    @fail_safe
     def __getFromImporter(self, section, _default=0.0):
-        if "import_{}".format(section) in self.__addArgs:
-            return self.__addArgs["import_{}".format(section)].getSumItems()
+        if f"import_{section}" in self.__addArgs:
+            return self.__addArgs[f"import_{section}"].getSumItems()
         return _default
 
-    @fail_safe
     def __getTiobeComplexity(self, metrics):
         cc = metrics[MetricBaseCyclomaticComplexity.METRIC_CYCLOMATIC_COMPLEXITY]
         return 6400.0 / float(math.pow(cc, 3) - math.pow(cc, 2) - cc + 65)
 
-    @fail_safe
     def __getTiobeFanout(self, metrics):
         _int = metrics[MetricBaseFanout.METRIC_FANOUT_INTERNAL]
         _ext = metrics[MetricBaseFanout.METRIC_FANOUT_EXTERNAL]
         return float(min(max(120.0 - ((8.0 * _int) + (2.0 * _ext)), 0.0), 100.0))
 
-    @fail_safe
     def __getTiobeCoverage(self, metrics):
-        _per = self.__getFromImporter("coverage", _default=100.0)
-        if _per < 1.0:
-            # No coverage
-            return 0.0
+        _per = max(0.0, self.__getFromImporter("coverage", _default=100.0))
         return min(((0.75 * _per) + 32.5), 100.0)
 
-    @fail_safe
     def __getTiobeStandard(self, metrics):
         return self.__getScaledValue(metrics, self.__getFromImporter("standard"))
 
-    @fail_safe
     def __getTiobeSecurity(self, metrics):
         return self.__getScaledValue(metrics, self.__getFromImporter("security"))
 
-    @fail_safe
     def __getTiobeDuplication(self, metrics):
         return min(-30.0 * math.log10(self.__getFromImporter("duplication") or 0.00001) +
                    70.0, 100.0)
-    
-    @fail_safe
+
     def __getTiobeCompiler(self, metrics):
         _violations = self.__getScaledValue(metrics, self.__getFromImporter("compiler"))
         return max(100.0 - 50.0 *
                    math.log((101 - _violations) or 0.00001), 0.0)
 
-    @fail_safe
     def __getTiobeFunctional(self, metrics):
         _violations = self.__getFromImporter("functional")
         return max(self.__getScaledValue(metrics, _violations) * 2.0 - 100.0, 0.0)
 
-    @fail_safe
     def __getTiobe(self, metrics):
-        return (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COVERAGE] * 0.2) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_FUNCTIONAL] * 0.2) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COMPLEXITY] * 0.15) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COMPILER] * 0.15) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_STANDARD] * 0.1) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_DUPLICATION] * 0.1) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_FANOUT] * 0.05) + \
-               (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_SECURITY] * 0.05)
+        return ((metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COVERAGE] * 0.2) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_FUNCTIONAL] * 0.2) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COMPLEXITY] * 0.15) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COMPILER] * 0.15) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_STANDARD] * 0.1) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_DUPLICATION] * 0.1) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_FANOUT] * 0.05) +
+                (metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_SECURITY] * 0.05))
 
     def get_results(self, metrics):
         metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COMPLEXITY] = self.__getTiobeComplexity(metrics)
         metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_FANOUT] = self.__getTiobeFanout(metrics)
         metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COMPILER] = self.__getTiobeCompiler(metrics)
         metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_COVERAGE] = self.__getTiobeCoverage(metrics)
         metrics[MetricBaseCalcTIOBE.METRIC_TIOBE_DUPLICATION] = self.__getTiobeDuplication(metrics)
```

### Comparing `multimetric-1.4.1/multimetric/cls/importer/mods/json.py` & `multimetric-2.0.0/multimetric/cls/importer/mods/json.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 import json
-import sys
+import logging
 
 from multimetric.cls.importer.base import Importer
 
 
 class ImporterJSON(Importer):
 
     def __init__(self, args, filearg):
@@ -11,13 +13,12 @@
         self.__readInput()
 
     def __readInput(self):
         try:
             with open(self._input) as i:
                 reader = json.load(i)
                 for k, v in reader.items():
-                    _sev = None
-                    if "severity" in v:
-                        _sev = v["severity"]
-                    self._items.append(Importer.ImporterItem(_file=k, _cnt=v["content"], _sev=_sev))
+                    self._items.append(Importer.ImporterItem(_file=k,
+                                                             _sev=v["severity"],
+                                                             _cnt=v.get('content', None)))
         except Exception as e:
-            sys.stderr.write("Read error: {}\n".format(e))
+            logging.getLogger('stderr').error(f"Read error: {e}\n")
```

### Comparing `multimetric-1.4.1/multimetric/cls/metric/comments.py` & `multimetric-2.0.0/multimetric/cls/metric/comments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.base import MetricBase
 
 
 class MetricBaseComments(MetricBase):
     _needles = [
         "Token.Comment",
         "Token.Comment.Hashbang",
         "Token.Comment.Multiline",
         "Token.Comment.Single",
         "Token.Comment.Special",
-        "Token.Literal.String.Doc"
+        "Token.Literal.String.Doc",
     ]
 
     _specific = {
         "Python": [
-            "Token.Comment.Preproc"
-        ]
+            "Token.Comment.Preproc",
+        ],
     }
 
     METRIC_COMMENT_RATIO = "comment_ratio"
 
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
         self.__overall = 0
         self.__comments = 0
 
     def parse_tokens(self, language, tokens):
         super().parse_tokens(language, [])
         _n = MetricBaseComments._needles
         if language in MetricBaseComments._specific:
-            _n += MetricBaseComments._specific[language]
+            _n += MetricBaseComments._specific[language]  # pragma: no cover - bug in pytest-cov
         for x in tokens:
             self.__overall += len(str(x[1]))
             if str(x[0]) in _n:
-                self.__comments += len(str(x[1]))
+                self.__comments += len(str(x[1]))  # pragma: no cover - bug in pytest-cov
 
     def get_results(self):
-        if self.__overall == 0:
-            # sanity
-            self.__overall = 1
-        self._metrics[MetricBaseComments.METRIC_COMMENT_RATIO] = self.__comments * \
-            100.0 / float(self.__overall)
+        self.__overall = max(1, self.__overall)
+        self._metrics[MetricBaseComments.METRIC_COMMENT_RATIO] = (self.__comments *
+                                                                  100.0 / float(self.__overall))
         self._internalstore["comments"] = self.__comments
         self._internalstore["overall"] = self.__overall
         return self._metrics
 
     def get_results_global(self, value_stores):
         __comments = 0
         __overall = 0
         for x in self._get_all_matching_store_objects(value_stores):
             __comments += x["comments"]
             __overall += x["overall"]
         return {
-            MetricBaseComments.METRIC_COMMENT_RATIO: __comments * 100.0 / float(__overall or 1.0)
+            MetricBaseComments.METRIC_COMMENT_RATIO: __comments * 100.0 / float(__overall or 1.0),
         }
```

### Comparing `multimetric-1.4.1/multimetric/cls/metric/cyclomatic.py` & `multimetric-2.0.0/multimetric/cls/metric/cyclomatic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.base import MetricBase
 
 
 class MetricBaseCyclomaticComplexity(MetricBase):
 
     __exitPoints = [
         "return",
         "exit",
         "assert",
         "break",
         "continue",
-        "yield"
+        "yield",
     ]
 
     __conditions = [
         "if",
         "else",
         "elif",
         "case",
         "default",
         "for",
         "while",
         "and",
         "or",
         "&&",
-        "||"
+        "||",
     ]
 
     METRIC_CYCLOMATIC_COMPLEXITY = "cyclomatic_complexity"
 
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
         self._internalstore["exitpoints"] = 0
@@ -50,9 +52,9 @@
         __exitPoints = 0
         __conditions = 0
         for x in self._get_all_matching_store_objects(value_stores):
             __conditions += x["conditions"]
             __exitPoints += x["exitpoints"]
         return {
             MetricBaseCyclomaticComplexity.METRIC_CYCLOMATIC_COMPLEXITY: max(
-                __conditions - __exitPoints + 2, 0)
+                __conditions - __exitPoints + 2, 0),
         }
```

### Comparing `multimetric-1.4.1/multimetric/cls/metric/loc.py` & `multimetric-2.0.0/multimetric/cls/metric/loc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.base import MetricBase
 
 
 class MetricBaseLOC(MetricBase):
     METRIC_LOC = "loc"
 
     _needles = [
-        "Token.Text"
+        "Token.Text",
+        "Token.Comment.Preproc",
+        "Token.Text.Whitespace",
     ]
 
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
+        self._previous_token = (None, None)
 
     def parse_tokens(self, language, tokens):
         super().parse_tokens(language, [])
         self._metrics[MetricBaseLOC.METRIC_LOC] = 0
         for x in tokens:
-            if str(x[0]) in MetricBaseLOC._needles:
-                self._metrics[MetricBaseLOC.METRIC_LOC] += len([y for y in x[1] if y == '\n'])
+            if self._previous_token != x:
+                if x[1].strip(' ').endswith('\n'):
+                    self._metrics[MetricBaseLOC.METRIC_LOC] += 1
+            self._previous_token = x
+
         self._metrics[MetricBaseLOC.METRIC_LOC] = max(self._metrics[MetricBaseLOC.METRIC_LOC], 1)
         self._internalstore["loc"] = self._metrics[MetricBaseLOC.METRIC_LOC]
 
     def get_results_global(self, value_stores):
         _sum = sum([x["loc"] for x in self._get_all_matching_store_objects(value_stores)])
-        return { MetricBaseLOC.METRIC_LOC: _sum }
+        return {MetricBaseLOC.METRIC_LOC: _sum}
```

### Comparing `multimetric-1.4.1/multimetric/cls/metric/operands.py` & `multimetric-2.0.0/multimetric/cls/metric/operands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.base import MetricBase
 
 
 class MetricBaseOperands(MetricBase):
     _needles = [
         "Token.Literal.Date",
         "Token.Literal.String.Double",
@@ -35,15 +37,15 @@
         "Token.String.Double",
         "Token.String.Escape",
         "Token.String.Heredoc",
         "Token.String.Interpol",
         "Token.String.Other",
         "Token.String.Regex",
         "Token.String.Single",
-        "Token.String.Symbol"
+        "Token.String.Symbol",
     ]
 
     METRIC_OPERANDS_SUM = "operands_sum"
     METRIC_OPERANDS_UNIQUE = "operands_uniq"
 
     def __init__(self, args, **kwargs):
         super().__init__(args, **kwargs)
@@ -64,9 +66,9 @@
 
     def get_results_global(self, value_stores):
         _operands = []
         for x in self._get_all_matching_store_objects(value_stores):
             _operands += x["operands"]
         return {
             MetricBaseOperands.METRIC_OPERANDS_SUM: len(_operands),
-            MetricBaseOperands.METRIC_OPERANDS_UNIQUE: len(list(set(_operands)))
+            MetricBaseOperands.METRIC_OPERANDS_UNIQUE: len(list(set(_operands))),
         }
```

### Comparing `multimetric-1.4.1/multimetric/cls/metric/operators.py` & `multimetric-2.0.0/multimetric/cls/metric/operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.base import MetricBase
 
 
 class MetricBaseOperator(MetricBase):
     _needles = [
         "Token.Name.Class",
         "Token.Name.Decorator",
@@ -39,9 +41,9 @@
 
     def get_results_global(self, value_stores):
         _operator = []
         for x in self._get_all_matching_store_objects(value_stores):
             _operator += x["operator"]
         return {
             MetricBaseOperator.METRIC_OPERATORS_SUM: len(_operator),
-            MetricBaseOperator.METRIC_OPERATORS_UNIQUE: len(list(set(_operator)))
+            MetricBaseOperator.METRIC_OPERATORS_UNIQUE: len(list(set(_operator))),
         }
```

### Comparing `multimetric-1.4.1/multimetric/cls/modules.py` & `multimetric-2.0.0/multimetric/cls/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 from multimetric.cls.calc.halstead import MetricBaseCalcHalstead
 from multimetric.cls.calc.maintenance import MetricBaseCalcMaintenanceIndex
 from multimetric.cls.calc.pylint import MetricBaseCalcPylint
 from multimetric.cls.calc.tiobe import MetricBaseCalcTIOBE
 from multimetric.cls.metric.comments import MetricBaseComments
 from multimetric.cls.metric.cyclomatic import MetricBaseCyclomaticComplexity
 from multimetric.cls.metric.fanout import MetricBaseFanout
@@ -23,21 +25,21 @@
 
 
 def get_modules_calculated(args, **kwargs):
     return [
         MetricBaseCalcHalstead(args, **kwargs),
         MetricBaseCalcMaintenanceIndex(args, **kwargs),
         MetricBaseCalcTIOBE(args, **kwargs),
-        MetricBaseCalcPylint(args, **kwargs)
+        MetricBaseCalcPylint(args, **kwargs),
     ]
 
 
 def get_modules_stats(args, **kwargs):
     return [
-        MetricBaseStatsAverage(args, **kwargs)
+        MetricBaseStatsAverage(args, **kwargs),
     ]
 
 
 def get_additional_parser_args(parser):
     parser.add_argument("--bugpredict",
                         choices=MetricBaseCalcHalstead.BUGPRED_METHOD.keys(),
                         default=MetricBaseCalcHalstead.BUGPRED_DEFAULT,
```

### Comparing `multimetric-1.4.1/multimetric/cls/stats/stats.py` & `multimetric-2.0.0/multimetric/cls/stats/stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
 import statistics
 
 from multimetric.cls.base_stats import MetricBaseStats
 
 
 class MetricBaseStatsAverage(MetricBaseStats):
```

### Comparing `multimetric-1.4.1/multimetric.egg-info/PKG-INFO` & `multimetric-2.0.0/multimetric.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 1.4.1
+Version: 2.0.0
 Summary: Calculate code metrics in various languages
-Home-page: https://github.com/startupos/multimetric
-Author: Jason Nichols
-Author-email: jn@ayl.us
+Home-page: https://github.com/priv-kweihmann/multimetric
+Author: Konrad Weihmann
+Author-email: kweihmann@outlook.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Python: >=3.10
 Description-Content-Type: text/plain
-License-File: LICENSE
+License-File: LICENSE.Zlib
+
+See https://github.com/priv-kweihmann/multimetric for documentation
 
-See https://github.com/startupos/multimetric for documentation
```

### Comparing `multimetric-1.4.1/setup.py` & `multimetric-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-import subprocess
+# SPDX-FileCopyrightText: 2023 Konrad Weihmann
+# SPDX-License-Identifier: Zlib
+import subprocess  # noqa: S404
+
 import setuptools
 
-_long_description = "See https://github.com/startupos/multimetric for documentation"
+_long_description = "See https://github.com/priv-kweihmann/multimetric for documentation"
 _long_description_content_type = "text/plain"
 try:
-    _long_description = subprocess.check_output(
+    _long_description = subprocess.check_output(  # noqa: S607 S603
         ["pandoc", "--from", "markdown", "--to", "rst", "README.md"]).decode("utf-8")
     _long_description_content_type = "text/x-rst"
 except (subprocess.CalledProcessError, FileNotFoundError):
     pass
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="multimetric",
-    version="1.4.1",
-    author="Jason Nichols",
-    author_email="jn@ayl.us",
+    version="2.0.0",
+    author="Konrad Weihmann",
+    author_email="kweihmann@outlook.com",
     description="Calculate code metrics in various languages",
     long_description=_long_description,
     long_description_content_type=_long_description_content_type,
-    url="https://github.com/startupos/multimetric",
-    packages=setuptools.find_packages(),
+    url="https://github.com/priv-kweihmann/multimetric",
+    packages=setuptools.find_packages(exclude='tests'),
     install_requires=requirements,
         entry_points={
         "console_scripts": [
             "multimetric = multimetric.__main__:main",
-        ]
+        ],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
+        "License :: OSI Approved :: zlib/libpng License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Quality Assurance",
     ],
+    python_requires='>=3.10',
 )
```

