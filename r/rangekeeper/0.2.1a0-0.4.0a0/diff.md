# Comparing `tmp/rangekeeper-0.2.1a0.tar.gz` & `tmp/rangekeeper-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rangekeeper-0.2.1a0.tar", max compression
+gzip compressed data, was "rangekeeper-0.4.0a0.tar", max compression
```

## Comparing `rangekeeper-0.2.1a0.tar` & `rangekeeper-0.4.0a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0    16725 2023-05-17 15:02:56.622311 rangekeeper-0.2.1a0/LICENSE
--rwxr-xr-x   0        0        0     1615 2023-05-18 13:03:49.441937 rangekeeper-0.2.1a0/README.md
--rwxr-xr-x   0        0        0     1029 2023-05-18 13:39:10.131779 rangekeeper-0.2.1a0/pyproject.toml
--rwxr-xr-x   0        0        0     1284 2023-05-17 15:02:56.651556 rangekeeper-0.2.1a0/rangekeeper/__init__.py
--rwxr-xr-x   0        0        0     2714 2023-05-17 15:02:56.651651 rangekeeper-0.2.1a0/rangekeeper/api.py
--rwxr-xr-x   0        0        0     9159 2023-05-17 15:02:56.651782 rangekeeper-0.2.1a0/rangekeeper/distribution.py
--rwxr-xr-x   0        0        0      207 2023-05-17 15:02:56.651889 rangekeeper-0.2.1a0/rangekeeper/dynamics/__init__.py
--rwxr-xr-x   0        0        0     2512 2023-05-17 15:02:56.651986 rangekeeper-0.2.1a0/rangekeeper/dynamics/black_swan.py
--rwxr-xr-x   0        0        0    16122 2023-05-18 03:02:43.724566 rangekeeper-0.2.1a0/rangekeeper/dynamics/cyclicality.py
--rwxr-xr-x   0        0        0    14841 2023-05-17 15:02:56.652228 rangekeeper-0.2.1a0/rangekeeper/dynamics/market.py
--rwxr-xr-x   0        0        0     1320 2023-05-17 15:02:56.652316 rangekeeper-0.2.1a0/rangekeeper/dynamics/noise.py
--rwxr-xr-x   0        0        0     2361 2023-05-17 15:02:56.652407 rangekeeper-0.2.1a0/rangekeeper/dynamics/trend.py
--rwxr-xr-x   0        0        0     5158 2023-05-17 15:02:56.652500 rangekeeper-0.2.1a0/rangekeeper/dynamics/volatility.py
--rwxr-xr-x   0        0        0     2974 2023-05-17 15:02:56.652595 rangekeeper-0.2.1a0/rangekeeper/extrapolation.py
--rwxr-xr-x   0        0        0    25004 2023-05-17 15:02:56.652746 rangekeeper-0.2.1a0/rangekeeper/flux.py
--rwxr-xr-x   0        0        0     3992 2023-05-17 15:02:56.652878 rangekeeper-0.2.1a0/rangekeeper/graph.py
--rwxr-xr-x   0        0        0     4138 2023-05-17 15:02:56.653017 rangekeeper-0.2.1a0/rangekeeper/measure.py
--rwxr-xr-x   0        0        0      199 2023-05-17 15:02:56.653120 rangekeeper-0.2.1a0/rangekeeper/models/__init__.py
--rwxr-xr-x   0        0        0     5461 2023-05-17 15:02:56.653249 rangekeeper-0.2.1a0/rangekeeper/models/deterministic.py
--rwxr-xr-x   0        0        0     6878 2023-05-17 15:02:56.653370 rangekeeper-0.2.1a0/rangekeeper/models/flexible.py
--rwxr-xr-x   0        0        0     5627 2023-05-17 15:02:56.653494 rangekeeper-0.2.1a0/rangekeeper/models/linear.py
--rwxr-xr-x   0        0        0     6389 2023-05-17 15:02:56.653612 rangekeeper-0.2.1a0/rangekeeper/models/linear_graph.py
--rwxr-xr-x   0        0        0     6116 2023-05-17 15:02:56.653737 rangekeeper-0.2.1a0/rangekeeper/models/probabilistic.py
--rwxr-xr-x   0        0        0     7330 2023-05-17 15:02:56.653910 rangekeeper-0.2.1a0/rangekeeper/periodicity.py
--rw-r--r--   0        0        0      567 2023-05-18 06:03:32.581789 rangekeeper-0.2.1a0/rangekeeper/policy.py
--rwxr-xr-x   0        0        0     8752 2023-05-17 15:02:56.654185 rangekeeper-0.2.1a0/rangekeeper/projection.py
--rwxr-xr-x   0        0        0     6856 2023-05-17 15:02:56.654323 rangekeeper-0.2.1a0/rangekeeper/segmentation.py
--rwxr-xr-x   0        0        0     1164 2023-05-17 15:02:56.654437 rangekeeper-0.2.1a0/rangekeeper/space.py
--rwxr-xr-x   0        0        0     7715 2023-05-17 15:02:56.654565 rangekeeper-0.2.1a0/rangekeeper/span.py
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 rangekeeper-0.2.1a0/PKG-INFO
+-rwxr-xr-x   0        0        0    16725 2023-05-17 15:02:56.622311 rangekeeper-0.4.0a0/LICENSE
+-rwxr-xr-x   0        0        0     1615 2023-06-16 00:51:56.463723 rangekeeper-0.4.0a0/README.md
+-rwxr-xr-x   0        0        0     1107 2023-07-03 04:31:13.220499 rangekeeper-0.4.0a0/pyproject.toml
+-rwxr-xr-x   0        0        0     1742 2023-06-16 00:51:56.561615 rangekeeper-0.4.0a0/rangekeeper/__init__.py
+-rwxr-xr-x   0        0        0     4790 2023-06-25 13:20:04.785577 rangekeeper-0.4.0a0/rangekeeper/api.py
+-rwxr-xr-x   0        0        0     9159 2023-05-17 15:02:56.651782 rangekeeper-0.4.0a0/rangekeeper/distribution.py
+-rwxr-xr-x   0        0        0      207 2023-05-17 15:02:56.651889 rangekeeper-0.4.0a0/rangekeeper/dynamics/__init__.py
+-rwxr-xr-x   0        0        0     2512 2023-05-17 15:02:56.651986 rangekeeper-0.4.0a0/rangekeeper/dynamics/black_swan.py
+-rwxr-xr-x   0        0        0    16122 2023-06-16 00:51:56.562003 rangekeeper-0.4.0a0/rangekeeper/dynamics/cyclicality.py
+-rwxr-xr-x   0        0        0    14841 2023-05-17 15:02:56.652228 rangekeeper-0.4.0a0/rangekeeper/dynamics/market.py
+-rwxr-xr-x   0        0        0     1320 2023-05-17 15:02:56.652316 rangekeeper-0.4.0a0/rangekeeper/dynamics/noise.py
+-rwxr-xr-x   0        0        0     2361 2023-05-17 15:02:56.652407 rangekeeper-0.4.0a0/rangekeeper/dynamics/trend.py
+-rwxr-xr-x   0        0        0     5158 2023-05-17 15:02:56.652500 rangekeeper-0.4.0a0/rangekeeper/dynamics/volatility.py
+-rwxr-xr-x   0        0        0     2974 2023-05-17 15:02:56.652595 rangekeeper-0.4.0a0/rangekeeper/extrapolation.py
+-rwxr-xr-x   0        0        0    25969 2023-06-29 14:34:44.921352 rangekeeper-0.4.0a0/rangekeeper/flux.py
+-rwxr-xr-x   0        0        0    27006 2023-06-30 03:17:42.028832 rangekeeper-0.4.0a0/rangekeeper/graph.py
+-rwxr-xr-x   0        0        0     4138 2023-05-17 15:02:56.653017 rangekeeper-0.4.0a0/rangekeeper/measure.py
+-rwxr-xr-x   0        0        0      199 2023-05-17 15:02:56.653120 rangekeeper-0.4.0a0/rangekeeper/models/__init__.py
+-rwxr-xr-x   0        0        0     5461 2023-05-17 15:02:56.653249 rangekeeper-0.4.0a0/rangekeeper/models/deterministic.py
+-rwxr-xr-x   0        0        0     6878 2023-05-17 15:02:56.653370 rangekeeper-0.4.0a0/rangekeeper/models/flexible.py
+-rwxr-xr-x   0        0        0     5627 2023-05-17 15:02:56.653494 rangekeeper-0.4.0a0/rangekeeper/models/linear.py
+-rwxr-xr-x   0        0        0     6389 2023-05-17 15:02:56.653612 rangekeeper-0.4.0a0/rangekeeper/models/linear_graph.py
+-rwxr-xr-x   0        0        0     6116 2023-05-17 15:02:56.653737 rangekeeper-0.4.0a0/rangekeeper/models/probabilistic.py
+-rwxr-xr-x   0        0        0     8591 2023-06-29 14:34:44.924722 rangekeeper-0.4.0a0/rangekeeper/periodicity.py
+-rw-r--r--   0        0        0      567 2023-06-16 00:51:56.562404 rangekeeper-0.4.0a0/rangekeeper/policy.py
+-rwxr-xr-x   0        0        0     8891 2023-06-29 14:34:44.925138 rangekeeper-0.4.0a0/rangekeeper/projection.py
+-rwxr-xr-x   0        0        0     6856 2023-05-17 15:02:56.654323 rangekeeper-0.4.0a0/rangekeeper/segmentation.py
+-rwxr-xr-x   0        0        0     1163 2023-06-16 00:51:56.562561 rangekeeper-0.4.0a0/rangekeeper/space.py
+-rwxr-xr-x   0        0        0     7738 2023-06-29 14:34:44.925484 rangekeeper-0.4.0a0/rangekeeper/span.py
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 rangekeeper-0.4.0a0/PKG-INFO
```

### Comparing `rangekeeper-0.2.1a0/LICENSE` & `rangekeeper-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/README.md` & `rangekeeper-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/pyproject.toml` & `rangekeeper-0.4.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Rangekeeper"
-version = "0.2.1-alpha"
+version = "0.4.0-alpha"
 description = "A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like"
 authors = ["Daniel Fink <danfink@mit.edu>"]
 license = "MPL-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
