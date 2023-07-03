# Comparing `tmp/findmyorder-1.5.2.tar.gz` & `tmp/findmyorder-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.2.tar", max compression
+gzip compressed data, was "findmyorder-1.5.3.tar", max compression
```

## Comparing `findmyorder-1.5.2.tar` & `findmyorder-1.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-26 19:19:02.821749 findmyorder-1.5.2/LICENSE
--rw-r--r--   0        0        0     2219 2023-06-26 19:19:02.821749 findmyorder-1.5.2/README.md
--rw-r--r--   0        0        0      113 2023-06-26 19:19:03.529761 findmyorder-1.5.2/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-06-26 19:19:02.821749 findmyorder-1.5.2/findmyorder/config.py
--rw-r--r--   0        0        0     2265 2023-06-26 19:19:02.821749 findmyorder-1.5.2/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5555 2023-06-26 19:19:02.821749 findmyorder-1.5.2/findmyorder/main.py
--rw-r--r--   0        0        0     2132 2023-06-26 19:19:03.529761 findmyorder-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 findmyorder-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-03 19:54:31.818702 findmyorder-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2262 2023-07-03 19:54:31.818702 findmyorder-1.5.3/README.md
+-rw-r--r--   0        0        0      113 2023-07-03 19:54:32.682752 findmyorder-1.5.3/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-03 19:54:31.818702 findmyorder-1.5.3/findmyorder/config.py
+-rw-r--r--   0        0        0     2848 2023-07-03 19:54:31.818702 findmyorder-1.5.3/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5780 2023-07-03 19:54:31.818702 findmyorder-1.5.3/findmyorder/main.py
+-rw-r--r--   0        0        0     2132 2023-07-03 19:54:32.682752 findmyorder-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 findmyorder-1.5.3/PKG-INFO
```

### Comparing `findmyorder-1.5.2/LICENSE` & `findmyorder-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.2/README.md` & `findmyorder-1.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,60 @@
+Metadata-Version: 2.1
+Name: findmyorder
+Version: 1.5.3
+Summary: A python package to identify and parse order for trade execution.
+License: MIT
+Keywords: trading,order,trade,buy,sell
+Author: mraniki
+Author-email: 8766259+mraniki@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: emoji (>=2.5.1,<3.0.0)
+Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
+Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
+Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
+Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
+Description-Content-Type: text/markdown
+
 # Find my order
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
 |<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![👷‍♂️Flow](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml)  [![codebeat badge](https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a)](https://codebeat.co/projects/github-com-mraniki-findmyorder-main) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
-- Settings for custom option
+- Capability to map a given instrument to a new one (e.g BTC to WBTC or ETHUSD to ETH)
+- Settings for custom options
 
 ## Install
 
 `pip install findmyorder`
 
 ## How to use it
 
-```
+```python
+>>> from findmyorder import FindMyOrder
 fmo = FindMyOrder()
 msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
 order = await fmo.get_order(msg_order)
 #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
 ### Real use case
 
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
+[TalkyTrader](https://github.com/mraniki/tt)
 
 ## Documentation
 
-
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
+
```

### Comparing `findmyorder-1.5.2/findmyorder/config.py` & `findmyorder-1.5.3/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.2/findmyorder/main.py` & `findmyorder-1.5.3/findmyorder/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 from datetime import datetime
 
 import emoji
 from pyparsing import (
     Combine, Optional, Word, alphas,
     nums, one_of, pyparsing_common, Suppress)
-
+from findmyorder import __version__
 from .config import settings
 
 
 class FindMyOrder:
     """find an order class """
 
     def __init__(
@@ -27,15 +27,14 @@
         """Search an order."""
         if my_string:
             string_check = my_string.split()[0].lower()
             if string_check in settings.action_identifier.lower():
                 return True
         return False
 
-
     async def contains_emoji(self, input_string: str) -> bool:
         """Check if the input string contains an emoji."""
         return any(emoji.is_emoji(character) for character in input_string)
 
     async def identify_order(
             self,
             my_string: str,
@@ -107,21 +106,26 @@
             print(settings.instrument_mapping)
             if settings.instrument_mapping:
                 await self.replace_instrument(order)
             return order
         return None
 
     async def replace_instrument(self, order):
+        """ replace instrument by an alternative instrument """
         instrument = order["instrument"]
         for item in settings.mapping:
             if item["id"] == instrument:
                 order["instrument"] = item["alt"]
                 break
         return order
 
+    async def get_info(self):
+        """ get info about the class """
+        return f"{__class__.__name__} {__version__}\n"
+
 # Grammar
 # class TradingGrammar:
 #     def __init__(self):
 #         self.action = self._action()
 #         self.instrument = self._instrument()
 #         self.exchange = self._exchange()
```

### Comparing `findmyorder-1.5.2/pyproject.toml` & `findmyorder-1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.2"
+version = "1.5.3"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.5.2/PKG-INFO` & `findmyorder-1.5.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,38 @@
-Metadata-Version: 2.1
-Name: findmyorder
-Version: 1.5.2
-Summary: A python package to identify and parse order for trade execution.
-License: MIT
-Keywords: trading,order,trade,buy,sell
-Author: mraniki
-Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
-Requires-Dist: emoji (>=2.5.1,<3.0.0)
-Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
-Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
-Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
-Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
-Description-Content-Type: text/markdown
-
 # Find my order
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
 |<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![👷‍♂️Flow](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml)  [![codebeat badge](https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a)](https://codebeat.co/projects/github-com-mraniki-findmyorder-main) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
-- Settings for custom option
+- Capability to map a given instrument to a new one (e.g BTC to WBTC or ETHUSD to ETH)
+- Settings for custom options
 
 ## Install
 
 `pip install findmyorder`
 
 ## How to use it
 
-```
+```python
+>>> from findmyorder import FindMyOrder
 fmo = FindMyOrder()
 msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
 order = await fmo.get_order(msg_order)
 #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 ```
 
 ### Example
 
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
 ### Real use case
 
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
+[TalkyTrader](https://github.com/mraniki/tt)
 
 ## Documentation
 
-
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
-
```

