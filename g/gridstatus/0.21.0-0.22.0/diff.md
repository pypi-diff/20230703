# Comparing `tmp/gridstatus-0.21.0.tar.gz` & `tmp/gridstatus-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-g5585lv9/gridstatus-0.21.0.tar", last modified: Tue May 23 00:38:18 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-7wsb32ge/gridstatus-0.22.0.tar", last modified: Mon Jul  3 14:58:33 2023, max compression
```

## Comparing `gridstatus-0.21.0.tar` & `gridstatus-0.22.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-23 00:38:04.000000 gridstatus-0.21.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4497 2023-05-23 00:38:18.000000 gridstatus-0.21.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2049 2023-05-23 00:38:04.000000 gridstatus-0.21.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/docs/
--rw-r--r--   0 root         (0) root         (0)     4290 2023-05-23 00:38:04.000000 gridstatus-0.21.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-23 00:38:04.000000 gridstatus-0.21.0/docs/update_docs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus/
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3743 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/base.py
--rw-r--r--   0 root         (0) root         (0)    45618 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/caiso.py
--rw-r--r--   0 root         (0) root         (0)    12502 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/decorators.py
--rw-r--r--   0 root         (0) root         (0)     5567 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/eia.py
--rw-r--r--   0 root         (0) root         (0)    35728 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/ercot.py
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/gs_logging.py
--rw-r--r--   0 root         (0) root         (0)    23024 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/isone.py
--rw-r--r--   0 root         (0) root         (0)     4983 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/lmp_config.py
--rw-r--r--   0 root         (0) root         (0)    11050 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/miso.py
--rw-r--r--   0 root         (0) root         (0)    26181 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/nyiso.py
--rw-r--r--   0 root         (0) root         (0)    21566 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/pjm.py
--rw-r--r--   0 root         (0) root         (0)    33028 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/spp.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12735 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/base_test_iso.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/decorators.py
--rw-r--r--   0 root         (0) root         (0)     9418 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_caiso.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_eia.py
--rw-r--r--   0 root         (0) root         (0)     9292 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_ercot.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_gridstatus.py
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_interconnection_queue.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_isone.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_lmp_config.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2813 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_miso.py
--rw-r--r--   0 root         (0) root         (0)     7599 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_nyiso.py
--rw-r--r--   0 root         (0) root         (0)    11196 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_pjm.py
--rw-r--r--   0 root         (0) root         (0)     1079 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_save_to.py
--rw-r--r--   0 root         (0) root         (0)    11968 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_spp.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)       92 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_version.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_viz.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/version.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4497 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1246 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      590 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3091 2023-05-23 00:38:04.000000 gridstatus-0.21.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 00:38:18.000000 gridstatus-0.21.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/utils/ercot/
--rw-r--r--   0 root         (0) root         (0)     2481 2023-05-23 00:38:04.000000 gridstatus-0.21.0/utils/ercot/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-03 14:58:16.000000 gridstatus-0.22.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-07-03 14:58:33.000000 gridstatus-0.22.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-03 14:58:16.000000 gridstatus-0.22.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-07-03 14:58:16.000000 gridstatus-0.22.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-03 14:58:16.000000 gridstatus-0.22.0/docs/update_docs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus/
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/base.py
+-rw-r--r--   0 root         (0) root         (0)    45271 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/caiso.py
+-rw-r--r--   0 root         (0) root         (0)    12471 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     6709 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/eia.py
+-rw-r--r--   0 root         (0) root         (0)    53342 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/ercot.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/gs_logging.py
+-rw-r--r--   0 root         (0) root         (0)    23025 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/isone.py
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/lmp_config.py
+-rw-r--r--   0 root         (0) root         (0)    11039 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/miso.py
+-rw-r--r--   0 root         (0) root         (0)    29103 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/nyiso.py
+-rw-r--r--   0 root         (0) root         (0)    21550 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/pjm.py
+-rw-r--r--   0 root         (0) root         (0)    33042 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/spp.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12669 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/base_test_iso.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     9418 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_caiso.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_eia.py
+-rw-r--r--   0 root         (0) root         (0)    19597 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_ercot.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_gridstatus.py
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_interconnection_queue.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_isone.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_lmp_config.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_miso.py
+-rw-r--r--   0 root         (0) root         (0)     9479 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_nyiso.py
+-rw-r--r--   0 root         (0) root         (0)    11196 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_pjm.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_save_to.py
+-rw-r--r--   0 root         (0) root         (0)    11968 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_spp.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)       92 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/tests/test_viz.py
+-rw-r--r--   0 root         (0) root         (0)     8739 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/version.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-07-03 14:58:16.000000 gridstatus-0.22.0/gridstatus/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-03 14:58:33.000000 gridstatus-0.22.0/gridstatus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3091 2023-07-03 14:58:16.000000 gridstatus-0.22.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 14:58:33.000000 gridstatus-0.22.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 14:58:33.000000 gridstatus-0.22.0/utils/ercot/
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-07-03 14:58:16.000000 gridstatus-0.22.0/utils/ercot/README.md
```

### Comparing `gridstatus-0.21.0/LICENSE` & `gridstatus-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/PKG-INFO` & `gridstatus-0.22.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatus
-Version: 0.21.0
+Version: 0.22.0
 Summary: API to access energy data
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gridstatus Version: 0.21.0 Summary: API to access
+Metadata-Version: 2.1 Name: gridstatus Version: 0.22.0 Summary: API to access
 energy data Author-email: Max Kanter
 gmail.com> Maintainer-email: Max Kanter
 gmail.com> License: Copyright 2022 James Max Kanter Redistribution and use in
 source and binary forms, with or without modification, are permitted provided
 that the following conditions are met: 1. Redistributions of source code must
 retain the above copyright notice, this list of conditions and the following
 disclaimer. 2. Redistributions in binary form must reproduce the above
```

### Comparing `gridstatus-0.21.0/README.md` & `gridstatus-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/docs/conf.py` & `gridstatus-0.22.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/docs/update_docs.py` & `gridstatus-0.22.0/docs/update_docs.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/__init__.py` & `gridstatus-0.22.0/gridstatus/__init__.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/base.py` & `gridstatus-0.22.0/gridstatus/base.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/caiso.py` & `gridstatus-0.22.0/gridstatus/caiso.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,25 +151,15 @@
         return df
 
     @support_date_range(frequency="DAY_START")
     def get_load(self, date, end=None, verbose=False):
         """Return load at a previous date in 5 minute intervals"""
 
         if date == "latest":
-            # todo call today
-            load_url = _BASE + "/demand.csv"
-            df = pd.read_csv(load_url)
-
-            # get last non null row
-            data = df[~df["Current demand"].isnull()].iloc[-1]
-
-            return {
-                "time": _make_timestamp(data["Time"], self._current_day()),
-                "load": data["Current demand"],
-            }
+            return self.get_load("today", verbose=verbose)
 
         return self._get_historical_load(date, verbose=verbose)
 
     def _get_historical_load(self, date, verbose=False):
         df = _get_historical("demand", date, verbose=verbose)
 
         df = df[["Time", "Interval Start", "Interval End", "Current demand"]]
