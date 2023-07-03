# Comparing `tmp/nomenklatura-3.0.3.tar.gz` & `tmp/nomenklatura-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.0.3.tar", last modified: Thu Jun 29 07:34:13 2023, max compression
+gzip compressed data, was "nomenklatura-3.1.0.tar", last modified: Mon Jul  3 09:52:57 2023, max compression
```

## Comparing `nomenklatura-3.0.3.tar` & `nomenklatura-3.1.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.386916 nomenklatura-3.0.3/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.386916 nomenklatura-3.0.3/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:33:48.000000 nomenklatura-3.0.3/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:52:30.000000 nomenklatura-3.1.0/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/setup.py
```

### Comparing `nomenklatura-3.0.3/LICENSE` & `nomenklatura-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/PKG-INFO` & `nomenklatura-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.0.3
+Version: 3.1.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -92,9 +91,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-3.0.3/README.md` & `nomenklatura-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/cache.py` & `nomenklatura-3.1.0/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/cli.py` & `nomenklatura-3.1.0/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.1.0/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.1.0/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/dataset/catalog.py` & `nomenklatura-3.1.0/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/dataset/coverage.py` & `nomenklatura-3.1.0/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/dataset/dataset.py` & `nomenklatura-3.1.0/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/dataset/publisher.py` & `nomenklatura-3.1.0/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/dataset/resource.py` & `nomenklatura-3.1.0/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/dataset/util.py` & `nomenklatura-3.1.0/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/db.py` & `nomenklatura-3.1.0/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/__init__.py` & `nomenklatura-3.1.0/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/aleph.py` & `nomenklatura-3.1.0/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/common.py` & `nomenklatura-3.1.0/nomenklatura/enrich/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
 import json
+import logging
 from banal import as_bool
 from typing import Union, Any, Dict, Optional, Generator
 from abc import ABC, abstractmethod
 from requests import Session
 from requests.exceptions import RequestException, HTTPError
 from followthemoney import model
 
 from nomenklatura import __version__
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.util import ParamsType, normalize_url
 
 EnricherConfig = Dict[str, Any]
+log = logging.getLogger(__name__)
 
 
 class EnrichmentException(Exception):
     pass
 
 
 class EnrichmentAbort(Exception):
@@ -110,24 +112,33 @@
                     raise EnrichmentAbort("Authorization failure: %s" % url) from rex
                 msg = "HTTP POST failed [%s]: %s" % (url, rex)
                 raise EnrichmentException(msg) from rex
             resp_data = resp.json()
             self.cache.set_json(cache_key, resp_data)
         return resp_data
 
+    def _make_data_entity(
+        self, entity: CE, data: Dict[str, Any], cleaned: bool = True
+    ) -> CE:
+        return type(entity).from_dict(
+            model,
+            data,
+            default_dataset=self.dataset.name,
+            cleaned=cleaned,
+        )
+
     def load_entity(self, entity: CE, data: Dict[str, Any]) -> CE:
-        proxy = type(entity).from_dict(model, data, cleaned=False)
+        proxy = self._make_data_entity(entity, data, cleaned=False)
         for prop in proxy.iterprops():
             if prop.stub:
                 proxy.pop(prop)
         return proxy
 
     def make_entity(self, entity: CE, schema: str) -> CE:
-        data = {"schema": schema}
-        return type(entity).from_dict(model, data)
+        return self._make_data_entity(entity, {"schema": schema})
 
     def match_wrapped(self, entity: CE) -> Generator[CE, None, None]:
         if len(self.schemata) and entity.schema.name not in self.schemata:
             return
         yield from self.match(entity)
 
     def expand_wrapped(self, entity: CE, match: CE) -> Generator[CE, None, None]:
```

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.1.0/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.1.0/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,20 @@
             return
 
         for name in entity.get("name", quiet=True):
             params = {
                 "format": "json",
                 "search": name,
                 "action": "wbsearchentities",
-                "language": "de",
+                "language": "en",
+                "strictlanguage": "false",
             }
-            data = self.http_get_json_cached(WD_API, params=params)
+            data = self.http_get_json_cached(
+                WD_API, params=params, cache_days=self.cache_days
+            )
             if "search" not in data:
                 self.http_remove_cache(WD_API, params=params)
                 log.warning("Search response [%s] does not include results" % name)
                 continue
             for result in data["search"]:
                 item = self.fetch_item(result["id"])
                 if item is not None:
@@ -98,17 +101,16 @@
     ) -> Dict[str, Any]:
         # https://www.mediawiki.org/wiki/Wikibase/API
         # https://www.wikidata.org/w/api.php?action=help&modules=wbgetentities
         params = {**kwargs, "format": "json", "ids": id, "action": "wbgetentities"}
         data = self.http_get_json_cached(WD_API, params=params, cache_days=cache_days)
         return cast(Dict[str, Any], data)
 
-    def fetch_item(self, qid: str, cache_days: Optional[int] = None) -> Optional[Item]:
-        cache_days = self.cache_days if cache_days is None else cache_days
-        data = self.wikibase_getentities(qid, cache_days=cache_days)
+    def fetch_item(self, qid: str) -> Optional[Item]:
+        data = self.wikibase_getentities(qid, cache_days=self.cache_days)
         entity = data.get("entities", {}).get(qid)
         if entity is None:
             return None
         return Item(entity)
 
     @cache
     def get_label(self, qid: str) -> LangText:
```

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/enrich/yente.py` & `nomenklatura-3.1.0/nomenklatura/enrich/yente.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         api_key: Optional[str] = os.path.expandvars(config.pop("api_key", "")).strip()
         if api_key is None or not len(api_key):
             api_key = os.environ.get("YENTE_API_KEY")
         self._api_key: Optional[str] = api_key
         if self._api_key is not None:
             self.session.headers["Authorization"] = f"ApiKey {self._api_key}"
 
