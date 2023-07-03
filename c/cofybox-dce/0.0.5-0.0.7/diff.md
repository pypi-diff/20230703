# Comparing `tmp/cofybox-dce-0.0.5.tar.gz` & `tmp/cofybox-dce-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofybox-dce-0.0.5.tar", last modified: Thu Mar 31 13:39:06 2022, max compression
+gzip compressed data, was "cofybox-dce-0.0.7.tar", last modified: Mon Jul  3 11:02:21 2023, max compression
```

## Comparing `cofybox-dce-0.0.5.tar` & `cofybox-dce-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,32 @@
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-03-31 13:39:06.241110 cofybox-dce-0.0.5/
--rw-r--r--   0 Jan        (504) staff       (20)     1055 2021-09-30 09:51:08.000000 cofybox-dce-0.0.5/LICENSE
--rw-r--r--   0 Jan        (504) staff       (20)      644 2022-03-31 13:39:06.241178 cofybox-dce-0.0.5/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      101 2021-09-29 10:14:10.000000 cofybox-dce-0.0.5/README.md
--rw-r--r--   0 Jan        (504) staff       (20)      103 2021-09-30 09:40:16.000000 cofybox-dce-0.0.5/pyproject.toml
--rw-r--r--   0 Jan        (504) staff       (20)      687 2022-03-31 13:39:06.241505 cofybox-dce-0.0.5/setup.cfg
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-03-31 13:39:06.238171 cofybox-dce-0.0.5/src/
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-03-31 13:39:06.240215 cofybox-dce-0.0.5/src/cofybox_dce/
--rw-r--r--   0 Jan        (504) staff       (20)        0 2021-09-30 09:37:01.000000 cofybox-dce-0.0.5/src/cofybox_dce/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)     1086 2022-02-11 15:10:39.000000 cofybox-dce-0.0.5/src/cofybox_dce/abstract.py
--rw-r--r--   0 Jan        (504) staff       (20)      822 2022-03-31 13:29:33.000000 cofybox-dce-0.0.5/src/cofybox_dce/factory.py
--rw-r--r--   0 Jan        (504) staff       (20)      259 2021-09-29 15:01:19.000000 cofybox-dce-0.0.5/src/cofybox_dce/misc.py
--rw-r--r--   0 Jan        (504) staff       (20)     4450 2022-03-31 13:37:07.000000 cofybox-dce-0.0.5/src/cofybox_dce/octopus_outgoing_workaround.py
--rw-r--r--   0 Jan        (504) staff       (20)     1737 2022-03-31 13:38:25.000000 cofybox-dce-0.0.5/src/cofybox_dce/pricing.py
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2022-03-31 13:39:06.241006 cofybox-dce-0.0.5/src/cofybox_dce.egg-info/
--rw-r--r--   0 Jan        (504) staff       (20)      644 2022-03-31 13:39:05.000000 cofybox-dce-0.0.5/src/cofybox_dce.egg-info/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      417 2022-03-31 13:39:06.000000 cofybox-dce-0.0.5/src/cofybox_dce.egg-info/SOURCES.txt
--rw-r--r--   0 Jan        (504) staff       (20)        1 2022-03-31 13:39:05.000000 cofybox-dce-0.0.5/src/cofybox_dce.egg-info/dependency_links.txt
--rw-r--r--   0 Jan        (504) staff       (20)       34 2022-03-31 13:39:06.000000 cofybox-dce-0.0.5/src/cofybox_dce.egg-info/requires.txt
--rw-r--r--   0 Jan        (504) staff       (20)       12 2022-03-31 13:39:06.000000 cofybox-dce-0.0.5/src/cofybox_dce.egg-info/top_level.txt
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.545331 cofybox-dce-0.0.7/
+-rw-r--r--   0 Jan        (504) staff       (20)     1055 2021-09-30 09:51:08.000000 cofybox-dce-0.0.7/LICENSE
+-rw-r--r--   0 Jan        (504) staff       (20)      608 2023-07-03 11:02:21.545433 cofybox-dce-0.0.7/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      101 2021-09-29 10:14:10.000000 cofybox-dce-0.0.7/README.md
+-rw-r--r--   0 Jan        (504) staff       (20)      103 2021-09-30 09:40:16.000000 cofybox-dce-0.0.7/pyproject.toml
+-rw-r--r--   0 Jan        (504) staff       (20)      705 2023-07-03 11:02:21.545864 cofybox-dce-0.0.7/setup.cfg
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.538311 cofybox-dce-0.0.7/src/
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.540756 cofybox-dce-0.0.7/src/cofybox_dce/
+-rw-r--r--   0 Jan        (504) staff       (20)        0 2021-09-30 09:37:01.000000 cofybox-dce-0.0.7/src/cofybox_dce/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)      907 2023-07-03 09:07:57.000000 cofybox-dce-0.0.7/src/cofybox_dce/abstract.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2245 2023-07-03 10:58:34.000000 cofybox-dce-0.0.7/src/cofybox_dce/factory.py
+-rw-r--r--   0 Jan        (504) staff       (20)      287 2023-06-29 14:21:07.000000 cofybox-dce-0.0.7/src/cofybox_dce/misc.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.543757 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/
+-rw-r--r--   0 Jan        (504) staff       (20)      200 2023-07-03 10:59:02.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)     3354 2023-07-03 11:00:07.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/belgium.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2075 2023-07-03 10:52:16.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/france.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1949 2023-07-03 10:48:15.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus.py
+-rw-r--r--   0 Jan        (504) staff       (20)     4624 2023-07-03 10:53:33.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus_outgoing_workaround.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1331 2023-07-03 10:48:03.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/pricing.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2271 2023-07-03 11:00:28.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/spain.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.541900 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/
+-rw-r--r--   0 Jan        (504) staff       (20)      608 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      790 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/SOURCES.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        1 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/dependency_links.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       51 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/requires.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       12 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/top_level.txt
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.545150 cofybox-dce-0.0.7/tests/
+-rw-r--r--   0 Jan        (504) staff       (20)     1980 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_belgium.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2522 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_factory.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1119 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_france.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2170 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_octopus.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2087 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_spain.py
```

### Comparing `cofybox-dce-0.0.5/LICENSE` & `cofybox-dce-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.5/PKG-INFO` & `cofybox-dce-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: cofybox-dce
-Version: 0.0.5
+Version: 0.0.7
 Summary: COFYCloud Data Collector Engine python code
 Home-page: https://docs.cofybox.io
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/rescoopvpp/cofybox-dce/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cofybox-dce
 
 COFYbox Data Collector Engine.
 Collects data from external sources, outputs DataFrames