@@ -653,15 +643,16 @@
 
             verbose: print out url being fetched. Defaults to False.
 
         Returns:
             pandas.DataFrame: A DataFrame of curtailment data
         """
 
-        # http://www.caiso.com/Documents/Wind_SolarReal-TimeDispatchCurtailmentReport02dec_2020.pdf
+        # round to beginning of day
+        date = date.normalize()
 
         date_strs = [
             date.strftime("%b%d_%Y"),
             date.strftime(
                 "%d%b_%Y",
             ).lower(),
             date.strftime("-%b%d_%Y"),
```

### Comparing `gridstatus-0.21.0/gridstatus/decorators.py` & `gridstatus-0.22.0/gridstatus/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,17 @@
                 if (
                     next_day_start < args_dict["end"]
                     and next_day_start != args_dict["date"]
                 ):
                     prepend = [args_dict["date"]]
                     args_dict["date"] = args_dict["date"].ceil("1D")
             elif frequency == "MONTH_START":
-                frequency = "1M"
-                next_month_start = (
-                    args_dict["date"] + pd.offsets.MonthBegin(1)
-                ).normalize()
+                frequency = pd.offsets.MonthBegin(1)
+                next_month_start = (args_dict["date"] + frequency).normalize()
+
                 if (
                     next_month_start < args_dict["end"]
                     and next_month_start != args_dict["date"]
                 ):
                     prepend = [args_dict["date"]]
                     args_dict["date"] = next_month_start
 
@@ -148,14 +147,15 @@
             dates = [
                 gridstatus.utils._handle_date(
                     d,
                     args_dict["self"].default_timezone,
                 )
                 for d in dates
             ]
+
             # sometime api have restrictions/optimizations based on date ranges
             # update_dates allows for the caller to insert this logic
             if self.update_dates is not None:
                 dates = self.update_dates(dates, args_dict)
 
             start_date = dates[0]
```

### Comparing `gridstatus-0.21.0/gridstatus/eia.py` & `gridstatus-0.22.0/gridstatus/eia.py`

 * *Files 26% similar despite different names*

```diff
@@ -146,18 +146,65 @@
 
         if dataset in DATASET_HANDLERS:
             df = DATASET_HANDLERS[dataset](df)
 
         return df
 
 
+def _handle_time(df, frequency="1h"):
+    df.insert(0, "Interval End", pd.to_datetime(df["period"], utc=True))
+    df.insert(0, "Interval Start", df["Interval End"] - pd.Timedelta(frequency))
+    df = df.drop("period", axis=1)
+    return df
+
+
+def _handle_region_data(df):
+    df = _handle_time(df, frequency="1h")
+
+    df = df.rename(
+        {
+            "value": "MW",
+            "respondent": "Respondent",
+            "respondent-name": "Respondent Name",
+            "type": "Type",
+        },
+        axis=1,
+    )
+
+    # ['TI', 'NG', 'DF', 'D']
+    df["Type"] = df["Type"].map(
+        {
+            "D": "Load",
+            "TI": "Total Interchange",
+            "NG": "Net Generation",
+            "DF": "Load Forecast",
+        },
+    )
+
+    df["MW"] = df["MW"].astype("Int64")
+
+    # pivot on type
+    df = df.pivot_table(
+        index=["Interval Start", "Interval End", "Respondent", "Respondent Name"],
+        columns="Type",
+        values="MW",
+    ).reset_index()
+
+    df.columns.name = None
+
+    # fix after pivot
+    for col in ["Load", "Net Generation", "Load Forecast", "Total Interchange"]:
+        df[col] = df[col].astype("Int64")
+
+    return df
+
+
 def _handle_rto_interchange(df):
     """electricity/rto/interchange-data"""
-    df["Interval End"] = pd.to_datetime(df["period"], utc=True)
-    df["Interval Start"] = df["Interval End"] - pd.Timedelta("1h")
+    df = _handle_time(df, frequency="1h")
     df = df.rename(
         {
             "value": "MW",
             "fromba": "From BA",
             "toba": "To BA",
             "fromba-name": "From BA Name",
             "toba-name": "To BA Name",
@@ -179,11 +226,12 @@
     df = df.sort_values(["Interval Start", "From BA"])
 
     return df
 
 
 DATASET_HANDLERS = {
     "electricity/rto/interchange-data": _handle_rto_interchange,
+    "electricity/rto/region-data": _handle_region_data,
 }
 
 # docs
 # https://www.eia.gov/opendata/documentation.php
```

### Comparing `gridstatus-0.21.0/gridstatus/ercot.py` & `gridstatus-0.22.0/gridstatus/ercot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import io
 from dataclasses import dataclass
 from zipfile import ZipFile
 
 import pandas as pd
 import requests
 import tqdm
+from bs4 import BeautifulSoup
 
 from gridstatus import utils
 from gridstatus.base import (
     GridStatus,
     InterconnectionQueueStatus,
     ISOBase,
     Markets,
@@ -53,18 +54,42 @@
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP6-905-CD
 SETTLEMENT_POINT_PRICES_AT_RESOURCE_NODES_HUBS_AND_LOAD_ZONES_RTID = 12301
 
 # Seven-Day Load Forecast by Forecast Zone
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP3-560-CD
 SEVEN_DAY_LOAD_FORECAST_BY_FORECAST_ZONE_RTID = 12311
 
+# Actual System Load by Weather Zone
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP6-345-CD
+ACTUAL_SYSTEM_LOAD_BY_WEATHER_ZONE = 13101
+
+# Actual System Load by Forecast Zone
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP6-346-CD
+ACTUAL_SYSTEM_LOAD_BY_FORECAST_ZONE = 14836
+
 # Historical DAM Clearing Prices for Capacity
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP4-181-ER
 HISTORICAL_DAM_CLEARING_PRICES_FOR_CAPACITY_RTID = 13091
 
+# Unplanned Resource Outages Report
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP1-346-ER
+UNPLANNED_RESOURCE_OUTAGES_REPORT_RTID = 22912
+
+# 3-Day Highest Price AS Offer Selected
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP3-915-EX
+THREE_DAY_HIGHEST_PRICE_AS_OFFER_SELECTED_RTID = 13018
+
+# 2-Day Ancillary Services Reports
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP3-911-ER
+TWO_DAY_ANCILLARY_SERVICES_REPORTS_RTID = 13057
+
+# Hourly Resource Outage Capacity
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP3-233-CD
+HOURLY_RESOURCE_OUTAGE_CAPACITY_RTID = 13103
+
 """
 Settlement	Point Type	Description
 ==========	==========	===========
 Resource Node	RN	Resource Node for normal resource
 Resource Node	PCCRN	Physical Resource Node for combined cycle units
 Resource Node	LCCRN	Logical Resource Node for combined cycle plant
 Resource Node	PUN	Private Area Network Resource Node
@@ -101,15 +126,16 @@
     location_types = [
         LOCATION_TYPE_HUB,
         LOCATION_TYPE_ZONE,
         LOCATION_TYPE_RESOURCE_NODE,
     ]
 
     BASE = "https://www.ercot.com/api/1/services/read/dashboards"
-    ACTUAL_LOADS_URL_FORMAT = "https://www.ercot.com/content/cdr/html/{timestamp}_actual_loads_of_forecast_zones.html"  # noqa
+    ACTUAL_LOADS_FORECAST_ZONES_URL_FORMAT = "https://www.ercot.com/content/cdr/html/{timestamp}_actual_loads_of_forecast_zones.html"  # noqa
+    ACTUAL_LOADS_WEATHER_ZONES_URL_FORMAT = "https://www.ercot.com/content/cdr/html/{timestamp}_actual_loads_of_weather_zones.html"  # noqa
     LOAD_HISTORICAL_MAX_DAYS = 14
     AS_PRICES_HISTORICAL_MAX_DAYS = 30
 
     @dataclass
     class Document:
         url: str
         publish_date: pd.Timestamp
@@ -214,48 +240,142 @@
 
         # return where date_parsed matches mix["Time"]
 
         return mix[mix["Time"].dt.date == date_parsed.date()].reset_index(drop=True)
 
     @support_date_range("DAY_START")
     def get_load(self, date, end=None, verbose=False):
-        """Get load for a date"""
+        """Get load for a date
+
+        Arguments:
+            date (datetime.date, str): "latest", "today", or a date string
+                are supported.
+
+
+        """
         if date == "latest":
-            today_load = self.get_load("today", verbose=verbose)
-            latest = today_load.iloc[-1]
-            return {"load": latest["Load"], "time": latest["Time"]}
+            return self.get_load("today", verbose=verbose)
 
         elif utils.is_today(date, tz=self.default_timezone):
             df = self._get_todays_outlook_non_forecast(date, verbose=verbose)
             df = df.rename(columns={"demand": "Load"})
             return df[["Time", "Interval Start", "Interval End", "Load"]]
 
         elif utils.is_within_last_days(
             date,
             self.LOAD_HISTORICAL_MAX_DAYS,
             tz=self.default_timezone,
         ):
-            df = self._get_load_html(date, verbose)
+            df = self._get_forecast_zone_load_html(date, verbose).rename(
+                columns={"TOTAL": "Load"},
+            )
             return df[["Time", "Interval Start", "Interval End", "Load"]]
 
         else:
             raise NotSupported()
 