@@ -26,14 +26,18 @@
 jupyterlab = "^4.0.0"
 docutils = "0.17.1" # See https://jupyterbook.org/en/stable/content/citations.html#citations-and-bibliographies
 tqdm = "^4.65.0"
 multiprocess = "^0.70.14"
 seaborn = "^0.12.2"
 jupyter-book = "^0.15.1"
 sphinx-rtd-theme = "^1.2.0"
+pygraphviz = "^1.11"
+pyvis = "^0.3.2"
+plotly = "^5.15.0"
+pyppeteer = "^1.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rangekeeper-0.2.1a0/rangekeeper/distribution.py` & `rangekeeper-0.4.0a0/rangekeeper/distribution.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/dynamics/black_swan.py` & `rangekeeper-0.4.0a0/rangekeeper/dynamics/black_swan.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/dynamics/cyclicality.py` & `rangekeeper-0.4.0a0/rangekeeper/dynamics/cyclicality.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/dynamics/market.py` & `rangekeeper-0.4.0a0/rangekeeper/dynamics/market.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/dynamics/noise.py` & `rangekeeper-0.4.0a0/rangekeeper/dynamics/noise.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/dynamics/trend.py` & `rangekeeper-0.4.0a0/rangekeeper/dynamics/trend.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/dynamics/volatility.py` & `rangekeeper-0.4.0a0/rangekeeper/dynamics/volatility.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/extrapolation.py` & `rangekeeper-0.4.0a0/rangekeeper/extrapolation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/flux.py` & `rangekeeper-0.4.0a0/rangekeeper/flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import rangekeeper as rk
 
 
 def _format_series(
         series: pd.Series,
         units: pint.Unit,
         decimals: int = 2):