-
```

### Comparing `cofybox-dce-0.0.5/setup.cfg` & `cofybox-dce-0.0.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cofybox-dce
-version = 0.0.5
+version = 0.0.7
 author = Jan Pecinovsky
 author_email = jan@energieid.be
 description = COFYCloud Data Collector Engine python code
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.cofybox.io
 project_urls = 
@@ -18,14 +18,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	pandas==1.4.0
 	octopusagile==0.0.6
+	entsoe-py==0.5.9
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cofybox-dce-0.0.5/src/cofybox_dce/octopus_outgoing_workaround.py` & `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus_outgoing_workaround.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,72 +3,77 @@
 
 THIS FILE NEEDS TO BE INCLUDED IN A FUTURE PYPI RELEASE OF OCTOPUS AGILE
 """
 
 import collections
 import logging
 from datetime import datetime, timedelta
+from typing import Optional
 
 import requests
 
 _LOGGER = logging.getLogger("OctopusOutgoing")
 
 
 class Outgoing:
+    """Class to request Octopus Outgoing Tariffs"""
+
     area_code = None
     url = None
 
     def __init__(self, area_code):
         self.area_code = area_code
         self.url = f"https://api.octopus.energy/v1/products/AGILE-OUTGOING-19-05-13/electricity-tariffs/E-1R-AGILE-OUTGOING-19-05-13-{area_code}/standard-unit-rates/"
 
-    def round_time(self, t: datetime) -> datetime:
+    def round_time(self, _time: datetime) -> datetime:
         """Rounds to start of current half hour time period
         Args:
-            t (datetime): a datetime object
+            _time (datetime): a datetime object
         Returns:
             datetime: the datetime representing the start of the half hour
                 time period
         """
         minute = 00
-        if t.minute // 30 == 1:
+        if _time.minute // 30 == 1:
             minute = 30
-        return t.replace(second=0, microsecond=0, minute=minute, hour=t.hour)
+        return _time.replace(second=0, microsecond=0, minute=minute, hour=_time.hour)
 
-    def get_raw_rates(self, date_from: str, date_to: str = None):
+    def get_raw_rates(self, date_from: str, date_to: Optional[str] = None):
         """Outgoing rate data from the Octopus API
         Args:
             date_from (str): date from in format "%Y-%m-%dT%H:%M:%SZ"
             date_to (str): date to in format "%Y-%m-%dT%H:%M:%SZ"
         Returns
             dict: the raw outgoing rate data
         """
         date_from = f"?period_from={ date_from }"
         if date_to is not None:
             date_to = f"&period_to={ date_to }"
         else:
             date_to = ""
         headers = {"content-type": "application/json"}
-        r = requests.get(f"{self.url}/{ date_from }{ date_to }", headers=headers)
-        results = r.json()["results"]
-        _LOGGER.debug(r.url)
+        request = requests.get(
+            f"{self.url}/{ date_from }{ date_to }", headers=headers, timeout=30
+        )
+        results = request.json()["results"]
+        _LOGGER.debug(request.url)
         return results
 
     def get_new_rates(self) -> dict:
         """
         Returns
             dict: all available future outgoing rates:
                 * date_rate (dict): Dict of date/time as key and rate as vaue
                 * rate_list (list): All outgoing rates as a list
         """
 
         date_from = datetime.strftime(datetime.utcnow(), "%Y-%m-%dT%H:%M:%SZ")
         return self.get_rates(date_from)
 
-    def get_rates(self, date_from: str, date_to: str = None) -> dict:
+    def get_rates(self, date_from: str, date_to: Optional[str] = None) -> dict:
         """
         Args:
             date_from (str): date from in format "%Y-%m-%dT%H:%M:%SZ"
             date_to (str): date to in format "%Y-%m-%dT%H:%M:%SZ"
         Returns
             dict: outgoing rates:
                 * date_rate (dict): Dict of date/time as key and rate as vaue