-    def _get_load_html(self, when, verbose=False):
+    @support_date_range("DAY_START")
+    def get_load_by_weather_zone(self, date, verbose=False):
+        """Get hourly load for ERCOT weather zones
+
+        Arguments:
+            date (datetime.date, str):  "today", or a date string
+                are supported.
+            verbose(bool): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame
+
+        """
+        if utils.is_today(date, tz=self.default_timezone):
+            df = self._get_weather_zone_load_html(date, verbose=verbose)
+        else:
+            doc_info = self._get_document(
+                report_type_id=ACTUAL_SYSTEM_LOAD_BY_WEATHER_ZONE,
+                date=date + pd.DateOffset(days=1),  # published day after
+                constructed_name_contains="csv.zip",
+                verbose=verbose,
+            )
+
+            df = self.read_doc(doc_info, verbose=verbose)
+        return df
+
+    @support_date_range("DAY_START")
+    def get_load_by_forecast_zone(self, date, verbose=False):
+        """Get hourly load for ERCOT forecast zones
+
+        Arguments:
+            date (datetime.date, str):  "today", or a date string
+                are supported.
+
+            verbose(bool): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame
+        """
+        if utils.is_today(date, tz=self.default_timezone):
+            df = self._get_forecast_zone_load_html(date, verbose=verbose)
+        else:
+            doc_info = self._get_document(
+                report_type_id=ACTUAL_SYSTEM_LOAD_BY_FORECAST_ZONE,
+                date=date + pd.DateOffset(days=1),  # published day after
+                constructed_name_contains="csv.zip",
+                verbose=verbose,
+            )
+
+            df = self.read_doc(doc_info, verbose=verbose)
+        return df
+
+    def _get_forecast_zone_load_html(self, when, verbose=False):
         """Returns load for currentDay or previousDay"""
-        url = self.ACTUAL_LOADS_URL_FORMAT.format(
+        url = self.ACTUAL_LOADS_FORECAST_ZONES_URL_FORMAT.format(
             timestamp=when.strftime("%Y%m%d"),
         )
+        df = self._read_html_display(url=url, verbose=verbose)
+        return df
 
+    def _get_weather_zone_load_html(self, when, verbose=False):
+        """Returns load for currentDay or previousDay"""
+        url = self.ACTUAL_LOADS_WEATHER_ZONES_URL_FORMAT.format(
+            timestamp=when.strftime("%Y%m%d"),
+        )
+        df = self._read_html_display(
+            url=url,
+            verbose=verbose,
+        )
+        return df
+
+    def _read_html_display(self, url, verbose=False):
         msg = f"Fetching {url}"
         log(msg, verbose)
 
         dfs = pd.read_html(url, header=0)
         df = dfs[0]
-        df = self._handle_html_data(df, {"TOTAL": "Load"})
+
+        df["Interval End"] = pd.to_datetime(df["Oper Day"]) + (
+            df["Hour Ending"] / 100
+        ).astype("timedelta64[h]")
+        df["Interval End"] = df["Interval End"].dt.tz_localize(
+            self.default_timezone,
+        )
+        df["Interval Start"] = df["Interval End"] - pd.DateOffset(hours=1)
+        df["Time"] = df["Interval Start"]
+
+        df = utils.move_cols_to_front(
+            df,
+            [
+                "Time",
+                "Interval Start",
+                "Interval End",
+            ],
+        )
+
+        to_drop = ["Oper Day", "Hour Ending"]
+        df = df.drop(to_drop, axis=1)
+
         return df
 
     def _get_todays_outlook_non_forecast(self, date, verbose=False):
         """Returns most recent data point for supply in MW
 
         Updates every 5 minutes
         """
@@ -570,17 +690,17 @@
         """Get SPP data for ERCOT
 
         Supported Markets:
             - ``REAL_TIME_15_MIN``
             - ``DAY_AHEAD_HOURLY``
 
         Supported Location Types:
-            - ``zone``
-            - ``hub``
-            - ``node``
+            - ``Load Zone``
+            - ``Trading Hub``
+            - ``Resource Node``
         """
         if market == Markets.REAL_TIME_15_MIN:
             df = self._get_spp_rtm15(
                 date,
                 verbose,
             )
         elif market == Markets.DAY_AHEAD_HOURLY:
@@ -702,43 +822,26 @@
         date,
         verbose=False,
     ):
         """Get Real-time 15-minute Market SPP data for ERCOT
 
         https://www.ercot.com/mp/data-products/data-product-details?id=NP6-905-CD
         """
-        query_date = date
-        if date == "latest":
-            query_date = utils._handle_date("today", self.default_timezone)
         # returns list of Document(url=,publish_date=)
 
-        query_date_str = f"SPPHLZNP6905_{query_date.strftime('%Y%m%d')}"
         all_docs = self._get_documents(
             report_type_id=SETTLEMENT_POINT_PRICES_AT_RESOURCE_NODES_HUBS_AND_LOAD_ZONES_RTID,
             extension="csv",
             verbose=verbose,
         )
 
-        # look at file name to determine the
-        # date/interval the file represents
-        docs = []
-        for doc in all_docs:
-            if query_date_str + "_0000" in doc.constructed_name:
-                continue
-
-            if (
-                query_date_str in doc.constructed_name
-                or f"SPPHLZNP6905_{(query_date + pd.Timedelta(days=1)).strftime('%Y%m%d')}_0000"  # noqa: E501
-                in doc.constructed_name
-            ):
-                docs.append(doc)
-
-        if date == "latest":
-            # just pluck out the latest document based on publish_date
-            docs = [max(docs, key=lambda x: x.publish_date)]
+        docs = self._filter_spp_rtm_files(
+            all_docs=all_docs,
+            date=date,
+        )
         if len(docs) == 0:
             raise ValueError(f"Could not fetch SPP data for {date}")
 
         all_dfs = []
         for doc_info in tqdm.tqdm(docs, disable=not verbose):
             doc_url = doc_info.url
             msg = f"Fetching {doc_url}"
@@ -747,14 +850,38 @@
             all_dfs.append(df)
 
         df = pd.concat(all_dfs).reset_index(drop=True)
 
         df["Market"] = Markets.REAL_TIME_15_MIN.value
         return df
 
+    def _filter_spp_rtm_files(self, all_docs, date):
+        if date == "latest":
+            # just pluck out the latest document based on publish_date
+            return [max(all_docs, key=lambda x: x.publish_date)]
+        query_date_str = date.strftime("%Y%m%d")
+        docs = []
+        for doc in all_docs:
+            # make sure to handle retry files
+            # e.g SPPHLZNP6905_retry_20230608_1545_csv
+            if "SPPHLZNP6905_" not in doc.constructed_name:
+                continue
+
+            if query_date_str + "_0000" in doc.constructed_name:
+                continue
+
+            if (
+                query_date_str in doc.constructed_name
+                or f"{(date + pd.Timedelta(days=1)).strftime('%Y%m%d')}_0000"  # noqa: E501
+                in doc.constructed_name
+            ):
+                docs.append(doc)
+
+        return docs
+
     @support_date_range(frequency="1Y", update_dates=ercot_update_dates)
     def get_as_prices(
         self,
         date,
         end=None,
         verbose=False,
     ):
@@ -767,15 +894,16 @@
                 data as a range, from "date" to "end"
 
             verbose (bool, optional): print verbose output. Defaults to False.
 
         Returns:
 
             pandas.DataFrame: A DataFrame with prices for "Non-Spinning Reserves", \
-                "Regulation Up", "Regulation Down", "Responsive Reserves".
+                "Regulation Up", "Regulation Down", "Responsive Reserves", \
+                "ERCOT Contingency Reserve Service"
 
         Source:
             https://www.ercot.com/mp/data-products/data-product-details?id=NP4-181-ER
         """
 
         # use to check if we need to pull daily files
         if (
@@ -827,26 +955,27 @@
         print(data)
 
         return data
 
     @support_date_range("DAY_START")
     def _get_as_prices_recent(self, date, verbose=False):
         """Get ancillary service clearing prices in hourly intervals in Day
-            Ahead Market. This function is can return the last 31 days
+            Ahead Market. This function can return the last 31 days
             of ancillary pricing.
 
         Arguments:
             date (datetime.date, str): date of delivery for AS services
 
             verbose (bool, optional): print verbose output. Defaults to False.
 
         Returns:
 
             pandas.DataFrame: A DataFrame with prices for "Non-Spinning Reserves", \
