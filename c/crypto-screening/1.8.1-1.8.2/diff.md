# Comparing `tmp/crypto-screening-1.8.1.tar.gz` & `tmp/crypto-screening-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.8.1.tar", last modified: Fri Jun 30 15:39:06 2023, max compression
+gzip compressed data, was "crypto-screening-1.8.2.tar", last modified: Mon Jul  3 11:17:36 2023, max compression
```

## Comparing `crypto-screening-1.8.1.tar` & `crypto-screening-1.8.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.779683 crypto-screening-1.8.1/
--rw-rw-rw-   0        0        0       98 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-30 15:39:06.779683 crypto-screening-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.8.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.8.1/build.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.758684 crypto-screening-1.8.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.771716 crypto-screening-1.8.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.8.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.8.1/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    10119 2023-06-30 15:31:03.000000 crypto-screening-1.8.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18829 2023-06-30 15:31:13.000000 crypto-screening-1.8.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.8.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.8.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5267 2023-06-30 15:34:44.000000 crypto-screening-1.8.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.771716 crypto-screening-1.8.1/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.773684 crypto-screening-1.8.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.8.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.8.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     7987 2023-06-30 15:33:11.000000 crypto-screening-1.8.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.778684 crypto-screening-1.8.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3391 2023-06-30 10:45:18.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24997 2023-06-30 10:47:57.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5401 2023-06-30 10:44:43.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.8.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.8.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9964 2023-06-30 15:35:25.000000 crypto-screening-1.8.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.8.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.767684 crypto-screening-1.8.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.8.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.8.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 15:39:06.779683 crypto-screening-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-30 15:38:55.000000 crypto-screening-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.126212 crypto-screening-1.8.2/
+-rw-rw-rw-   0        0        0       98 2023-07-03 11:17:34.000000 crypto-screening-1.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-03 11:17:36.126212 crypto-screening-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.8.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.8.2/build.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.045473 crypto-screening-1.8.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.080444 crypto-screening-1.8.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.8.2/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.8.2/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10119 2023-06-30 15:31:03.000000 crypto-screening-1.8.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18829 2023-06-30 15:31:13.000000 crypto-screening-1.8.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.8.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.8.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5267 2023-06-30 15:34:44.000000 crypto-screening-1.8.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.084474 crypto-screening-1.8.2/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.102444 crypto-screening-1.8.2/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.8.2/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.8.2/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     7987 2023-06-30 15:33:11.000000 crypto-screening-1.8.2/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.125242 crypto-screening-1.8.2/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.8.2/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.8.2/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3219 2023-07-03 10:58:09.000000 crypto-screening-1.8.2/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.8.2/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24974 2023-07-03 10:52:01.000000 crypto-screening-1.8.2/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5402 2023-07-03 10:51:03.000000 crypto-screening-1.8.2/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.8.2/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.8.2/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9964 2023-06-30 15:35:25.000000 crypto-screening-1.8.2/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.8.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:17:36.058471 crypto-screening-1.8.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-03 11:17:35.000000 crypto-screening-1.8.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2023-07-03 11:17:35.000000 crypto-screening-1.8.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 11:17:35.000000 crypto-screening-1.8.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-03 11:17:35.000000 crypto-screening-1.8.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 11:17:35.000000 crypto-screening-1.8.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-03 11:17:34.000000 crypto-screening-1.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.8.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.8.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 11:17:36.126212 crypto-screening-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-03 10:56:45.000000 crypto-screening-1.8.2/setup.py
```

### Comparing `crypto-screening-1.8.1/PKG-INFO` & `crypto-screening-1.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.8.1
+Version: 1.8.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - written and owned by: Shahaf Frank-Shapir
 - all the rights are saved for Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `crypto-screening-1.8.1/README.md` & `crypto-screening-1.8.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - written and owned by: Shahaf Frank-Shapir
 - all the rights are saved for Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `crypto-screening-1.8.1/build.py` & `crypto-screening-1.8.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/collect/assets.py` & `crypto-screening-1.8.2/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/collect/exchanges.py` & `crypto-screening-1.8.2/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/collect/screeners.py` & `crypto-screening-1.8.2/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/collect/symbols.py` & `crypto-screening-1.8.2/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/dataset.py` & `crypto-screening-1.8.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/interval.py` & `crypto-screening-1.8.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/market/foundation/data.py` & `crypto-screening-1.8.2/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.8.2/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.8.2/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/market/screeners/base.py` & `crypto-screening-1.8.2/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/market/screeners/container.py` & `crypto-screening-1.8.2/crypto_screening/market/screeners/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # container.py
 
 from typing import Iterable, List
 
 from represent import Modifiers
 
-from crypto_screening.collect.assets import exchanges_symbols_quote_assets
 from crypto_screening.market.screeners.base import (
     BaseScreener, structure_screener_datasets
 )
 from crypto_screening.market.screeners.recorder import MarketRecorder
 
 class ScreenersContainer(MarketRecorder):
     """
@@ -27,36 +26,35 @@
     >>> from crypto_screening.market.screeners.container import ScreenersContainer
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
     >>> dynamic_screener = ScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
-    >>> dynamic_screener.screener(exchange="binance", symbol="BTC/USDT"))
+    >>> dynamic_screener.find_screener(exchange="binance", symbol="BTC/USDT"))
     >>> dynamic_screener.data(exchange="binance", symbol="BTC/USDT", length=10))
     """
 