-
     if units.dimensionality == '[currency]':
         formatted = pd.Series(
             data=[str(locale.currency(value, grouping=True)) for value in series],
             index=pd.Series(series.index, name='date'),
             name=series.name)
     else:
         floatfmt = "{:." + str(decimals) + "f}"
@@ -93,19 +92,21 @@
         return _format_series(
             series=self.movements,
             units=self.units).to_markdown(
             stralign="right",
             numalign="right",
             tablefmt='html')
 
-    def duplicate(self) -> Flow:
+    def duplicate(
+            self,
+            name: str = None) -> Flow:
         return self.__class__(
             movements=self.movements.copy(deep=True),
             units=self.units,
-            name=self.name)
+            name=self.name if name is None else name)
 
     # def _format(
     #         self,
     #         decimals: int = 2):
 
     def display(
             self,
@@ -218,14 +219,17 @@
                 raise ValueError("Unsupported extrapolation form")
 
         elif isinstance(proj, rk.projection.Distribution):
             movements = value * proj.interval_density()
         else:
             raise ValueError("Unsupported projection type: {0}".format(type(proj)))
 
+        # movements = movements[proj.bounds[0].to_timestamp(how='start'):proj.bounds[1].to_timestamp(how='end')]  # Fix for >yearly periodicities
+        # TODO: Fix for issues with >yearly periodicities inducing movements at the end of multi-year periods beyond the end of the projection
+
         return cls(
             movements=movements,
             units=units,
             name=name)
 
     def invert(self) -> Flow:
         """
@@ -242,14 +246,17 @@
         :return:
         """
         return self.__class__.from_dict(
             name=self.name,
             movements={self.movements.index[-1]: self.movements.sum()},
             units=self.units)
 
+    def total(self) -> np.float64:
+        return self.collapse().movements[0]
+
     def pv(
             self,
             period_type: rk.periodicity.Type,
             discount_rate: float,
             name: str = None) -> Flow:
         """
         Returns a Flow with values discounted to the present (i.e. before its first period) by a specified rate
@@ -434,14 +441,27 @@
 
     # def display(
     #         self,
     #         decimals: int = 2):
     #     format = self._format(decimals=decimals)
     #     print(format + os.linesep)
 
+    def __iadd__(self, other):
+        flows = self.flows
+        if isinstance(other, Flow):
+            flows.append(other)
+        elif isinstance(other, Stream):
+            flows.extend(other.flows)
+        else:
+            raise Exception("Cannot add type " + type(other).__name__ + " to Stream.")
+        return self.__class__(
+            name=self.name,
+            flows=flows,
+            period_type=self.period_type)
+
     def duplicate(self) -> Stream:
         return self.__class__(
             name=self.name,
             flows=[flow.duplicate() for flow in self.flows],
             period_type=self.period_type)
 
     @classmethod
@@ -613,16 +633,16 @@
         # Check if all units are the same:
         if not len(list(set(list(self.units.values())))) == 1:
             raise ValueError("Error: summation requires all flows' units to be the same. Units: {0}".format(
                 json.dumps(
                     {flow.name: flow.units.__str__() for flow in self.flows}, indent=4)))
 
         return Flow.from_periods(
-            name=name if name is not None else self.name,
-            index=self.frame.index,  # .to_period(),
+            name=name if name is not None else self.name + ' (sum)',
+            index=self.frame.index,
             data=self.frame.sum(axis=1).to_list(),
             units=next(iter(self.units.values())))
 
     def product(
             self,
             name: str = None,
             registry: pint.UnitRegistry = None,
@@ -641,15 +661,15 @@
             registry=registry)
         reduced_units = rk.measure.remove_dimension(
             quantity=registry.Quantity(1, units),
             dimension='[time]',
             registry=registry).units
 
         return Flow.from_periods(
-            name=name if name is not None else self.name,
+            name=name if name is not None else self.name + ' (product)',
             index=self.frame.index,  # .to_period(),
             data=self.frame.prod(axis=1).to_list(),
             units=reduced_units)
 
     def collapse(self) -> Stream:
         """
         Returns an Stream with Flows' movements collapsed (summed) to the Stream's final period
@@ -657,14 +677,17 @@
         """
         flows = [self.extract(flow_name=flow_name) for flow_name in list(self.frame.columns)]
         return self.__class__(
             name=self.name,
             flows=[flow.collapse() for flow in flows],
             period_type=self.period_type)
 
+    def total(self) -> np.float64:
+        return self.sum().collapse().movements[0]
+
     def append(
             self,
             flows: [Flow]) -> None:
         """
         Appends a list of Flows to the Stream
         :param flows:
         :type flows:
```

### Comparing `rangekeeper-0.2.1a0/rangekeeper/measure.py` & `rangekeeper-0.4.0a0/rangekeeper/measure.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/models/deterministic.py` & `rangekeeper-0.4.0a0/rangekeeper/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/models/flexible.py` & `rangekeeper-0.4.0a0/rangekeeper/models/flexible.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/models/linear.py` & `rangekeeper-0.4.0a0/rangekeeper/models/linear.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/models/linear_graph.py` & `rangekeeper-0.4.0a0/rangekeeper/models/linear_graph.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/models/probabilistic.py` & `rangekeeper-0.4.0a0/rangekeeper/models/probabilistic.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/periodicity.py` & `rangekeeper-0.4.0a0/rangekeeper/periodicity.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,26 +7,39 @@
 import enum
 from datetime import datetime
 import dateutil.relativedelta
 import pandas as pd
 
 import rangekeeper as rk
 
+
 class Type(enum.Enum):
+    DECADE = '10A'
+    SEMIDECADE = '5A'
+    BIENNIUM = '2A'
     YEAR = 'A-DEC'  # Anchored on end of December
+    SEMIYEAR = '6M'  # Anchored on end of June & December
     QUARTER = 'Q-DEC'  # Anchored on end of March, June, September, & December
     MONTH = 'M'  # Anchored on end-of-month
     SEMIMONTH = 'SM'  # Twice-monthly periods anchored on mid-month and end-of-month dates
     WEEK = 'W'  # Anchored on Sundays
     DAY = 'D'  # Daily
 
 
 def from_value(value: str):
+    if value == '10A':
+        return Type.DECADE
+    if value == '5A':
+        return Type.SEMIDECADE
+    if value == '2A':
+        return Type.BIENNIUM
     if value == 'A-DEC':
         return Type.YEAR
+    if value == '6M':
+        return Type.SEMIYEAR
     if value == 'Q-DEC':
         return Type.QUARTER
     if value == 'M':
         return Type.MONTH
     if value == 'SM':
         return Type.SEMIMONTH
     if value == 'W':
@@ -66,46 +79,49 @@
     elif isinstance(bound, int):
         return pd.period_range(
             start=include_start,
             periods=bound,
             freq=period_type.value,
             name='periods')
 
+
 def offset_periodindex(
         index: pd.PeriodIndex,
         offset_start: Optional[int] = None,
         offset_end: Optional[int] = None) -> pd.PeriodIndex:
     """
     Returns a pd.PeriodIndex with periods offset by given number of periods (of type given by the index)
     """
     start = index[0].to_timestamp()
     if offset_start is not None:
         start = offset_date(
-            date=period_index[0].to_timestamp(),
+            date=start,
             period_type=from_value(index.freq),
             num_periods=offset_start)
     end = index[-1].to_timestamp()
     if offset_end is not None:
         end = offset_date(
             date=index[-1].to_timestamp(),
             period_type=from_value(index.freq),
             num_periods=offset_end)
     return period_index(
         include_start=start,
         period_type=from_value(index.freq),
         bound=end)
 
+
 def to_span(period_index: pd.PeriodIndex):
     """
     Returns a Span encompassing a pd.PeriodIndex
     """
     return rk.span.Span(
         start_date=period_index[0].to_timestamp(how='start'),
         end_date=period_index[-1].to_timestamp(how='end'))
 
+
 def single_period_index(period: pd.Period) -> pd.PeriodIndex:
     return pd.period_range(
         start=period,
         periods=1)
 
 
 def to_datestamps(
@@ -121,15 +137,19 @@
         timestamps = period_index.to_timestamp(how='start')
     datestamps = timestamps.date
     return pd.DatetimeIndex(datestamps)
 
 
 def periods_per_year(period_type: Type) -> int:
     return {
+        Type.DECADE: 0.1,
+        Type.SEMIDECADE: 0.2,
+        Type.BIENNIUM: 0.5,
         Type.YEAR: 1,
+        Type.SEMIYEAR: 2,
         Type.QUARTER: 4,
         Type.MONTH: 12,
         Type.SEMIMONTH: 24,
         Type.WEEK: 52,
         Type.DAY: 365
         }.get(period_type, None)
 
@@ -145,16 +165,24 @@
     :param period_type:
     :type period_type:
     :param num_periods:
     :type num_periods:
     :return:
     :rtype:
     """
-    if period_type.value == Type.YEAR.value:
+    if period_type.value == Type.DECADE.value:
+        return date + pd.DateOffset(years=10 * num_periods)
+    elif period_type.value == Type.SEMIDECADE.value:
+        return date + pd.DateOffset(years=5 * num_periods)
+    elif period_type.value == Type.BIENNIUM.value:
+        return date + pd.DateOffset(years=2 * num_periods)
+    elif period_type.value == Type.YEAR.value:
         return date + pd.DateOffset(years=num_periods)
+    elif period_type.value == Type.SEMIYEAR.value:
+        return date + pd.DateOffset(months=6 * num_periods)
     elif period_type.value == Type.QUARTER.value:
         return date + pd.DateOffset(months=3 * num_periods)
     elif period_type.value == Type.MONTH.value:
         return date + pd.DateOffset(months=num_periods)
     elif period_type.value == Type.WEEK.value:
         return date + pd.DateOffset(weeks=num_periods)
     elif period_type.value == Type.DAY.value:
@@ -176,16 +204,24 @@
         calc_end_date = offset_date(
             date=end_date,
             period_type=Type.DAY,
             num_periods=1)
 
     delta = dateutil.relativedelta.relativedelta(calc_end_date, start_date)
 
-    if period_type.value == Type.YEAR.value:
+    if period_type.value == Type.DECADE.value:
+        result = math.floor(delta.years / 10)
+    elif period_type.value == Type.SEMIDECADE.value:
+        result = math.floor(delta.years / 5)
+    elif period_type.value == Type.BIENNIUM.value:
+        result = math.floor(delta.years / 2)
+    elif period_type.value == Type.YEAR.value:
         result = delta.years
+    elif period_type.value == Type.SEMIYEAR.value:
+        result = (delta.years * 2) + math.floor(delta.months / 6)
     elif period_type.value == Type.QUARTER.value:
         result = (delta.years * 4) + math.floor(delta.months / 3)
     elif period_type.value == Type.MONTH.value:
         result = (delta.years * 12) + delta.months
     elif period_type.value == Type.SEMIMONTH.value:
         result = (delta.years * 24) + delta.months * 2
     elif period_type.value == Type.WEEK.value:
```

### Comparing `rangekeeper-0.2.1a0/rangekeeper/policy.py` & `rangekeeper-0.4.0a0/rangekeeper/policy.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/projection.py` & `rangekeeper-0.4.0a0/rangekeeper/projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,22 +122,31 @@
             type=self.padding[0])
         right = self._pad(
             value=terms[-1],
             length=right_length.n,
             type=self.padding[1])
         data = np.concatenate((left, terms, right))
 
-        return pd.Series(
+        start = self.bounds[0].to_timestamp(how='start')
+        bound = self.bounds[1].to_timestamp(how='end')
+
+        period_index = rk.periodicity.period_index(
+            include_start=start,
+            period_type=rk.periodicity.from_value(self.sequence.freq),
+            bound=bound)
+
+        index = rk.periodicity.to_datestamps(period_index=period_index)
+
+        result = pd.Series(
             data=data,
-            index=rk.periodicity.to_datestamps(
-                rk.periodicity.period_index(
-                    include_start=self.bounds[0].to_timestamp(how='start'),
-                    period_type=rk.periodicity.from_value(self.sequence.freq),
-                    bound=self.bounds[1].to_timestamp(how='start'))))
+            index=index)
+
+        # result = result[start:bound]
 
+        return result
 
 class Distribution(Projection):
     form: rk.distribution.Form
 
     def __init__(
             self,
             form: rk.distribution.Form,
```

### Comparing `rangekeeper-0.2.1a0/rangekeeper/segmentation.py` & `rangekeeper-0.4.0a0/rangekeeper/segmentation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.2.1a0/rangekeeper/space.py` & `rangekeeper-0.4.0a0/rangekeeper/space.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, List, Union, Optional
 from decimal import Decimal
 from pint import Quantity
 
 import rangekeeper as rk
 
 
-class Space(rk.graph.Element):
+class Space(rk.graph.Entity):
     def __init__(
             self,
             name: str,
             type: str,
             measurements: Dict[rk.measure.Measure, Quantity] = None,
             events: List[rk.graph.Event] = None,
             attributes: Dict = None):
```

### Comparing `rangekeeper-0.2.1a0/rangekeeper/span.py` & `rangekeeper-0.4.0a0/rangekeeper/span.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
 import rangekeeper as rk
 
+
 class Span:
     start_date: pd.Timestamp
     end_date: pd.Timestamp
     name: str = None
     """
     A `Span` is a pd.Interval of pd.Timestamps that bound its start and end dates
     """
@@ -184,15 +185,16 @@
         :rtype:
         """
         if len(names) != len(dates) - 1:
             raise Exception('Error: number of Span names must equal number of Spans created'
                             ' (i.e. one less than number of dates)')
 
         date_pairs = list(zip(dates, dates[1:]))
-        date_pairs = [(start, rk.periodicity.offset_date(end, rk.periodicity.Type.DAY, -1)) for (start, end) in date_pairs]
+        date_pairs = [(start, rk.periodicity.offset_date(end, rk.periodicity.Type.DAY, -1)) for (start, end) in
+                      date_pairs]
 
         spans = []
         for i in range(len(names)):
             spans.append(cls(name=names[i], start_date=date_pairs[i][0], end_date=date_pairs[i][1]))
         return spans
 
     @classmethod
```

### Comparing `rangekeeper-0.2.1a0/PKG-INFO` & `rangekeeper-0.4.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rangekeeper
-Version: 0.2.1a0
+Version: 0.4.0a0
 Summary: A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like
 License: MPL-2.0
 Author: Daniel Fink
 Author-email: danfink@mit.edu
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -18,17 +18,21 @@
 Requires-Dist: jupyter-book (>=0.15.1,<0.16.0)
 Requires-Dist: jupyterlab (>=4.0.0,<5.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: py-linq (>=1.4.0,<2.0.0)
 Requires-Dist: py-moneyed (>=3.0,<4.0)
+Requires-Dist: pygraphviz (>=1.11,<2.0)
+Requires-Dist: pyppeteer (>=1.0.2,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Requires-Dist: pyxirr (>=0.9.0,<0.10.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: specklepy (>=2.12.0,<3.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