-                "Regulation Up", "Regulation Down", "Responsive Reserves".
+                "Regulation Up", "Regulation Down", "Responsive Reserves", \
+                "ERCOT Contingency Reserve Service"
 
         """
         # subtract one day since it's the day ahead market happens on the day
         # before for the delivery day
 
         date = date - pd.DateOffset(days=1)
 
@@ -881,51 +1010,468 @@
             ).reset_index()
 
             doc.columns.name = None
 
         # some columns from workbook contain trailing/leading whitespace
         doc.columns = [x.strip() for x in doc.columns]
 
-        # NSPIN  REGDN  REGUP  RRS
+        # NSPIN  REGDN  REGUP  RRS  ECRS
         rename = {
             "NSPIN": "Non-Spinning Reserves",
             "REGDN": "Regulation Down",
             "REGUP": "Regulation Up",
             "RRS": "Responsive Reserves",
+            "ECRS": "ERCOT Contingency Reserve Service",
         }
 
         col_order = [
             "Time",
             "Interval Start",
             "Interval End",
             "Market",
             "Non-Spinning Reserves",
             "Regulation Down",
             "Regulation Up",
             "Responsive Reserves",
+            "ERCOT Contingency Reserve Service",
         ]
 
+        if "ECRS" not in doc.columns:
+            doc["ECRS"] = None
+
         doc.rename(columns=rename, inplace=True)
 
         return doc[col_order]
 
+    def get_as_monitor(self, date="latest", verbose=False):
+        """Get Ancillary Service Capacity Monitor.
+
+        Parses table from
+        https://www.ercot.com/content/cdr/html/as_capacity_monitor.html
+
+        Arguments:
+            date (str): only supports "latest"
+            verbose (bool, optional): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: A DataFrame with ancillary service capacity monitor data
+        """
+
+        url = "https://www.ercot.com/content/cdr/html/as_capacity_monitor.html"
+
+        df = self._download_html_table(url, verbose=verbose)
+
+        return df
+
+    def get_real_time_system_conditions(self, date="latest", verbose=False):
+        """Get Real-Time System Conditions.
+
+        Parses table from
+        https://www.ercot.com/content/cdr/html/real_time_system_conditions.html
+
+        Arguments:
+            date (str): only supports "latest"
+            verbose (bool, optional): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: A DataFrame with real-time system conditions
+        """
+
+        url = "https://www.ercot.com/content/cdr/html/real_time_system_conditions.html"
+        df = self._download_html_table(url, verbose=verbose)
+        df = df.rename(
+            columns={
+                "Frequency - Current Frequency": "Current Frequency",
+                "Real-Time Data - Actual System Demand": "Actual System Demand",
+                "Real-Time Data - Average Net Load": "Average Net Load",
+                "Real-Time Data - Total System Capacity (not including Ancillary Services)": "Total System Capacity excluding Ancillary Services",  # noqa: E501
+                "Real-Time Data - Total Wind Output": "Total Wind Output",
+                "Real-Time Data - Total PVGR Output": "Total PVGR Output",
+                "Real-Time Data - Current System Inertia": "Current System Inertia",
+            },
+        )
+
+        return df
+
+    def _download_html_table(self, url, verbose=False):
+        log(f"Downloading {url}", verbose)
+
+        html = requests.get(url).content
+
+        soup = BeautifulSoup(html, "html.parser")
+
+        table = soup.find("table", attrs={"class": "tableStyle"})
+
+        data = {}
+        header = None
+        for row in table.find_all("tr"):
+            cells = row.find_all("td")
+            if cells[0].get("class") == ["headerValueClass"]:
+                header = cells[0].text.strip()  # new header for new dataframe
+            else:
+                category = cells[0].text.strip()
+                value = cells[1].text.strip()
+                header_prepend = header
+                if " (MW)" in header:
+                    header_prepend = header_prepend.replace(" (MW)", "")
+                    category = f"{category} (MW)"
+
+                parsed_value = value.replace(",", "")
+                try:
+                    parsed_value = int(parsed_value)
+                except ValueError:
+                    parsed_value = float(parsed_value)
+
+                data[f"{header_prepend} - {category}"] = parsed_value
+
+        df = pd.DataFrame([data])
+
+        time_div = soup.find("div", attrs={"class": "schedTime rightAlign"})
+        time_text = time_div.text.split(": ")[
+            1
+        ]  # Split the string on ': ' to get just the time part
+
+        df.insert(
+            0,
+            "Time",
+            pd.to_datetime(time_text).tz_localize(self.default_timezone),
+        )
+
+        return df
+
+    @support_date_range("1H")
+    def get_hourly_resource_outage_capacity(self, date, end=None, verbose=False):
+        """Hourly Resource Outage Capacity report sourced
+        from the Outage Scheduler (OS).
+
+        Returns outage data for for next 7 days.
+
+        Total Resource MW doesnt includ IRR, New Equipment outages,
+        retirement of old equipment, seasonal
+        mothballed (during the outaged season),
+        and mothballed.
+
+        As such, it is a proxy for thermal outages.
+
+        Arguments:
+            date (str): time to download. Returns last hourly report
+                before this time. Supports "latest"
+            end (str, optional): end time to download. Defaults to None.
+            verbose (bool, optional): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: A DataFrame with hourly resource outage capacity data
+
+
+        """
+        all_docs = self._get_documents(
+            report_type_id=HOURLY_RESOURCE_OUTAGE_CAPACITY_RTID,
+            extension="csv",
+            verbose=verbose,
+        )
+
+        if date == "latest":
+            doc = max(all_docs, key=lambda x: x.publish_date)
+
+        else:
+            hour = date.floor("1H")
+            for doc in all_docs:
+                if hour == doc.publish_date.floor("1H"):
+                    break
+
+        df = self._handle_hourly_resource_outage_capacity(doc, verbose=verbose)
+
+        return df
+
+    def _handle_hourly_resource_outage_capacity(self, doc, verbose=False):
+        df = self.read_doc(doc, verbose=verbose)
+        df.insert(
+            0,
+            "Publish Time",
+            pd.to_datetime(doc.publish_date).tz_convert(self.default_timezone),
+        )
+
+        outage_types = ["Total Resource", "Total IRR", "Total New Equip Resource"]
+
+        for t in outage_types:
+            t_no_space = t.replace(" ", "")
+            df = df.rename(
+                columns={
+                    f"{t_no_space}MWZoneSouth": f"{t} MW Zone South",
+                    f"{t_no_space}MWZoneNorth": f"{t} MW Zone North",
+                    f"{t_no_space}MWZoneWest": f"{t} MW Zone West",
+                    f"{t_no_space}MWZoneHouston": f"{t} MW Zone Houston",
+                },
+            )
+
+            df.insert(
+                df.columns.tolist().index(f"{t} MW Zone Houston") + 1,
+                f"{t} MW",
+                (
+                    df[f"{t} MW Zone South"]
+                    + df[f"{t} MW Zone North"]
+                    + df[f"{t} MW Zone West"]
+                    + df[f"{t} MW Zone Houston"]
+                ),
+            )
+        return df
+
+    @support_date_range("DAY_START")
+    def get_unplanned_resource_outages(self, date, verbose=False):
+        """Get Unplanned Resource Outages.
+
+        Data published at ~5am central on the 3rd day after the day of interest.
+
+        Arguments:
+            date (str, datetime): date to get data for
+            verbose (bool, optional): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: A DataFrame with unplanned resource outages
+
+        """
+        doc = self._get_document(
+            report_type_id=UNPLANNED_RESOURCE_OUTAGES_REPORT_RTID,
+            date=date.normalize() + pd.DateOffset(days=3),
+            verbose=verbose,
+        )
+
+        xls = utils.get_zip_file(doc.url, verbose=verbose)
+
+        df = self._handle_unplanned_resource_outages_file(xls)
+
+        return df
+
+    def _handle_unplanned_resource_outages_file(self, xls):
+        as_of = pd.to_datetime(
+            pd.read_excel(
+                xls,
+                sheet_name="Unplanned Resource Outages",
+                skiprows=2,
+                nrows=1,
+            )
+            .values[0][0]
+            .split(": ")[1],
+        ).tz_localize(self.default_timezone)
+        df = pd.read_excel(
+            xls,
+            sheet_name="Unplanned Resource Outages",
+            skiprows=4,
+            skipfooter=1,
+        )
+
+        df.insert(0, "Report Time", as_of)
+
+        time_cols = ["Actual Outage Start", "Planned End Date", "Actual End Date"]
+        for col in time_cols:
+            df[col] = pd.to_datetime(df[col]).dt.tz_localize(self.default_timezone)
+
+        return df
+
+    @support_date_range("DAY_START")
+    def get_as_reports(self, date, verbose=False):
+        """Get Ancillary Services Reports.
+
+        Published with a 2 day delay around 3am central
+        """
+        report_date = date.normalize() + pd.DateOffset(days=2)
+
+        doc = self._get_document(
+            report_type_id=TWO_DAY_ANCILLARY_SERVICES_REPORTS_RTID,
+            date=report_date,
+            verbose=verbose,
+        )
+
+        return self._handle_as_reports_file(doc.url, verbose=verbose)
+
+    def _handle_as_reports_file(self, file_path, verbose):
+        z = utils.get_zip_folder(file_path, verbose=verbose)
+
+        # extract the date from the file name
+        date_str = z.namelist()[0][-13:-4]
+
+        self_arranged_products = [
+            "RRSPFR",
+            "RRSUFR",
+            "RRSFFR",
+            "ECRSM",
+            "ECRSS",
+            "REGUP",
+            "REGDN",
+            "NSPIN",
+            "NSPNM",
+        ]
+        cleared_products = [
+            "RRSPFR",
+            "RRSUFR",
+            "RRSFFR",
+            "ECRSM",
+            "ECRSS",
+            "REGUP",
+            "REGDN",
+            "NSPIN",
+        ]
+        offers_products = [
+            "RRSPFR",
+            "RRSUFR",
+            "RRSFFR",
+            "ECRSM",
+            "ECRSS",
+            "REGUP",
+            "REGDN",
+            "ONNS",
+            "OFFNS",
+        ]
+
+        all_dfs = []
+        for as_name in cleared_products:
+            suffix = f"{as_name}-{date_str}.csv"
+            cleared = f"2d_Cleared_DAM_AS_{suffix}"
+
+            if as_name in ["ECRSM", "ECRSS"] and cleared not in z.namelist():
+                continue
+
+            df_cleared = pd.read_csv(z.open(cleared))
+            all_dfs.append(df_cleared)
+
+        for as_name in self_arranged_products:
+            suffix = f"{as_name}-{date_str}.csv"
+            self_arranged = f"2d_Self_Arranged_AS_{suffix}"
+
+            if as_name in ["ECRSM", "ECRSS"] and self_arranged not in z.namelist():
+                continue
+
+            df_self_arranged = pd.read_csv(z.open(self_arranged))
+            all_dfs.append(df_self_arranged)
+
+        def _make_bid_curve(df):
+            return [
+                tuple(x)
+                for x in df[["MW Offered", f"{as_name} Offer Price"]].values.tolist()
+            ]
+
+        for as_name in offers_products:
+            suffix = f"{as_name}-{date_str}.csv"
+            offers = f"2d_Agg_AS_Offers_{suffix}"
+
+            if as_name in ["ECRSM", "ECRSS"] and offers not in z.namelist():
+                continue
+
+            df_offers = pd.read_csv(z.open(offers))
+            name = f"Bid Curve - {as_name}"
+            if df_offers.empty:
+                # use last df to get the index
+                # and set values to None
+                df_offers_hourly = all_dfs[0].rename(
+                    columns={
+                        all_dfs[0].columns[-1]: name,
+                    },
+                )
+                df_offers_hourly[name] = None
+
+            else:
+                df_offers_hourly = (
+                    df_offers.groupby(["Delivery Date", "Hour Ending"])
+                    .apply(_make_bid_curve)
+                    .reset_index(name=name)
+                )
+            all_dfs.append(df_offers_hourly)
+
+        df = pd.concat(
+            [df.set_index(["Delivery Date", "Hour Ending"]) for df in all_dfs],
+            axis=1,
+        ).reset_index()
+
+        return self.parse_doc(df, verbose=verbose)
+
+    @support_date_range("DAY_START")
+    def get_highest_price_as_offer_selected(self, date, verbose=False):
+        """Get the offer price and the name of the Entity submitting
+        the offer for the highest-priced Ancillary Service (AS) Offer.
+
+        Published with 3 day delay
+
+        Arguments:
+            date (str, datetime): date to get data for
+            verbose (bool, optional): print verbose output. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: A DataFrameq
+        """
+        report_date = date.normalize() + pd.DateOffset(days=3)
+
+        doc = self._get_document(
+            report_type_id=THREE_DAY_HIGHEST_PRICE_AS_OFFER_SELECTED_RTID,
+            date=report_date,
+            verbose=verbose,
+        )
+
+        df = self._handle_three_day_highest_price_as_offer_selected_file(doc, verbose)
+
+        return df
+
+    def _handle_three_day_highest_price_as_offer_selected_file(self, doc, verbose):
+        df = self.read_doc(doc, verbose=verbose)
+
+        df = df.rename(
+            columns={
+                "Resource Name with Highest-Priced Offer Selected in DAM and SASMs": "Resource Name",  # noqa: E501
+            },
+        )
+
+        def _handle_offers(df):
+            return pd.Series(
+                {
+                    "Offered Price": df["Offered Price"].iloc[0],
+                    "Total Offered Quantity": df["Offered Quantity"].sum(),
+                    "Offered Quantities": df["Offered Quantity"].tolist(),
+                },
+            )
+
+        df = (
+            df.groupby(
+                [
+                    "Time",
+                    "Interval Start",
+                    "Interval End",
+                    "Market",
+                    "QSE",
+                    "DME",
+                    "Resource Name",
+                    "AS Type",
+                    "Block Indicator",
+                ],
+            )
+            .apply(_handle_offers)
+            .reset_index()
+        )
+
+        return df
+
     def _get_document(
         self,
         report_type_id,
         date=None,
         constructed_name_contains=None,
         verbose=False,
     ) -> Document:
         """Searches by Report Type ID, filtering for date and/or constructed name
 
         Raises a ValueError if no document matches
 
         Returns:
             Latest Document by publish_date
         """
+
+        # no need to pass this on
+        # since this only returns the latest
+        # document anyways
+        if date == "latest":
+            date = None
+
         documents = self._get_documents(
             report_type_id=report_type_id,
             date=date,
             constructed_name_contains=constructed_name_contains,
             verbose=verbose,
         )
         if len(documents) == 0:
@@ -994,31 +1540,14 @@
             .dt.tz_localize("UTC")
             .dt.tz_convert(self.default_timezone)
         )
 
         cols_to_keep = ["Time"] + list(columns.keys())
         return df[cols_to_keep].rename(columns=columns)
 
-    def _handle_html_data(self, df, columns):
-        df["Interval End"] = pd.to_datetime(df["Oper Day"]) + (
-            df["Hour Ending"] / 100
-        ).astype("timedelta64[h]")
-        df["Interval End"] = df["Interval End"].dt.tz_localize(
-            self.default_timezone,
-        )
-        df["Interval Start"] = df["Interval End"] - pd.DateOffset(hours=1)
-        df["Time"] = df["Interval Start"]
-
-        cols_to_keep = [
-            "Time",
-            "Interval Start",
-            "Interval End",
-        ] + list(columns.keys())
-        return df[cols_to_keep].rename(columns=columns)
-
     def _get_settlement_point_mapping(self, verbose=False):
         """Get DataFrame whose columns can help us filter out values"""
 
         doc_info = self._get_document(
             report_type_id=SETTLEMENT_POINTS_LIST_AND_ELECTRICAL_BUSES_MAPPING_RTID,
             verbose=verbose,
         )
@@ -1033,25 +1562,28 @@
         settlement_points_file = [
             name for name in names if "Settlement_Points" in name
         ][0]
         df = pd.read_csv(z.open(settlement_points_file))
         return df
 
     def read_doc(self, doc, verbose=False):
+        log(f"Reading {doc.url}", verbose)
         doc = pd.read_csv(doc.url, compression="zip")
         return self.parse_doc(doc, verbose=verbose)
 
     def parse_doc(self, doc, verbose=False):
         # files sometimes have different naming conventions
         # a more elegant solution would be nice
         doc.rename(
             columns={
                 "Delivery Date": "DeliveryDate",
+                "OperDay": "DeliveryDate",
                 "Hour Ending": "HourEnding",
                 "Repeated Hour Flag": "DSTFlag",
+                "Date": "DeliveryDate",
                 "DeliveryHour": "HourEnding",
                 "Delivery Hour": "HourEnding",
                 "Delivery Interval": "DeliveryInterval",
                 # fix whitespace in column name
                 "DSTFlag    ": "DSTFlag",
             },
             inplace=True,
@@ -1084,17 +1616,21 @@
                 .astype(int)
                 - 1
             )
             doc["Interval Start"] = pd.to_datetime(doc["DeliveryDate"]) + doc[
                 "HourBeginning"
             ].astype("timedelta64[h]")
 
+        ambiguous = "infer"
+        if "DSTFlag" in doc.columns:
+            ambiguous = doc["DSTFlag"] == "Y"
+
         doc["Interval Start"] = doc["Interval Start"].dt.tz_localize(
             self.default_timezone,
-            ambiguous=doc["DSTFlag"] == "Y",
+            ambiguous=ambiguous,
         )
 
         doc["Interval End"] = doc["Interval Start"] + interval_length
 
         doc["Time"] = doc["Interval Start"]
 
         cols_to_keep = [
@@ -1105,19 +1641,22 @@
 
         # todo try to clean up this logic
         doc = doc[cols_to_keep]
         doc = doc.drop(
             columns=[
                 "DeliveryDate",
                 "HourEnding",
-                "DSTFlag",
             ],
         )
-        if "DeliveryInterval" in doc.columns:
-            doc = doc.drop(columns=["DeliveryInterval"])
+
+        optional_drop = ["DSSTFlag", "DeliveryInterval"]
+
+        for col in optional_drop:
+            if col in doc.columns:
+                doc = doc.drop(columns=[col])
 
         return doc
 
 
 if __name__ == "__main__":
     iso = Ercot()
```

### Comparing `gridstatus-0.21.0/gridstatus/isone.py` & `gridstatus-0.22.0/gridstatus/isone.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
     @support_date_range(frequency="DAY_START")
     def get_load(self, date, end=None, verbose=False):
         """Return load at a previous date in 5 minute intervals"""
         # todo document the earliest supported date
         # supports a start and end date
         if date == "latest":
-            return self._latest_from_today(self.get_load)
+            return self.get_load("today", verbose=verbose)
 
         date_str = date.strftime("%Y%m%d")
         url = f"https://www.iso-ne.com/transform/csv/fiveminutesystemload?start={date_str}&end={date_str}"  # noqa
         data = _make_request(url, skiprows=[0, 1, 2, 3, 5], verbose=verbose)
 
         data["Date/Time"] = pd.to_datetime(data["Date/Time"]).dt.tz_localize(
             self.default_timezone,
```

### Comparing `gridstatus-0.21.0/gridstatus/lmp_config.py` & `gridstatus-0.22.0/gridstatus/lmp_config.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/miso.py` & `gridstatus-0.22.0/gridstatus/miso.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         df.index.name = "Interval Start"
         df = df.reset_index()
         df = add_interval_end(df, 5)
         return df
 
     def get_load(self, date, verbose=False):
         if date == "latest":
-            return self._latest_from_today(self.get_load, verbose=verbose)
+            return self.get_load(date="today", verbose=verbose)
 
         elif utils.is_today(date, tz=self.default_timezone):
             r = self._get_load_and_forecast_data(verbose=verbose)
 
             date = pd.to_datetime(r["LoadInfo"]["RefId"].split(" ")[0])
 
             df = pd.DataFrame([x["Load"] for x in r["LoadInfo"]["FiveMinTotalLoad"]])
```

### Comparing `gridstatus-0.21.0/gridstatus/nyiso.py` & `gridstatus-0.22.0/gridstatus/nyiso.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             verbose (bool): Whether to print verbose output. Optional.
 
         Returns:
             pandas.DataFrame: Load data for NYISO and each zone
 
         """
         if date == "latest":