-        # match_url = urljoin(self._api, f"match/{self._dataset}")
-        # self.cache.preload(f"{match_url}%")
+        match_url = urljoin(self._api, f"match/{self._dataset}")
+        self.cache.preload(f"{match_url}%")
 
     def make_url(self, entity: CE) -> str:
         return urljoin(self._api, f"entities/{entity.id}")
 
     def match(self, entity: CE) -> Generator[CE, None, None]:
         if not entity.schema.matchable:
             return
@@ -62,15 +62,20 @@
                     "schema": entity.schema.name,
                     "properties": props,
                 }
             }
         }
         for retry in range(4):
             try:
-                response = self.http_post_json_cached(url, cache_key, query)
+                response = self.http_post_json_cached(
+                    url,
+                    cache_key,
+                    query,
+                    cache_days=self.cache_days,
+                )
             except EnrichmentException as exc:
                 log.info("Error matching %r: %s", entity, exc)
                 if retry == 3:
                     raise
                 time.sleep((retry + 1) ** 2)
 
         inner_resp = response.get("responses", {}).get("entity", {})
@@ -101,9 +106,9 @@
 
     def expand(self, entity: CE, match: CE) -> Generator[CE, None, None]:
         url = self.make_url(match)
         for source_url in match.get("sourceUrl", quiet=True):
             if source_url.startswith(self._api):
                 url = source_url
         url = normalize_url(url, {"nested": self._nested})
-        response = self.http_get_json_cached(url)
+        response = self.http_get_json_cached(url, cache_days=self.cache_days)
         yield from self._traverse_nested(match, response)
```

### Comparing `nomenklatura-3.0.3/nomenklatura/entity.py` & `nomenklatura-3.1.0/nomenklatura/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     @property
     def _properties(self) -> Dict[str, List[str]]:  # type: ignore
         return {p: [s.value for s in v] for p, v in self._statements.items()}
 
     def _iter_stmt(self) -> Generator[Statement, None, None]:
         for stmts in self._statements.values():
             for stmt in stmts:
+                if stmt.entity_id is None and self.id is not None:
+                    stmt.entity_id = self.id
+                    stmt.id = stmt.generate_key()
                 if stmt.id is None and stmt.entity_id is not None:
                     stmt.id = stmt.generate_key()
                 yield stmt
 
     def checksum(self) -> str:
         hash = sha1(self.schema.name.encode("utf-8"))
         for stmt in sorted(self._iter_stmt()):
@@ -388,26 +391,29 @@
         return {p: list({s.value for s in vs}) for p, vs in self._statements.items()}
 
     def iterprops(self) -> List[Property]:
         return [self.schema.properties[p] for p in self._statements.keys()]
 
     def clone(self: CE) -> CE:
         data = {"schema": self.schema.name, "id": self.id}
-        cloned = type(self).from_dict(self.schema.model, data)
+        cloned = type(self).from_dict(
+            self.schema.model,
+            data,
+            default_dataset=self.default_dataset,
+        )
         for stmt in self._iter_stmt():
             cloned.add_statement(stmt)
         return cloned
 
     def merge(self: CE, other: "CompositeEntity") -> CE:
         for stmt in other._iter_stmt():
             if self.id is not None:
                 stmt.canonical_id = self.id
             self.add_statement(stmt)