-    modifiers = Modifiers(hidden=["screeners", "currencies"], excluded=["structure"])
+    __slots__ = "screeners",
+
+    modifiers = Modifiers(hidden=["screeners"], excluded=["structure"])
 
     def __init__(self, screeners: Iterable[BaseScreener]) -> None:
         """
         Defines the class attributes.
 
         :param screeners: The data screener object.
         """
 
         super().__init__(market=structure_screener_datasets(screeners=screeners))
 
         self.screeners = screeners
-
-        self.currencies = exchanges_symbols_quote_assets(data=self.market)
-        self.exchanges = list(self.market.keys())
     # end __init__
 
-    def screener(self, exchange: str, symbol: str) -> BaseScreener:
+    def find_screener(self, exchange: str, symbol: str) -> BaseScreener:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
         :return: The data.
@@ -72,15 +70,15 @@
         for screener in self.screeners:
             if (screener.exchange == exchange) and (screener.symbol == symbol):
                 return screener
             # end if
         # end for
     # end screener
 
-    def screeners(self, exchange: str, symbol: str) -> List[BaseScreener]:
+    def find_screeners(self, exchange: str, symbol: str) -> List[BaseScreener]:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
         :return: The data.
```

### Comparing `crypto-screening-1.8.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.8.2/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.8.2/crypto_screening/market/screeners/orderbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,16 +121,14 @@
     >>> from crypto_screening.market.screeners import market_orderbook_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = market_orderbook_recorder(data=market)
     """
 
-    __slots__ = "market"
-
     COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
 
     def parameters(self) -> RecorderParameters:
         """
         Returns the order book parameters.
 
         :return: The order book parameters.
@@ -349,15 +347,15 @@
 
     modifiers = Modifiers(**BaseMultiScreener.modifiers)
     modifiers.excluded.extend(
         ['screening_parameters', 'feeds_parameters', 'handler']
     )
 
     __slots__ = (
-        "handler", 'amount', "loop", "limited", "feeds_parameters",
+        "handler", 'amount', "loop", "limited", "_feeds_parameters",
         "_run_parameters", 'refresh'
     )
 
     screeners: List[OrderbookScreener]
     recorder: MarketOrderbookRecorder
 
     DELAY = 5
@@ -408,15 +406,15 @@
         self.amount = amount or self.AMOUNT
         self.refresh = refresh
 
         self.screeners[:] = list(screeners or []) or self.create_screeners()
 
         self.loop: Optional[asyncio.AbstractEventLoop] = None
 
-        self.feeds_parameters: Optional[Dict[str, Any]] = None
+        self._feeds_parameters: Optional[Dict[str, Any]] = None
         self._run_parameters: Optional[Dict[str, Any]] = None
     # end __init__
 
     def create_screener(
             self,
             symbol: str,
             exchange: str,
@@ -508,15 +506,15 @@
         :param data: The data of the exchanges and symbols to add.
         :param parameters: The parameters for the exchanges.
         :param fixed: The value for fixed parameters to all exchanges.
         :param amount: The maximum amount of symbols for each feed.
         :param separator: The separator of the assets.
         """
 
-        self.feeds_parameters = dict(
+        self._feeds_parameters = dict(
             data=data, fixed=fixed, separator=separator,
             parameters=parameters
         )
 
         feed_params = self.recorder.parameters()
         feed_params.update(parameters or {})
 
@@ -525,26 +523,26 @@
             parameters=feed_params, amount=amount or self.amount
         )
     # end add_feeds
 
     def refresh_feeds(self) -> None:
         """Refreshes the feed objects."""
 
-        if self.feeds_parameters is None:
+        if self._feeds_parameters is None:
             warnings.warn(
                 "Cannot refresh feeds as there was "
                 "no feeds initialization to repeat."
             )
 
             return
         # end if
 
         self.handler.feeds.clear()
 
-        self.add_feeds(**self.feeds_parameters)
+        self.add_feeds(**self._feeds_parameters)
     # end refresh
 
     def rerun(self) -> None:
         """Refreshes the process."""
 
         if self._run_parameters is None:
             warnings.warn(
```

### Comparing `crypto-screening-1.8.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.8.2/crypto_screening/market/screeners/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     >>> recorder = MarketRecorder(data=market)
 
     """
 
     modifiers = Modifiers(**BaseModel.modifiers)
     modifiers.hidden.append("market")
 
-    __slots__ = "market"
+    __slots__ = "market",
 
     def __init__(self, market: Optional[Market] = None) -> None:
         """
         Defines the class attributes.
 
         :param market: The object to fill with the crypto feed record.
         """
```

### Comparing `crypto-screening-1.8.1/crypto_screening/market/waiting.py` & `crypto-screening-1.8.2/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/process.py` & `crypto-screening-1.8.2/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/symbols.py` & `crypto-screening-1.8.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening/validate.py` & `crypto-screening-1.8.2/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.8.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.8.1
+Version: 1.8.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - written and owned by: Shahaf Frank-Shapir
 - all the rights are saved for Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `crypto-screening-1.8.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.8.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.1/pyproject.toml` & `crypto-screening-1.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.8.1'
+version = '1.8.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.8.1/setup.py` & `crypto-screening-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.8.1',
+        version='1.8.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