-            return self._latest_from_today(self.get_load)
+            return self.get_load(date="today", verbose=verbose)
 
         data = self._download_nyiso_archive(
             date=date,
             end=end,
             dataset_name="pal",
             verbose=verbose,
         )
@@ -139,14 +139,87 @@
         df.reset_index(inplace=True)
         # drop NA loads
         # data = data.dropna(subset=["Load"])
 
         return df
 
     @support_date_range(frequency="MONTH_START")
+    def get_btm_solar(self, date, end=None, verbose=False):
+        """Returns estimated BTM solar generation at a previous date in hourly
+            intervals for system and each zone.
+
+            Available ~8 hours after the end of the operating day.
+
+        Parameters:
+            date (str, pd.Timestamp, datetime.datetime): Date to get load for.
+              Can be "latest", "today", or a date
+            end (str, pd.Timestamp, datetime.datetime): End date for date range.
+                Optional.
+            verbose (bool): Whether to print verbose output. Optional.
+
+        Returns:
+            pandas.DataFrame: BTM solar data for NYISO system and each zone
+
+        """
+        if date == "latest":
+            return self.get_load(date="today", verbose=verbose)
+
+        data = self._download_nyiso_archive(
+            date=date,
+            end=end,
+            dataset_name="btmactualforecast",
+            filename="BTMEstimatedActual",
+            verbose=verbose,
+        )
+
+        df = data.pivot_table(
+            index=["Time", "Interval Start", "Interval End"],
+            columns="Zone Name",
+            values="MW Value",
+            aggfunc="first",
+        )
+
+        # move system to first column
+        df.insert(0, "SYSTEM", df.pop("SYSTEM"))
+
+        df = df.reset_index()
+
+        df.columns.name = None
+
+        return df
+
+    @support_date_range(frequency="MONTH_START")
+    def get_btm_solar_forecast(self, date, end=None, verbose=False):
+        if date == "latest":
+            return self.get_load(date="today", verbose=verbose)
+
+        data = self._download_nyiso_archive(
+            date=date,
+            end=end,
+            dataset_name="btmdaforecast",
+            verbose=verbose,
+        )
+
+        df = data.pivot_table(
+            index=["Time", "Interval Start", "Interval End"],
+            columns="Zone Name",
+            values="MW Value",
+            aggfunc="first",
+        )
+
+        # move system to first column
+        df.insert(0, "SYSTEM", df.pop("SYSTEM"))
+
+        df = df.reset_index()
+
+        df.columns.name = None
+
+        return df
+
+    @support_date_range(frequency="MONTH_START")
     def get_load_forecast(self, date, end=None, verbose=False):
         """Get load forecast for a date in 1 hour intervals"""
         date = utils._handle_date(date, self.default_timezone)
 
         # todo optimize this to accept a date range
         data = self._download_nyiso_archive(
             date,
@@ -637,18 +710,23 @@
         Returns:
             pandas.DataFrame: the downloaded data
 
         """
         if filename is None:
             filename = dataset_name
 
-        date = gridstatus.utils._handle_date(date)
+        date = gridstatus.utils._handle_date(date, self.default_timezone)
         month = date.strftime("%Y%m01")
         day = date.strftime("%Y%m%d")
 
+        # if same day, we can just download the single file
+        if end is not None and date.normalize() == end.normalize():
+            end = None
+            date = date.normalize()
+
         # the last 7 days of file are hosted directly as csv
         # todo this can probably be optimized to down single csv if
         # a range and all files are in the last 7 days
         if end is None and date > pd.Timestamp.now(
             tz=self.default_timezone,
         ).normalize() - pd.DateOffset(days=7):
             csv_filename = f"{day}{filename}.csv"
@@ -667,19 +745,26 @@
             if end is None:
                 date_range = [date]
             else:
                 date_range = pd.date_range(
                     date.date(),
                     end.date(),
                     freq="1D",
-                    inclusive="both",
-                )
+                    inclusive="left",
+                ).tolist()
+
+                # if end month is not same as start month, don't add to list
+                # this handles case where end is the first of the next month
+                # this pops up from the support_date_range decorator
+                # and that date will be handled in the next month's zip file
+                if end.month == date.month:
+                    date_range += [end]
 
             for d in date_range:
-                d = gridstatus.utils._handle_date(d)
+                d = gridstatus.utils._handle_date(d, tz=self.default_timezone)
                 month = d.strftime("%Y%m01")
                 day = d.strftime("%Y%m%d")
 
                 csv_filename = f"{day}{filename}.csv"
                 if csv_filename not in z.namelist():
                     msg = f"{csv_filename} not found in {zip_url}"
                     log(msg, verbose)
@@ -765,14 +850,18 @@
     "isolf": ("start", 60),
     # dam lmp
     "damlbmp": ("start", 60),
     # rt lmp
     "realtime": ("end", 5),
     # real time events
     "RealTimeEvents": ("instantaneous", None),
+    # btm solar
+    "btmactualforecast": ("start", 60),
+    # btm solar forecast
+    "btmdaforecast": ("start", 60),
 }
 
 
 def _handle_time(df, dataset_name):
     time_type, interval_duration_minutes = dataset_interval_map[dataset_name]
 
     if "Time Stamp" in df.columns:
```

### Comparing `gridstatus-0.21.0/gridstatus/pjm.py` & `gridstatus-0.22.0/gridstatus/pjm.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             * Returns data for the following areas: AE, AEP, APS, ATSI,
             BC, COMED, DAYTON, DEOK, DOM, DPL, DUQ, EKPC, JC,
             ME, PE, PEP, PJM MID ATLANTIC REGION, PJM RTO,
             PJM SOUTHERN REGION, PJM WESTERN REGION, PL, PN, PS, RECO
         """
 
         if date == "latest":
-            return self._latest_from_today(self.get_load, verbose=verbose)
+            return self.get_load("today", verbose=verbose)
 
         # more hourly historical load here: https://dataminer2.pjm.com/feed/hrl_load_metered/definition
 
         # todo can support a load area
         data = {
             "order": "Asc",
             "sort": "datetime_beginning_utc",
```

### Comparing `gridstatus-0.21.0/gridstatus/spp.py` & `gridstatus-0.22.0/gridstatus/spp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 )
 from gridstatus.decorators import support_date_range
 from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
 
 FS_RTBM_LMP_BY_LOCATION = "rtbm-lmp-by-location"
 FS_DAM_LMP_BY_LOCATION = "da-lmp-by-location"
-MARKETPLACE_BASE_URL = "https://marketplace.spp.org"
-FILE_BROWSER_API_URL = "https://marketplace.spp.org/file-browser-api/"
+MARKETPLACE_BASE_URL = "https://portal.spp.org"
+FILE_BROWSER_API_URL = "https://portal.spp.org/file-browser-api/"
+FILE_BROWSER_DOWNLOAD_URL = "https://portal.spp.org/file-browser-api/download"
 
 LOCATION_TYPE_HUB = "HUB"
 LOCATION_TYPE_INTERFACE = "INTERFACE"
 LOCATION_TYPE_SETTLEMENT_LOCATION = "SETTLEMENT_LOCATION"
 
 QUERY_RTM5_HUBS_URL = "https://pricecontourmap.spp.org/arcgis/rest/services/MarketMaps/RTBM_FeatureData/MapServer/1/query"  # noqa
 QUERY_RTM5_INTERFACES_URL = "https://pricecontourmap.spp.org/arcgis/rest/services/MarketMaps/RTBM_FeatureData/MapServer/2/query"  # noqa
@@ -115,49 +116,50 @@
             ).reset_index(drop=True)
 
         if not utils.is_today(date, self.default_timezone):
             # https://marketplace.spp.org/pages/generation-mix-historical
             # many years of historical 5 minute data
             raise NotSupported
 