-        self.referents.update(other.referents)
-        self.datasets.update(other.datasets)
+        self.extra_referents.update(other.extra_referents)
         return self
 
     def to_dict(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {
             "id": self.id,
             "caption": self.caption,
             "schema": self.schema.name,
```

### Comparing `nomenklatura-3.0.3/nomenklatura/index/entry.py` & `nomenklatura-3.1.0/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/index/index.py` & `nomenklatura-3.1.0/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/index/tokenizer.py` & `nomenklatura-3.1.0/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/judgement.py` & `nomenklatura-3.1.0/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/__init__.py` & `nomenklatura-3.1.0/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.1.0/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.1.0/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/pairs.py` & `nomenklatura-3.1.0/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/types.py` & `nomenklatura-3.1.0/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/util.py` & `nomenklatura-3.1.0/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.1.0/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.1.0/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v1/model.py` & `nomenklatura-3.1.0/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v1/names.py` & `nomenklatura-3.1.0/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v1/train.py` & `nomenklatura-3.1.0/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v1/util.py` & `nomenklatura-3.1.0/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.1.0/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.1.0/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v2/model.py` & `nomenklatura-3.1.0/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v2/names.py` & `nomenklatura-3.1.0/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v2/train.py` & `nomenklatura-3.1.0/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/matching/v2/util.py` & `nomenklatura-3.1.0/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/publish/dates.py` & `nomenklatura-3.1.0/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/publish/edges.py` & `nomenklatura-3.1.0/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/publish/names.py` & `nomenklatura-3.1.0/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/resolver/edge.py` & `nomenklatura-3.1.0/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/resolver/identifier.py` & `nomenklatura-3.1.0/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/resolver/resolver.py` & `nomenklatura-3.1.0/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/senzing.py` & `nomenklatura-3.1.0/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/statement/serialize.py` & `nomenklatura-3.1.0/nomenklatura/statement/serialize.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import csv
 import _csv
 import click
 import orjson
 from pathlib import Path
 from io import TextIOWrapper
-from typing import BinaryIO, TextIO, Generator, Iterable, Type, Dict, Any, List
+from types import TracebackType
+from typing import Optional, Dict, Any, List
+from typing import BinaryIO, TextIO, Generator, Iterable, Type
 from followthemoney.cli.util import MAX_LINE
 
 from nomenklatura.statement.statement import S
 from nomenklatura.util import pack_prop, unpack_prop
 
 JSON = "json"
 CSV = "csv"
@@ -101,71 +103,122 @@
         fh = click.get_binary_stream("stdin")
         yield from read_statements(fh, format=format, statement_type=statement_type)
         return
     with open(path, "rb") as fh:
         yield from read_statements(fh, format=format, statement_type=statement_type)
 
 
-def write_json_statement(fh: BinaryIO, statement: S) -> None:
-    data = statement.to_dict()
-    out = orjson.dumps(data, option=orjson.OPT_APPEND_NEWLINE)
-    fh.write(out)
-
-
-def write_json_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
-    for stmt in statements:
-        write_json_statement(fh, stmt)
-
-
-def write_csv_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
-    with TextIOWrapper(fh, encoding="utf-8") as wrapped:
-        writer = csv.writer(wrapped, dialect=csv.unix_dialect)
-        writer.writerow(CSV_COLUMNS)
-        for stmt in statements:
-            row = stmt.to_row()
-            writer.writerow([row.get(c) for c in CSV_COLUMNS])
+# def write_json_statement(fh: BinaryIO, statement: S) -> None:
+#     data = statement.to_dict()
+#     out = orjson.dumps(data, option=orjson.OPT_APPEND_NEWLINE)
+#     fh.write(out)
+
+
+# def write_json_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
+#     for stmt in statements:
+#         write_json_statement(fh, stmt)
+
+
+# def write_csv_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
+#     with TextIOWrapper(fh, encoding="utf-8") as wrapped:
+#         writer = csv.writer(wrapped, dialect=csv.unix_dialect)
+#         writer.writerow(CSV_COLUMNS)
+#         for stmt in statements:
+#             row = stmt.to_row()
+#             writer.writerow([row.get(c) for c in CSV_COLUMNS])
 
 
 def pack_statement(stmt: S) -> Dict[str, Any]:
     row = stmt.to_row()
     row.pop("canonical_id", None)
     row.pop("prop_type", None)
     prop = row.pop("prop")
     schema = row.pop("schema")
     if prop is None or schema is None:
         raise ValueError("Cannot pack statement without prop and schema")
     row["prop"] = pack_prop(schema, prop)
     return row
 
 
-def pack_row(stmt: S) -> List[Any]:
-    row = stmt.to_row()
-    prop = row.pop("prop")
-    schema = row.pop("schema")
-    if prop is None or schema is None:
-        raise ValueError("Cannot pack statement without prop and schema")
-    row["prop"] = pack_prop(schema, prop)
-    return [row.get(c) for c in PACK_COLUMNS]
+def get_statement_writer(fh: BinaryIO, format: str) -> "StatementWriter":
+    if format == CSV:
+        return CSVStatementWriter(fh)
+    elif format == PACK:
+        return PackStatementWriter(fh)
+    elif format == JSON:
+        return JSONStatementWriter(fh)
+    raise RuntimeError("Unknown statement format: %s" % format)
 
 
-def pack_writer(fh: TextIO) -> "_csv._writer":
-    return csv.writer(
-        fh,
-        dialect=csv.unix_dialect,
-        quoting=csv.QUOTE_MINIMAL,
-    )
-
-
-def write_pack_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
-    with TextIOWrapper(fh, encoding="utf-8") as wrapped:
-        writer = pack_writer(wrapped)
-        for stmt in statements:
-            writer.writerow(pack_row(stmt))
+def write_statements(fh: BinaryIO, format: str, statements: Iterable[S]) -> None:
+    writer = get_statement_writer(fh, format)
+    for stmt in statements:
+        writer.write(stmt)
 
 
-def write_statements(fh: BinaryIO, format: str, statements: Iterable[S]) -> None:
-    if format == CSV:
-        write_csv_statements(fh, statements)
-    elif format == PACK:
-        write_pack_statements(fh, statements)
-    else:
-        write_json_statements(fh, statements)
+class StatementWriter(object):
+    def __init__(self, fh: BinaryIO) -> None:
+        self.fh = fh
+
+    def write(self, stmt: S) -> None:
+        raise NotImplementedError()
+
+    def close(self) -> None:
+        self.fh.close()
+
+    def __enter__(self) -> "StatementWriter":
+        return self
+
+    def __exit__(
+        self,
+        type: Optional[Type[BaseException]],
+        value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        self.close()
+
+
+class JSONStatementWriter(StatementWriter):
+    def write(self, stmt: S) -> None:
+        data = stmt.to_dict()
+        out = orjson.dumps(data, option=orjson.OPT_APPEND_NEWLINE)
+        self.fh.write(out)
+
+
+class CSVStatementWriter(StatementWriter):
+    def __init__(self, fh: BinaryIO) -> None:
+        super().__init__(fh)
+        self.wrapper = TextIOWrapper(fh, encoding="utf-8")
+        self.writer = csv.writer(self.wrapper, dialect=csv.unix_dialect)
+        self.writer.writerow(CSV_COLUMNS)
+
+    def write(self, stmt: S) -> None:
+        row = stmt.to_row()
+        self.writer.writerow([row.get(c) for c in CSV_COLUMNS])
+
+    def close(self) -> None:
+        self.wrapper.close()
+        super().close()
+
+
+class PackStatementWriter(StatementWriter):
+    def __init__(self, fh: BinaryIO) -> None:
+        super().__init__(fh)
+        self.wrapper = TextIOWrapper(fh, encoding="utf-8")
+        self.writer = csv.writer(
+            self.wrapper,
+            dialect=csv.unix_dialect,
+            quoting=csv.QUOTE_MINIMAL,
+        )
+
+    def write(self, stmt: S) -> None:
+        row = stmt.to_row()
+        prop = row.pop("prop")
+        schema = row.pop("schema")
+        if prop is None or schema is None:
+            raise ValueError("Cannot pack statement without prop and schema")
+        row["prop"] = pack_prop(schema, prop)
+        self.writer.writerow([row.get(c) for c in PACK_COLUMNS])
+
+    def close(self) -> None:
+        self.wrapper.close()
+        super().close()
```

### Comparing `nomenklatura-3.0.3/nomenklatura/statement/statement.py` & `nomenklatura-3.1.0/nomenklatura/statement/statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         dataset: str,
         entity_id: Optional[str],
         prop: str,
         value: str,
         external: Optional[bool],
     ) -> Optional[str]:
         """Hash the key properties of a statement record to make a unique ID."""
-        if entity_id is None:
+        if entity_id is None or prop is None:
             return None
         key = f"{dataset}.{entity_id}.{prop}.{value}"
         if external:
             # We consider the external flag in key composition to avoid race conditions where
             # a certain entity might be emitted as external while it is already linked in to
             # the graph via another route.
             key = f"{key}.ext"
```

### Comparing `nomenklatura-3.0.3/nomenklatura/store/__init__.py` & `nomenklatura-3.1.0/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/store/base.py` & `nomenklatura-3.1.0/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/store/level.py` & `nomenklatura-3.1.0/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/store/memory.py` & `nomenklatura-3.1.0/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/store/util.py` & `nomenklatura-3.1.0/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/tui/app.py` & `nomenklatura-3.1.0/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/tui/comparison.py` & `nomenklatura-3.1.0/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/tui/util.py` & `nomenklatura-3.1.0/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/util.py` & `nomenklatura-3.1.0/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura/xref.py` & `nomenklatura-3.1.0/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.1.0/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.0.3
+Version: 3.1.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -92,9 +91,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-3.0.3/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.1.0/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.3/setup.py` & `nomenklatura-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.0.3",
+    version="3.1.0",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