@@ -118,8 +123,8 @@
         """
         now = self.round_time(datetime.utcnow())
         rounded_time = datetime.strftime(
             self.round_time(now) + timedelta(minutes=30), "%Y-%m-%dT%H:%M:%SZ"
         )
         next_time = datetime.strftime(now + timedelta(minutes=60), "%Y-%m-%dT%H:%M:%SZ")
         date_rates = self.get_rates(rounded_time, next_time)["date_rates"]
-        return date_rates[next(iter(date_rates))]
+        return date_rates[next(iter(date_rates))]
```

### Comparing `cofybox-dce-0.0.5/src/cofybox_dce/pricing.py` & `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,64 @@
+"""Collectors for Octopus Energy"""
+
+import warnings
 from typing import Optional
+
 import pandas as pd
 from OctopusAgile import Agile
-from cofybox_dce.octopus_outgoing_workaround import Outgoing
-import warnings
 
-from .abstract import PricingCollector
-from .misc import iso8601z
+from ..misc import iso8601z
+from .octopus_outgoing_workaround import Outgoing
+from .pricing import PricingCollector
 
 
 class Octopus(PricingCollector):
-    country = 'UK'
-    supplier = 'Octopus'
-    timezone = 'Europe/London'
-    unit = 'p£/kWh'
+    """Collector for Octopus Agile"""
+
+    country = "UK"
+    supplier = "Octopus"
+    timezone = "Europe/London"
+    unit = "p£/kWh"
 
     def __init__(self, region_code: str, **kwargs):
+        """Initialize"""
+        self.region_code = region_code
         self.agile = Agile(region_code)
-        self.price_name = f'{self.supplier}_{region_code}'
-        super(Octopus, self).__init__(**kwargs)
+        self.price_name = f"{self.supplier}_{region_code}"
+        super().__init__(**kwargs)
 
-    def get_data(
-            self,
-            interval: Optional[pd.Interval] = None,
+    async def get_data(
+        self,
+        interval: Optional[pd.Interval] = None,
     ) -> pd.DataFrame:
+        """Request data"""
         if not interval:
             rates = self.agile.get_new_rates()
         else:
             date_from = iso8601z(interval.left)
             date_to = iso8601z(interval.right)
             if interval.length.days > 2:
                 warnings.warn(
-                    'You requested an interval larger than 2 days, '
-                    'be advised that the response may not be complete')
+                    "You requested an interval larger than 2 days, "
+                    "be advised that the response may not be complete"
+                )
             rates = self.agile.get_rates(date_from, date_to)
 
-        rates = pd.DataFrame.from_dict(rates['date_rates'], orient='index')
+        rates = pd.DataFrame.from_dict(rates["date_rates"], orient="index")
         # noinspection PyTypeChecker
         rates.index = pd.to_datetime(rates.index)
-        rates.rename(columns={0: 'value_inc_vat'}, inplace=True)
+        rates.rename(columns={0: "value_inc_vat"}, inplace=True)
         rates = rates.tz_convert(self.timezone)
         rates.sort_index(inplace=True)
-        rates['Unit'] = self.unit
+        rates["Unit"] = self.unit
         return rates
 
 
 class OctopusOutgoing(Octopus):
-    supplier = 'Octopus_Outgoing'
+    """Collector for Octopus Outgoing Prices"""
+
+    supplier = "Octopus_Outgoing"
 
     def __init__(self, region_code: str, **kwargs):
-        super(OctopusOutgoing, self).__init__(region_code=region_code, **kwargs)
+        """Initialize"""
+        super().__init__(region_code=region_code, **kwargs)
         self.agile = Outgoing(region_code)
```

### Comparing `cofybox-dce-0.0.5/src/cofybox_dce.egg-info/PKG-INFO` & `cofybox-dce-0.0.7/src/cofybox_dce.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: cofybox-dce
-Version: 0.0.5
+Version: 0.0.7
 Summary: COFYCloud Data Collector Engine python code
 Home-page: https://docs.cofybox.io
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/rescoopvpp/cofybox-dce/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cofybox-dce
 
 COFYbox Data Collector Engine.
 Collects data from external sources, outputs DataFrames
-
```