-        url = "https://marketplace.spp.org/file-browser-api/download/generation-mix-historical?path=%2FGenMix2Hour.csv"  # noqa
+        url = f"{FILE_BROWSER_DOWNLOAD_URL}/generation-mix-historical?path=%2FGenMix2Hour.csv"  # noqa
         df_raw = pd.read_csv(url)
         historical_mix = process_gen_mix(df_raw, detailed=detailed)
 
         historical_mix = historical_mix.drop(
             columns=["Short Term Load Forecast", "Average Actual Load"],
             errors="ignore",
         )
 
         return historical_mix
 
     def get_load(self, date, verbose=False):
         """Returns load for last 24hrs in 5 minute intervals"""
+        original_date = date
 
         if date == "latest":
-            return self._latest_from_today(self.get_load)
+            date = "today"
 
-        elif utils.is_today(date, tz=self.default_timezone):
-            date = utils._handle_date(date, self.default_timezone)
+        date = utils._handle_date(date, self.default_timezone)
 
-            df = self._get_load_and_forecast(verbose=verbose)
-
-            df = df.dropna(subset=["Actual Load"])
-
-            df = df.rename(columns={"Actual Load": "Load"})
+        df = self._get_load_and_forecast(verbose=verbose)
 
-            df = df[["Time", "Load"]]
+        df = df.dropna(subset=["Actual Load"])
 
-            # returns two days, so make sure to only return current day's load
-            df = df[df["Time"].dt.date == date.date()]
+        df = df.rename(columns={"Actual Load": "Load"})
 
-            df = df.reset_index(drop=True)
+        df = df[["Time", "Load"]]
+        df = df.reset_index(drop=True)
+        df = add_interval(df, interval_min=5)
 
-            df = add_interval(df, interval_min=5)
+        if original_date == "latest":
+            return df
 
+        elif utils.is_today(original_date, tz=self.default_timezone):
+            # returns two days, so make sure to only return current day's load
+            df = df[df["Time"].dt.date == date.date()].reset_index(drop=True)
             return df
 
         else:
             # hourly historical zonal loads
             # https://marketplace.spp.org/pages/hourly-load
             raise NotSupported()
 
@@ -256,15 +258,15 @@
 
         Args:
             date: start date
             end: end date
 
 
         """
-        url = f"https://marketplace.spp.org/file-browser-api/download/ver-curtailments?path=%2F{date.strftime('%Y')}%2F{date.strftime('%m')}%2FVER-Curtailments-{date.strftime('%Y%m%d')}.csv"  # noqa
+        url = f"{FILE_BROWSER_DOWNLOAD_URL}/ver-curtailments?path=%2F{date.strftime('%Y')}%2F{date.strftime('%m')}%2FVER-Curtailments-{date.strftime('%Y%m%d')}.csv"  # noqa
 
         msg = f"Downloading {url}"
         log(msg, verbose)
         df = pd.read_csv(url)
 
         return self._process_ver_curtailments(df)
 
@@ -275,15 +277,15 @@
         Args:
             year: year to get data for
             verbose: print url
 
         Returns:
             pd.DataFrame: VER Curtailments
         """
-        url = f"https://marketplace.spp.org/file-browser-api/download/ver-curtailments?path=%2F{year}%2F{year}.zip"  # noqa
+        url = f"{FILE_BROWSER_DOWNLOAD_URL}/ver-curtailments?path=%2F{year}%2F{year}.zip"  # noqa
         z = utils.get_zip_folder(url, verbose=verbose)
 
         # iterate through all files in zip
         # find the one that end with .csv
         # read that csv
         all_dfs = []
         for f in z.filelist:
@@ -298,15 +300,15 @@
         df = df[~df["Interval Start"].isnull()]
 
         df = df.sort_values("Time")
 
         return df
 
     def _get_load_and_forecast(self, verbose=False):
-        url = "https://marketplace.spp.org/chart-api/load-forecast/asChart"
+        url = f"{MARKETPLACE_BASE_URL}/chart-api/load-forecast/asChart"
 
         msg = f"Getting load and forecast from {url}"
         log(msg, verbose)
 
         r = self._get_json(url)["response"]
 
         data = {"Time": r["labels"]}
@@ -325,15 +327,15 @@
         ).dt.tz_convert(self.default_timezone)
 
         return df
 
         # todo where does date got in argument order
         # def get_historical_lmp(self, date, market: str, nodes: list):
         # 5 minute interal data
-        # https://marketplace.spp.org/file-browser-api/download/rtbm-lmp-by-location?path=/2022/08/By_Interval/08/RTBM-LMP-SL-202208082125.csv
+        # {FILE_BROWSER_API_URL}/rtbm-lmp-by-location?path=/2022/08/By_Interval/08/RTBM-LMP-SL-202208082125.csv
 
         # hub and interface prices
         # https://marketplace.spp.org/pages/hub-and-interface-prices
 
         # historical generation mix
         # https://marketplace.spp.org/pages/generation-mix-rolling-365
         # https://marketplace.spp.org/chart-api/gen-mix-365/asFile
@@ -783,15 +785,15 @@
             df = pd.DataFrame(list_results.json())
             return df
         else:
             return pd.DataFrame()
 
     def _file_browser_download_url(self, fs_name, params=None):
         qs = "?" + urlencode(params) if params else ""
-        return f"{FILE_BROWSER_API_URL}download/{fs_name}{qs}"
+        return f"{FILE_BROWSER_DOWNLOAD_URL}/{fs_name}{qs}"
 
     @staticmethod
     def _clean_status_text(text):
         text = text.lower()
 
         # remove punctuation
         text = re.sub(r"[,\.\(\)]", "", text)
```

### Comparing `gridstatus-0.21.0/gridstatus/tests/base_test_iso.py` & `gridstatus-0.22.0/gridstatus/tests/base_test_iso.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,19 +210,18 @@
         df = self.iso.get_load(test_date)
         self._check_load(df)
         assert df.loc[0]["Time"].strftime(
             "%Y%m%d",
         ) == test_date.strftime("%Y%m%d")
 
     def test_get_load_latest(self):
-        load = self.iso.get_load("latest")
-        set(["time", "load"]) == load.keys()
-        assert is_numeric_dtype(type(load["load"]))
+        df = self.iso.get_load("latest")
+        self._check_load(df)
         today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
-        assert load["time"].date() == today
+        assert df["Time"].max().date() == today
 
     def test_get_load_today(self):
         df = self.iso.get_load("today")
         self._check_load(df)
         today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
         assert (df["Time"].dt.date == today).all()
         return df
```

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_caiso.py` & `gridstatus-0.22.0/gridstatus/tests/test_caiso.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_eia.py` & `gridstatus-0.22.0/gridstatus/tests/test_eia.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,32 @@
     # assert interval start and interval end are datetimes in utc
     assert df["Interval Start"].dtype == "datetime64[ns, UTC]"
     assert df["Interval End"].dtype == "datetime64[ns, UTC]"
     assert df.shape[0] > 0
     assert df.columns.tolist() == columns
 
 
+def _check_region_data(df):
+    columns = [
+        "Interval Start",
+        "Interval End",
+        "Respondent",
+        "Respondent Name",
+        "Load",
+        "Load Forecast",
+        "Net Generation",
+        "Total Interchange",
+    ]
+
+    assert df["Interval Start"].dtype == "datetime64[ns, UTC]"
+    assert df["Interval End"].dtype == "datetime64[ns, UTC]"
+    assert df.shape[0] > 0
+    assert df.columns.tolist() == columns
+
+
 def test_rto_interchange():
     eia = gridstatus.EIA()
 
     start = "2020-01-01"
     end = "2020-01-04"
 
     df = eia.get_dataset(
@@ -35,14 +53,30 @@
 
     assert df["Interval End"].min().date() == pd.Timestamp(start).date()
     assert df["Interval End"].max().date() == pd.Timestamp(end).date()
 
     _check_interchange(df)
 
 
+def test_rto_region_data():
+    eia = gridstatus.EIA()
+    start = "2020-01-01"
+    end = "2020-01-04"
+    df = eia.get_dataset(
+        dataset="electricity/rto/region-data",
+        start=start,
+        end=end,
+        verbose=True,
+    )
+
+    assert df["Interval End"].min().date() == pd.Timestamp(start).date()
+    assert df["Interval End"].max().date() == pd.Timestamp(end).date()
+    _check_region_data(df)
+
+
 def test_list_routes():
     eia = gridstatus.EIA()
 
     routes = eia.list_routes("electricity/rto/")
 
     assert "interchange-data" in [r["id"] for r in routes["routes"]]
```

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_gridstatus.py` & `gridstatus-0.22.0/gridstatus/tests/test_gridstatus.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_isone.py` & `gridstatus-0.22.0/gridstatus/tests/test_isone.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_lmp_config.py` & `gridstatus-0.22.0/gridstatus/tests/test_lmp_config.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_miso.py` & `gridstatus-0.22.0/gridstatus/tests/test_miso.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_nyiso.py` & `gridstatus-0.22.0/gridstatus/tests/test_nyiso.py`

 * *Files 12% similar despite different names*

```diff
@@ -245,12 +245,91 @@
 
         df = self.iso.get_fuel_mix(date=date)
         assert df.shape[0] >= 281
 
         df = self.iso.get_load(date=date)
         assert df.shape[0] >= 281
 
+    # test btm solar
+    def test_get_btm_solar(self):
+        # published ~8 hours after finish of previous day
+        two_days_ago = pd.Timestamp.now(tz="US/Eastern").date() - pd.Timedelta(days=2)
+        df = self.iso.get_btm_solar(
+            date=two_days_ago,
+            verbose=True,
+        )
+
+        columns = [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "SYSTEM",
+            "CAPITL",
+            "CENTRL",
+            "DUNWOD",
+            "GENESE",
+            "HUD VL",
+            "LONGIL",
+            "MHK VL",
+            "MILLWD",
+            "N.Y.C.",
+            "NORTH",
+            "WEST",
+        ]
+
+        assert df.columns.tolist() == columns
+        assert df.shape[0] >= 0
+
+        # test range last month
+        start = "2023-04-30"
+        end = "2023-05-02"
+        df = self.iso.get_btm_solar(
+            start=start,
+            end=end,
+            verbose=True,
+        )
+
+        assert df["Time"].dt.date.nunique() == 3
+
+    def test_get_btm_solar_forecast(self):
+        df = self.iso.get_btm_solar_forecast(
+            date="today",
+            verbose=True,
+        )
+
+        columns = [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "SYSTEM",
+            "CAPITL",
+            "CENTRL",
+            "DUNWOD",
+            "GENESE",
+            "HUD VL",
+            "LONGIL",
+            "MHK VL",
+            "MILLWD",
+            "N.Y.C.",
+            "NORTH",
+            "WEST",
+        ]
+
+        assert df.columns.tolist() == columns
+        assert df.shape[0] >= 0
+
+        # test range last month
+        start = "2023-04-30"
+        end = "2023-05-02"
+        df = self.iso.get_btm_solar_forecast(
+            start=start,
+            end=end,
+            verbose=True,
+        )
+
+        assert df["Time"].dt.date.nunique() == 3
+
     @staticmethod
     def _check_status(df):
         assert set(df.columns) == set(
             ["Time", "Status", "Notes"],
         )
```

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_pjm.py` & `gridstatus-0.22.0/gridstatus/tests/test_pjm.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_save_to.py` & `gridstatus-0.22.0/gridstatus/tests/test_save_to.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_spp.py` & `gridstatus-0.22.0/gridstatus/tests/test_spp.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/tests/test_viz.py` & `gridstatus-0.22.0/gridstatus/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus/utils.py` & `gridstatus-0.22.0/gridstatus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,26 +189,22 @@
     if locations != "ALL" and locations is not None:
         df = df[df["Location"].isin(locations)]
 
     return df
 
 
 def get_zip_file(url, verbose=False):
-    # todo add retry logic
-    # todo does this need to be a with statement?
-    log(f"Downloading {url}", verbose=verbose)
-    r = requests.get(url)
-    z = ZipFile(io.BytesIO(r.content))
+    z = get_zip_folder(url, verbose=verbose)
     return z.open(z.namelist()[0])
 
 
-def get_zip_folder(zip_url, verbose=False):
-    msg = f"Requesting {zip_url}"
+def get_zip_folder(url, verbose=False):
+    msg = f"Requesting {url}"
     log(msg, verbose)
-    r = requests.get(zip_url)
+    r = requests.get(url)
     z = ZipFile(io.BytesIO(r.content))
     return z
 
 
 def is_today(date, tz):
     return _handle_date(date, tz=tz).date() == pd.Timestamp.now(tz=tz).date()
```

### Comparing `gridstatus-0.21.0/gridstatus/viz.py` & `gridstatus-0.22.0/gridstatus/viz.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus.egg-info/PKG-INFO` & `gridstatus-0.22.0/gridstatus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatus
-Version: 0.21.0
+Version: 0.22.0
 Summary: API to access energy data
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gridstatus Version: 0.21.0 Summary: API to access
+Metadata-Version: 2.1 Name: gridstatus Version: 0.22.0 Summary: API to access
 energy data Author-email: Max Kanter
 gmail.com> Maintainer-email: Max Kanter
 gmail.com> License: Copyright 2022 James Max Kanter Redistribution and use in
 source and binary forms, with or without modification, are permitted provided
 that the following conditions are met: 1. Redistributions of source code must
 retain the above copyright notice, this list of conditions and the following
 disclaimer. 2. Redistributions in binary form must reproduce the above
```

### Comparing `gridstatus-0.21.0/gridstatus.egg-info/SOURCES.txt` & `gridstatus-0.22.0/gridstatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/gridstatus.egg-info/requires.txt` & `gridstatus-0.22.0/gridstatus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/pyproject.toml` & `gridstatus-0.22.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gridstatus-0.21.0/utils/ercot/README.md` & `gridstatus-0.22.0/utils/ercot/README.md`

 * *Files identical despite different names*

