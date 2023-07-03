# Comparing `tmp/OctoBot-Trading-2.4.4.tar.gz` & `tmp/OctoBot-Trading-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Trading-2.4.4.tar", last modified: Thu Jun  8 21:05:46 2023, max compression
+gzip compressed data, was "OctoBot-Trading-2.4.5.tar", last modified: Mon Jul  3 20:04:11 2023, max compression
```

## Comparing `OctoBot-Trading-2.4.4.tar` & `OctoBot-Trading-2.4.5.tar`

### file list

```diff
@@ -1,573 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    32589 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.719763 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-08 21:05:46.000000 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-06-08 21:05:46.000000 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:05:46.000000 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:05:46.000000 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 21:05:46.000000 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 21:05:46.000000 OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.719763 OctoBot-Trading-2.4.4/octobot_trading/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.719763 OctoBot-Trading-2.4.4/octobot_trading/api/
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/api/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.719763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.719763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/margin_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/exchange_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/funding_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/kline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/kline_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/prices_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.723763 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25402 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/abstract_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/adapters/abstract_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/basic_exchange_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/backtesting_exchange_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/exchange_config_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18004 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    44897 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_websocket_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/exchange_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42921 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/trader_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44555 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/exchange_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/websockets_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/modes/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/channel/abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/channel/abstract_mode_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/channel/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/mode_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/modes_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/modes_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.727764 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/context_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/modes/scripted_trading_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/scripted_trading_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/exchange_personal_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/orders_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/decimal_order_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    41048 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.731763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/sell_market_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/unknown_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/unsupported_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/balance_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/sub_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.735763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/positions_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/active_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/idle_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/liquidate_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/position_state_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/linear_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/trades_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trade_pnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trades_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/fee_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/transfer_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/signals/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/channel/remote_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/channel/signal_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/signal_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/signals/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/abstract_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/candles_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/orders_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/portfolio_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/trades_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/transactions_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/storage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/supervisors/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/supervisors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/supervisors/abstract_portfolio_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/supervisors/abstract_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.739763 OctoBot-Trading-2.4.4/octobot_trading/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/initializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/initialization_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/simulator_updater_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/exchanges_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/websocket_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.719763 OctoBot-Trading-2.4.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/api/test_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/contracts/test_future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/contracts/test_margin_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/funding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/funding/test_funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/kline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/kline/test_kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/test_candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/test_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/order_book/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/order_book/test_order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/prices/test_price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/prices/test_prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/recent_trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/recent_trades/test_recent_trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/test_exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchange_data/ticker/test_ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.743763 OctoBot-Trading-2.4.4/tests/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/implementations/test_default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/implementations/test_default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_abstract_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_basic_exchange_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/test_exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50864 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/traders/test_trader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/types/test_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/util/test_exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/exchanges/util/test_exchange_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/modes/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/script_keywords/basic_keywords/test_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/script_keywords/basic_keywords/test_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/script_keywords/dsl/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/test_abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/modes/test_abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/test_group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_pending_creation_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_decimal_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_double_filled_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/test_orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.747763 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/market/test_buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/market/test_sell_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/test_unknown_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/test_future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/test_margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/test_spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/test_future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/test_margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/test_spot_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/test_position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/test_positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/types/test_inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/positions/types/test_linear_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/trades/test_trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/trades/test_trade_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/trades/test_trade_pnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/transactions/test_transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/personal_data/transactions/test_transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.751763 OctoBot-Trading-2.4.4/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/signals/test_trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/signals/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/test_utils/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/test_utils/random_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests/util/test_config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/tests_additional/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:05:46.755763 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/real_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/real_futures_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bithumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bittrex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bybit_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_coinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_hitbtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_hollaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_ndax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_okcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_okx_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_phemex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_poloniex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_upbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-08 21:04:43.000000 OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_wavesexchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.506185 OctoBot-Trading-2.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.466185 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-03 20:04:11.000000 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-07-03 20:04:11.000000 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:04:11.000000 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:04:11.000000 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-03 20:04:11.000000 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 20:04:11.000000 OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-03 20:04:11.506185 OctoBot-Trading-2.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.466185 OctoBot-Trading-2.4.5/octobot_trading/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/api/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/margin_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/exchange_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/funding_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/kline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/kline_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/prices_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.470185 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/abstract_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/adapters/abstract_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/backtesting_exchange_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/exchange_config_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44886 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_websocket_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/exchange_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.474186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42964 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/trader_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45451 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/exchange_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/websockets_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/modes/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/channel/abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22982 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/channel/abstract_mode_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/channel/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/mode_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/modes_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/modes_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/context_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/modes/scripted_trading_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/scripted_trading_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/exchange_personal_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.478186 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/orders_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/decimal_order_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/sell_market_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/unknown_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/unsupported_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.482185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/balance_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/sub_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/positions_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39334 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/active_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/idle_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/liquidate_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/position_state_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/linear_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/trades_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trade_pnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trades_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.486185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/fee_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/transfer_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/signals/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/channel/remote_trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/channel/signal_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/signal_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/signals/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/abstract_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/candles_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/orders_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/portfolio_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/trades_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/transactions_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/storage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/supervisors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/supervisors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/supervisors/abstract_portfolio_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/supervisors/abstract_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/initializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/initialization_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/simulator_updater_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/exchanges_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/websocket_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:04:11.506185 OctoBot-Trading-2.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.466185 OctoBot-Trading-2.4.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/api/test_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.490185 OctoBot-Trading-2.4.5/tests/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/contracts/test_future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/contracts/test_margin_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/funding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/funding/test_funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/kline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/kline/test_kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/test_candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/test_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/order_book/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/order_book/test_order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/prices/test_price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/prices/test_prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/recent_trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/recent_trades/test_recent_trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/test_exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchange_data/ticker/test_ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/implementations/test_default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/implementations/test_default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_abstract_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/test_exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50875 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/traders/test_trader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/types/test_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/util/test_exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/exchanges/util/test_exchange_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.494185 OctoBot-Trading-2.4.5/tests/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/script_keywords/basic_keywords/test_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/script_keywords/basic_keywords/test_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/script_keywords/dsl/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/test_abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/modes/test_abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/test_group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_pending_creation_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_decimal_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_double_filled_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/test_orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/market/test_buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/market/test_sell_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/test_unknown_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.498185 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/test_future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/test_margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/test_spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/test_future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/test_margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/test_spot_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/test_position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/test_positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/types/test_inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/positions/types/test_linear_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/trades/test_trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/trades/test_trade_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/trades/test_trade_pnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/transactions/test_transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/personal_data/transactions/test_transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/signals/test_trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/signals/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/test_utils/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/test_utils/random_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests/util/test_config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.502185 OctoBot-Trading-2.4.5/tests_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:04:11.506185 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/real_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/real_futures_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_binance_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bithumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitstamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bittrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bybit_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_coinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_hitbtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_hollaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_ndax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_okcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_okx_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_phemex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_poloniex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_upbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-03 20:03:19.000000 OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_wavesexchange.py
```

### Comparing `OctoBot-Trading-2.4.4/CHANGELOG.md` & `OctoBot-Trading-2.4.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.4.5] - 2023-07-03
+### Added
+- Full stop loss support for supporting exchanges
+- Binance futures support
+- MEXC support
+### Updated
+- Improved futures trading related error messages
+- Position and orders update request policy: now retry once before giving up and falling back to the next update cycle
+- Improved orders logs
+### Fixed
+- Positions sync issues when order are instantly filled
+- Positions duplicate issues
+- Futures trading non-future symbols related errors
+- Decimal division by zero error when building signals
+
 ## [2.4.4] - 2023-06-08
 ### Fixed
 - Orders sync issues
 - Order sizing issues when using % param
 
 ## [2.4.3] - 2023-05-12
 ### Updated
```

### Comparing `OctoBot-Trading-2.4.4/LICENSE` & `OctoBot-Trading-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/PKG-INFO` & `OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.4
+Version: 2.4.5
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.4](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.5](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.4/OctoBot_Trading.egg-info/SOURCES.txt` & `OctoBot-Trading-2.4.5/OctoBot_Trading.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
 octobot_trading/exchange_data/ticker/channel/__init__.py
 octobot_trading/exchange_data/ticker/channel/ticker.py
 octobot_trading/exchange_data/ticker/channel/ticker_updater.py
 octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
 octobot_trading/exchanges/__init__.py
 octobot_trading/exchanges/abstract_exchange.py
 octobot_trading/exchanges/abstract_websocket_exchange.py
-octobot_trading/exchanges/basic_exchange_wrapper.py
 octobot_trading/exchanges/exchange_builder.py
 octobot_trading/exchanges/exchange_channels.py
+octobot_trading/exchanges/exchange_details.py
 octobot_trading/exchanges/exchange_factory.py
 octobot_trading/exchanges/exchange_manager.py
 octobot_trading/exchanges/exchange_websocket_factory.py
 octobot_trading/exchanges/exchanges.py
 octobot_trading/exchanges/adapters/__init__.py
 octobot_trading/exchanges/adapters/abstract_adapter.py
 octobot_trading/exchanges/config/__init__.py
@@ -313,15 +313,14 @@
 tests/exchange_data/recent_trades/__init__.py
 tests/exchange_data/recent_trades/test_recent_trades_manager.py
 tests/exchange_data/ticker/__init__.py
 tests/exchange_data/ticker/test_ticker_manager.py
 tests/exchanges/__init__.py
 tests/exchanges/test_abstract_exchange.py
 tests/exchanges/test_abstract_websocket_exchange.py
-tests/exchanges/test_basic_exchange_wrapper.py
 tests/exchanges/test_exchange_builder.py
 tests/exchanges/test_exchange_config_data.py
 tests/exchanges/test_exchange_factory.py
 tests/exchanges/test_exchange_manager.py
 tests/exchanges/test_exchange_simulator.py
 tests/exchanges/test_exchanges.py
 tests/exchanges/connectors/__init__.py
@@ -428,14 +427,15 @@
 tests/util/test_config_util.py
 tests_additional/__init__.py
 tests_additional/real_exchanges/__init__.py
 tests_additional/real_exchanges/real_exchange_tester.py
 tests_additional/real_exchanges/real_futures_exchange_tester.py
 tests_additional/real_exchanges/test_ascendex.py
 tests_additional/real_exchanges/test_binance.py
+tests_additional/real_exchanges/test_binance_futures.py
 tests_additional/real_exchanges/test_bitfinex.py
 tests_additional/real_exchanges/test_bitget.py
 tests_additional/real_exchanges/test_bithumb.py
 tests_additional/real_exchanges/test_bitso.py
 tests_additional/real_exchanges/test_bitstamp.py
 tests_additional/real_exchanges/test_bittrex.py
 tests_additional/real_exchanges/test_bybit.py
@@ -447,14 +447,15 @@
 tests_additional/real_exchanges/test_hitbtc.py
 tests_additional/real_exchanges/test_hollaex.py
 tests_additional/real_exchanges/test_huobi.py
 tests_additional/real_exchanges/test_huobipro.py
 tests_additional/real_exchanges/test_kraken.py
 tests_additional/real_exchanges/test_kucoin.py
 tests_additional/real_exchanges/test_kucoin_futures.py
+tests_additional/real_exchanges/test_mexc.py
 tests_additional/real_exchanges/test_ndax.py
 tests_additional/real_exchanges/test_okcoin.py
 tests_additional/real_exchanges/test_okx.py
 tests_additional/real_exchanges/test_okx_futures.py
 tests_additional/real_exchanges/test_phemex.py
 tests_additional/real_exchanges/test_poloniex.py
 tests_additional/real_exchanges/test_upbit.py
```

### Comparing `OctoBot-Trading-2.4.4/PKG-INFO` & `OctoBot-Trading-2.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.4
+Version: 2.4.5
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.4](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.5](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.4/README.md` & `OctoBot-Trading-2.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Trading [2.4.4](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.5](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Trading"
-VERSION = "2.4.4"  # major.minor.revision
+VERSION = "2.4.5"  # major.minor.revision
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     has_only_ohlcv,
     get_is_backtesting,
     get_backtesting_data_files,
     get_backtesting_data_file,
     get_has_websocket,
     supports_websockets,
     is_compatible_account,
+    get_new_ccxt_client,
     get_default_exchange_type,
     is_sponsoring,
     is_valid_account,
     get_historical_ohlcv,
     get_bot_id,
     get_supported_exchange_types,
     get_trading_pairs,
@@ -110,14 +111,16 @@
     get_fees,
     get_max_handled_pair_with_time_frame,
     get_currently_handled_pair_with_time_frame,
     get_required_historical_candles_count,
     is_overloaded,
     store_history_in_run_storage,
     get_enabled_exchanges_names,
+    get_auto_filled_exchange_names,
+    get_exchange_details,
     cancel_ccxt_throttle_task,
     stop_exchange,
 )
 from octobot_trading.api.modes import (
     get_trading_modes,
     get_trading_mode_symbol,
     get_trading_mode_followed_strategy_signals_identifier,
@@ -256,14 +259,15 @@
     "has_only_ohlcv",
     "get_is_backtesting",
     "get_backtesting_data_files",
     "get_backtesting_data_file",
     "get_has_websocket",
     "supports_websockets",
     "is_compatible_account",
+    "get_new_ccxt_client",
     "get_default_exchange_type",
     "is_sponsoring",
     "is_valid_account",
     "get_historical_ohlcv",
     "get_bot_id",
     "get_supported_exchange_types",
     "get_trading_pairs",
@@ -277,14 +281,16 @@
     "get_fees",
     "get_max_handled_pair_with_time_frame",
     "get_currently_handled_pair_with_time_frame",
     "get_required_historical_candles_count",
     "is_overloaded",
     "store_history_in_run_storage",
     "get_enabled_exchanges_names",
+    "get_auto_filled_exchange_names",
+    "get_exchange_details",
     "cancel_ccxt_throttle_task",
     "stop_exchange",
     "get_trading_modes",
     "get_trading_mode_symbol",
     "get_trading_mode_followed_strategy_signals_identifier",
     "get_trading_mode_current_state",
     "get_activated_trading_mode",
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/channels.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/contracts.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/contracts.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
+import contextlib
+
 import trading_backend
 
 import octobot_trading.constants
 import octobot_trading.enums
 import octobot_trading.exchanges.connectors.ccxt.enums
 import octobot_trading.exchanges as exchanges
 import octobot_trading.exchange_data as exchange_data
@@ -40,30 +42,28 @@
 
 def get_exchange_manager_from_exchange_name_and_id(exchange_name: str, exchange_id: str) -> object:
     return exchanges.Exchanges.instance().get_exchange(exchange_name, exchange_id).exchange_manager
 
 
 async def get_ccxt_exchange_available_time_frames(
         exchange_name: str,
-        exchange_lib: octobot_trading.exchanges.connectors.ccxt.enums.ExchangeWrapperLibs =
-        octobot_trading.exchanges.connectors.ccxt.enums.ExchangeWrapperLibs.CCXT
+        tentacles_setup_config
 ) -> list:
     """
     When using CCXT, prefer using the sync lib since no request is required to get time frames
     :param exchange_name: name of the exchange
-    :param exchange_lib: octobot_trading.exchanges.connectors.ccxt.enums.ExchangeWrapperLibs to use
     :return: the list of time frames
     """
     try:
         # first try in available exchanges
         for exchange_configuration in get_exchange_configurations_from_exchange_name(exchange_name).values():
             return exchange_configuration.exchange_manager.client_time_frames
     except KeyError:
-        async with exchanges.temporary_exchange_wrapper(exchange_name, exchange_lib) as wrapper:
-            return list(await wrapper.get_available_time_frames())
+        async with get_new_ccxt_client(exchange_name, {}, tentacles_setup_config, False) as ccxt_exchange:
+            return ccxt_exchange.timeframes
 
 
 def get_exchange_available_required_time_frames(exchange_name: str, exchange_id: str) -> list:
     return exchanges.Exchanges.instance().get_exchange(exchange_name, exchange_id).available_required_time_frames
 
 
 # prefer get_exchange_configurations_from_exchange_name when possible
@@ -259,14 +259,22 @@
 
 
 async def is_compatible_account(exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool) \
         -> (bool, bool, str):
     return await exchanges.is_compatible_account(exchange_name, exchange_config, tentacles_setup_config, is_sandboxed)
 
 
+@contextlib.asynccontextmanager
+async def get_new_ccxt_client(exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool):
+    async with exchanges.get_local_exchange_manager(
+        exchange_name, exchange_config, tentacles_setup_config, is_sandboxed, ignore_config=True
+    ) as local_exchange_manager:
+        yield local_exchange_manager.exchange.connector.client
+
+
 def get_default_exchange_type(exchange_name: str) -> str:
     return exchanges.get_default_exchange_type(exchange_name)
 
 
 def is_sponsoring(exchange_name: str) -> bool:
     return trading_backend.is_sponsoring(exchange_name)
 
@@ -284,24 +292,36 @@
     )
 
 
 def get_bot_id(exchange_manager):
     return exchange_manager.bot_id
 
 
-def get_supported_exchange_types(exchange_name) -> list:
-    return exchanges.get_supported_exchange_types(exchange_name)
+def get_supported_exchange_types(exchange_name, tentacles_setup_config) -> list:
+    return exchanges.get_supported_exchange_types(exchange_name, tentacles_setup_config)
 
 
 async def store_history_in_run_storage(exchange_manager):
     await exchange_manager.storage_manager.store_history()
 
 
 def get_enabled_exchanges_names(config) -> list:
     return exchanges.get_enabled_exchanges(config)
 
 
+def get_auto_filled_exchange_names(tentacles_setup_config) -> list:
+    return exchanges.get_auto_filled_exchange_names(tentacles_setup_config)
+
+
+async def get_exchange_details(
+    exchange_name, is_autofilled, tentacles_setup_config, aiohttp_session
+) -> exchanges.ExchangeDetails:
+    return await exchanges.get_exchange_details(
+        exchange_name, is_autofilled, tentacles_setup_config, aiohttp_session
+    )
+
+
 def cancel_ccxt_throttle_task():
     for task in asyncio.all_tasks():
         # manually cancel ccxt async throttle task since it apparently can't be cancelled otherwise
         if str(task._coro).startswith("<coroutine object Throttler.looper at"):
             task.cancel()
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/modes.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/orders.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/portfolio.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/positions.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/profitability.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/symbol_data.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/trader.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/api/trades.py` & `OctoBot-Trading-2.4.5/octobot_trading/api/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/constants.py` & `OctoBot-Trading-2.4.5/octobot_trading/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 
 # exchanges where test_get_historical_symbol_prices is successful can be listed here
 FULL_CANDLE_HISTORY_EXCHANGES = [
     "ascendex",
     "binance",
     "bitfinex2",
     "bitstamp",
-    "bittrex",
     "bybit",
     "gateio",
     "hitbtc",
     "hollaex",
     "huobi",
     "huobipro",
     "kucoin",
@@ -97,14 +96,15 @@
     "ascendex",
     "kucoin",
     "coinbase",
     "bybit",
     "cryptocom",
     "phemex",
     "hollaex",
+    "mexc",
 ]
 DEFAULT_FUTURE_EXCHANGES = ["binanceusdm", "bybit"]
 SIMULATOR_TESTED_EXCHANGES = ["bitfinex2", "bithumb", "bitstamp", "bittrex", "coinex",
                               "hitbtc", "kraken", "poloniex", "bitso", "ndax", "upbit",
                               "wavesexchange"]
 
 CONFIG_DEFAULT_FEES = 0.001
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/enums.py` & `OctoBot-Trading-2.4.5/octobot_trading/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,7 +562,12 @@
 
 
 class OrderUpdateType(enum.Enum):
     NEW = "new"
     CLOSED = "closed"
     EDIT = "edit"
     STATE_CHANGE = "state_transition"
+
+
+class ExchangeSupportedElements(enum.Enum):
+    UNSUPPORTED_ORDERS = "unsupported_orders"
+    SUPPORTED_BUNDLED_ORDERS = "supported_bundled_orders"
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/errors.py` & `OctoBot-Trading-2.4.5/octobot_trading/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_channel.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/contract_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/future_contract.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/contracts/margin_contract.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/contracts/margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/exchange_symbol_data.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/exchange_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/exchange_symbols_data.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/funding.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/funding.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/funding_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/funding_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 import typing
 
 import octobot_commons.async_job as async_job
 import octobot_commons.constants as common_constants
-import octobot_commons.symbols as common_symbols
 
 import octobot_trading.exchange_data.funding.channel.funding as funding_channel
 import octobot_trading.exchanges.exchange_websocket_factory as exchange_websocket_factory
 import octobot_trading.constants as constants
 import octobot_trading.enums as enums
 import octobot_trading.errors as errors
 
@@ -75,16 +74,14 @@
 
         await self.initialize()
         await self.fetch_funding_job.run()
 
     async def _funding_fetch_and_push(self) -> list:
         next_funding_times = []
         for pair in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
-            if not common_symbols.parse_symbol(pair).is_future():
-                continue
             next_funding_time_candidate = await self.fetch_symbol_funding_rate(pair)
             if next_funding_time_candidate is not None:
                 next_funding_times.append(next_funding_time_candidate)
         return next_funding_times
 
     async def fetch_symbol_funding_rate(self, symbol: str) -> typing.Optional[int]:
         """
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/funding/funding_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/funding/funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/kline.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/kline.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/kline_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/kline_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/kline/kline_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/kline/kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/candles_adapter.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/candles_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/order_book.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/order_book.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/order_book_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/order_book_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/order_book/order_book_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/order_book/order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/price.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/price.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/prices_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/prices_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/price_events_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/prices/prices_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/prices/prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/ticker.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/ticker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/ticker_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/ticker_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchange_data/ticker/ticker_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchange_data/ticker/ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,20 +36,14 @@
 )
 
 from octobot_trading.exchanges import abstract_websocket_exchange
 from octobot_trading.exchanges.abstract_websocket_exchange import (
     AbstractWebsocketExchange,
 )
 
-from octobot_trading.exchanges import basic_exchange_wrapper
-from octobot_trading.exchanges.basic_exchange_wrapper import (
-    BasicExchangeWrapper,
-    temporary_exchange_wrapper,
-)
-
 from octobot_trading.exchanges import exchange_manager
 from octobot_trading.exchanges.exchange_manager import (
     ExchangeManager,
 )
 
 from octobot_trading.exchanges import exchange_factory
 from octobot_trading.exchanges.exchange_factory import (
@@ -72,14 +66,17 @@
     get_exchange_type,
     get_default_exchange_type,
     get_supported_exchange_types,
     update_raw_order_from_raw_trade,
     is_missing_trading_fees,
     apply_trades_fees,
     get_exchange_class_from_name,
+    get_local_exchange_manager,
+    get_auto_filled_exchange_names,
+    get_exchange_details,
     force_disable_web_socket,
     check_web_socket_config,
     search_websocket_class,
     supports_websocket,
 )
 from octobot_trading.exchanges import exchange_websocket_factory
 from octobot_trading.exchanges.exchange_websocket_factory import (
@@ -118,14 +115,18 @@
 from octobot_trading.exchanges.connectors import (
     CCXTWebsocketConnector,
     CCXTConnector,
     CCXTAdapter,
     ExchangeSimulatorConnector,
     ExchangeSimulatorAdapter,
 )
+from octobot_trading.exchanges import exchange_details
+from octobot_trading.exchanges.exchange_details import (
+    ExchangeDetails,
+)
 
 __all__ = [
     "AbstractAdapter",
     "ExchangeConfig",
     "BacktestingExchangeConfig",
     "ExchangeManager",
     "ExchangeBuilder",
@@ -147,14 +148,17 @@
     "get_exchange_type",
     "get_default_exchange_type",
     "get_supported_exchange_types",
     "update_raw_order_from_raw_trade",
     "is_missing_trading_fees",
     "apply_trades_fees",
     "get_exchange_class_from_name",
+    "get_local_exchange_manager",
+    "get_auto_filled_exchange_names",
+    "get_exchange_details",
     "AbstractExchange",
     "is_channel_managed_by_websocket",
     "is_channel_fully_managed_by_websocket",
     "is_websocket_feed_requiring_init",
     "search_and_create_websocket",
     "requires_refresh_trigger",
     "create_exchange_channels",
@@ -167,18 +171,17 @@
     "ExchangeSimulator",
     "CCXTWebsocketConnector",
     "WebSocketExchange",
     "RestExchange",
     "ExchangeMarketStatusFixer",
     "is_ms_valid",
     "AbstractWebsocketExchange",
-    "BasicExchangeWrapper",
-    "temporary_exchange_wrapper",
     "force_disable_web_socket",
     "check_web_socket_config",
     "search_websocket_class",
     "supports_websocket",
     "CCXTConnector",
     "CCXTAdapter",
     "ExchangeSimulatorConnector",
     "ExchangeSimulatorAdapter",
+    "ExchangeDetails",
 ]
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/abstract_exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/abstract_exchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,31 +30,49 @@
 
 
 class AbstractExchange(tentacles_management.AbstractTentacle):
     USER_INPUT_TENTACLE_TYPE = common_enums.UserInputTentacleTypes.EXCHANGE
     BUY_STR = enums.TradeOrderSide.BUY.value
     SELL_STR = enums.TradeOrderSide.SELL.value
 
-    # order that should be self-managed by OctoBot
-    # can be overridden locally to match exchange support
-    UNSUPPORTED_ORDERS = [
-        enums.TraderOrderType.STOP_LOSS,
-        enums.TraderOrderType.STOP_LOSS_LIMIT,
-        enums.TraderOrderType.TAKE_PROFIT,
-        enums.TraderOrderType.TAKE_PROFIT_LIMIT,
-        enums.TraderOrderType.TRAILING_STOP,
-        enums.TraderOrderType.TRAILING_STOP_LIMIT
-    ]
-
-    # order that can be bundled together to create them all in one request
-    # format: dict of bundled types by base order type
-    # ex: SUPPORTED_BUNDLED_ORDERS[enums.TraderOrderType.BUY_MARKET] = \
-    # [enums.TraderOrderType.STOP_LOSS, enums.TraderOrderType.TAKE_PROFIT]
-    # can be overridden locally to match exchange support
-    SUPPORTED_BUNDLED_ORDERS = {}
+    # should be overridden locally to match exchange support
+    SUPPORTED_ELEMENTS = {
+        enums.ExchangeTypes.FUTURE.value: {
+            # order that should be self-managed by OctoBot
+            enums.ExchangeSupportedElements.UNSUPPORTED_ORDERS.value: [
+                enums.TraderOrderType.STOP_LOSS,
+                enums.TraderOrderType.STOP_LOSS_LIMIT,
+                enums.TraderOrderType.TAKE_PROFIT,
+                enums.TraderOrderType.TAKE_PROFIT_LIMIT,
+                enums.TraderOrderType.TRAILING_STOP,
+                enums.TraderOrderType.TRAILING_STOP_LIMIT
+            ],
+            # order that can be bundled together to create them all in one request
+            # format: dict of bundled types by base order type
+            # ex: SUPPORTED_BUNDLED_ORDERS[enums.TraderOrderType.BUY_MARKET] = \
+            # [enums.TraderOrderType.STOP_LOSS, enums.TraderOrderType.TAKE_PROFIT]
+            enums.ExchangeSupportedElements.SUPPORTED_BUNDLED_ORDERS.value: {},
+        },
+        enums.ExchangeTypes.SPOT.value: {
+            # order that should be self-managed by OctoBot
+            enums.ExchangeSupportedElements.UNSUPPORTED_ORDERS.value: [
+                enums.TraderOrderType.STOP_LOSS,
+                enums.TraderOrderType.STOP_LOSS_LIMIT,
+                enums.TraderOrderType.TAKE_PROFIT,
+                enums.TraderOrderType.TAKE_PROFIT_LIMIT,
+                enums.TraderOrderType.TRAILING_STOP,
+                enums.TraderOrderType.TRAILING_STOP_LIMIT
+            ],
+            # order that can be bundled together to create them all in one request
+            # format: dict of bundled types by base order type
+            # ex: SUPPORTED_BUNDLED_ORDERS[enums.TraderOrderType.BUY_MARKET] = \
+            # [enums.TraderOrderType.STOP_LOSS, enums.TraderOrderType.TAKE_PROFIT]
+            enums.ExchangeSupportedElements.SUPPORTED_BUNDLED_ORDERS.value: {},
+        }
+    }
     ACCOUNTS = {}
 
     def __init__(self, config, exchange_manager):
         super().__init__()
         self.config = config
         self.exchange_manager = exchange_manager
         self.connector = None
@@ -148,14 +166,22 @@
         WARNING: does not check if the timestamp is already in the right form, better using get_uniformized_timestamp
         to be sure to keep the right format and uniformize if necessary only
         :param timestamp: the timestamp to uniformize
         :return: the uniformized timestamp
         """
         raise NotImplementedError("get_uniform_timestamp not implemented")
 
+    def get_supported_elements(self, element_key: enums.ExchangeSupportedElements):
+        """
+        :return: the supported elements such as order type and bundle orders for the current exchange and trading type
+        """
+        exchange_type_key = enums.ExchangeTypes.FUTURE if self.exchange_manager.is_future \
+            else enums.ExchangeTypes.SPOT
+        return self.__class__.SUPPORTED_ELEMENTS[exchange_type_key.value][element_key.value]
+
     def get_market_status(self, symbol, price_example=None, with_fixer=True):
         """
         Return the market status
         :param symbol: the symbol
         :param price_example: a price example to be used in MarketStatusFixer
         :param with_fixer: when True, return a new instance of MarketStatusFixer
         :return: market status dict
@@ -332,15 +358,17 @@
         the same time as a buy order)
         :param base_order: the first order of the combo
         :param bundled_order_type: the type of the order that we try to bundle with base_order
         :return: True if an order of type tied_order_type can be pushed alongside base_order to the exchange
         in one request
         """
         try:
-            return bundled_order_type in self.SUPPORTED_BUNDLED_ORDERS[base_order.order_type]
+            return bundled_order_type in self.get_supported_elements(
+                enums.ExchangeSupportedElements.SUPPORTED_BUNDLED_ORDERS
+            )[base_order.order_type]
         except KeyError:
             return False
 
     def get_bundled_order_parameters(self, order, stop_loss_price=None, take_profit_price=None) -> dict:
         """
         Returns the updated params when this exchange supports orders created upon other orders fill
         (ex: a stop loss created at the same time as a buy order)
@@ -355,15 +383,15 @@
     def is_supported_order_type(self, order_type):
         """
         Check if the order type is supported by the current exchange instance
         Should be used to know if we should simulate this order or create it on the exchange
         :param order_type: the order type, should be a member of enums.TraderOrderType
         :return: True if the order type is supported by the exchange, else False
         """
-        return order_type not in self.UNSUPPORTED_ORDERS
+        return order_type not in self.get_supported_elements(enums.ExchangeSupportedElements.UNSUPPORTED_ORDERS)
 
     def get_trade_fee(self, symbol, order_type, quantity, price, taker_or_maker):
         """
         Calculates fees resulting to a trade
         :param symbol: the symbol
         :param order_type: the order type
         :param quantity: the trade quantity
@@ -430,18 +458,24 @@
     async def get_sub_account_list(self):
         """
         :return: the exchange sub account list if supported by the exchange
         """
         raise NotImplementedError("get_sub_account_list is not available on this exchange")
 
     async def retry_till_success(self, timeout, request_func, *args, **kwargs):
+        return await self._retry_until(timeout, 0, request_func, *args, **kwargs)
+
+    async def retry_n_time(self, n_times, request_func, *args, **kwargs):
+        return await self._retry_until(0, n_times, request_func, *args, **kwargs)
+
+    async def _retry_until(self, timeout, n_times, request_func, *args, **kwargs):
         t0 = time.time()
         minimal_interval = 0.1
         attempt = 1
-        while time.time() - t0 < timeout:
+        while (timeout != 0 and time.time() - t0 < timeout) or (n_times != 0 and attempt <= n_times + 1):
             last_request_time = time.time()
             try:
                 result = await request_func(*args, **kwargs)
                 if attempt > 1:
                     self.logger.debug(f"Request retrier success for {request_func.__name__} after {attempt} attempts")
                 return result
             except errors.FailedRequest:
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/abstract_websocket_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,18 @@
         self.time_frames = []
         self.channels = []
 
         self.books = {}
 
         self.client = None
         self.name = self.get_name()
-        self.logger = logging.get_logger(f"WebSocket - {self.name}")
+        self.logger = logging.get_logger(self._get_logger_name())
+
+    def _get_logger_name(self):
+        return f"WebSocket - {self.name}"
 
     def initialize(self, currencies=None, pairs=None, time_frames=None, channels=None):
         self.pairs = [self.get_exchange_pair(pair) for pair in pairs] if pairs else []
         # inner list required for cythonization
         self.channels = list(set([self.feed_to_exchange(channel) for channel in channels])) if channels else []
         self.time_frames = [
             time_frame
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/adapters/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/adapters/abstract_adapter.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/adapters/abstract_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
             if args[1] is None:
                 # element to adapt is None, no need to go any further
                 return None
             adapted = func(*args, **kwargs)
             # add any other common adapter function logic here
             return adapted
         except Exception as err:
-            raise errors.UnexpectedAdapterError(f"Unexpected error when adapting exchange data: {err}") from err
+            raise errors.UnexpectedAdapterError(
+                f"Unexpected error when adapting exchange data: {err} (data: {args[1]})"
+            ) from err
     return wrapper
 
 
 class AbstractAdapter:
     def __init__(self, connector):
         self.logger = logging.get_logger(self.__class__.__name__)
         self.connector = connector
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/backtesting_exchange_config.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/backtesting_exchange_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/config/exchange_config_data.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/config/exchange_config_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 import octobot_commons.logging as logging
 import octobot_commons.errors as errors
 import octobot_commons.enums as commons_enums
 import octobot_commons.tree as commons_tree
 
 import octobot_trading.exchange_channel as exchange_channel
 import octobot_trading.exchanges.config.backtesting_exchange_config as backtesting_exchange_config
+import octobot_trading.exchanges.util as exchange_util
 import octobot_trading.constants as trading_constants
+import octobot_trading.enums as trading_enums
 import octobot_trading.util as util
 
 
 class ExchangeConfig(util.Initializable):
     def __init__(self, exchange_manager):
         super().__init__()
         self._logger = logging.get_logger(self.__class__.__name__)
@@ -200,35 +202,52 @@
                                    f"OctoBot requires at least one trading pair in configuration to handle an asset. "
                                    f"You can add trading pair(s) for each asset in the configuration section.")
         except errors.ConfigError as err:
             self._logger.error(str(err))
         return traded_symbol_pairs_set
 
     def _populate_non_wildcard_pairs(self, cryptocurrency, existing_pairs, is_enabled):
+        exchange_type = exchange_util.get_exchange_type(self.exchange_manager)
         if self.config[constants.CONFIG_CRYPTO_CURRENCIES][cryptocurrency][constants.CONFIG_CRYPTO_PAIRS] != \
                 constants.CONFIG_SYMBOLS_WILDCARD:
             currency_pairs = []
             for symbol in self.config[constants.CONFIG_CRYPTO_CURRENCIES][cryptocurrency][
-                constants.CONFIG_CRYPTO_PAIRS]:
-                if self.exchange_manager.symbol_exists(symbol):
-                    if is_enabled:
-                        currency_pairs.append(symbol)
-                    # also add disabled pairs to existing pairs since they still exist on exchange
-                    existing_pairs.add(symbol)
-                elif is_enabled:
-                    additional_details = ""
-                    if self.exchange_manager.is_sandboxed:
-                        additional_details = f" Exchange sandbox is enabled, please make sure this pair is traded on " \
-                                             f" the {self.exchange_manager.exchange_name} sandbox as sandboxes " \
-                                             f"usually only support a subset of the real exchange's pairs."
-                    self._logger.error(f"{self.exchange_manager.exchange_name} is not supporting the "
-                                       f"{symbol} trading pair.{additional_details}")
+               constants.CONFIG_CRYPTO_PAIRS]:
+                self._add_compatible_pairs(currency_pairs, symbol, existing_pairs, is_enabled, exchange_type)
             if is_enabled:
                 self.traded_cryptocurrencies[cryptocurrency] = currency_pairs
 
+    def _add_compatible_pairs(self, currency_pairs, symbol, existing_pairs, is_enabled, exchange_type):
+        if self.exchange_manager.symbol_exists(symbol):
+            if is_enabled:
+                if self._is_pair_compatible(exchange_type, symbol):
+                    currency_pairs.append(symbol)
+                else:
+                    self._logger.warning(f"Ignored {symbol} trading pair: only {exchange_type.value} "
+                                         f"pairs are allowed on {self.exchange_manager.exchange_name} when "
+                                         f"using {exchange_type.value} trading")
+            # also add disabled pairs to existing pairs since they still exist on exchange
+            existing_pairs.add(symbol)
+        elif is_enabled:
+            additional_details = ""
+            if self.exchange_manager.is_sandboxed:
+                additional_details = f" Exchange sandbox is enabled, please make sure this pair is traded on " \
+                                     f" the {self.exchange_manager.exchange_name} sandbox as sandboxes " \
+                                     f"usually only support a subset of the real exchange's pairs."
+            self._logger.error(f"{self.exchange_manager.exchange_name} is not supporting the "
+                               f"{symbol} trading pair.{additional_details}")
+
+    @staticmethod
+    def _is_pair_compatible(exchange_type, symbol):
+        parsed_symbol = octobot_commons.symbols.parse_symbol(symbol)
+        if exchange_type is trading_enums.ExchangeTypes.FUTURE:
+            return parsed_symbol.is_future()
+        # allow futures symbols for spot
+        return True
+
     def _populate_wildcard_pairs(self, cryptocurrency, existing_pairs, is_enabled):
         try:
             wildcard_pairs_list = self._create_wildcard_symbol_list(self.config[constants.CONFIG_CRYPTO_CURRENCIES]
                                                                     [cryptocurrency][constants.CONFIG_CRYPTO_QUOTE])
         except KeyError as e:
             raise errors.ConfigError(f"Impossible to use a wildcard configuration for {cryptocurrency}: missing {e} "
                                      f"value in {cryptocurrency} {constants.CONFIG_CRYPTO_CURRENCIES} "
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,27 +193,28 @@
         #     if side == enums.PositionSide.LONG.value else enums.PositionSide.
         symbol = fixed.get(ccxt_enums.ExchangePositionCCXTColumns.SYMBOL.value)
         contract_size = decimal.Decimal(str(fixed.get(ccxt_enums.ExchangePositionCCXTColumns.CONTRACT_SIZE.value, 0)))
         contracts = constants.ZERO if force_empty \
             else decimal.Decimal(str(fixed.get(ccxt_enums.ExchangePositionCCXTColumns.CONTRACTS.value, 0)))
         is_empty = contracts == constants.ZERO
         liquidation_price = fixed.get(ccxt_enums.ExchangePositionCCXTColumns.LIQUIDATION_PRICE.value, 0)
+        if margin_type := fixed.get(ccxt_enums.ExchangePositionCCXTColumns.MARGIN_TYPE.value, None):
+            margin_type = enums.MarginType(margin_type)
         if force_empty or liquidation_price is None:
             liquidation_price = constants.NaN
         else:
             liquidation_price = decimal.Decimal(str(liquidation_price))
         try:
             fixed.update({
                 enums.ExchangeConstantsPositionColumns.SYMBOL.value: symbol,
                 enums.ExchangeConstantsPositionColumns.TIMESTAMP.value:
                     fixed.get(ccxt_enums.ExchangePositionCCXTColumns.TIMESTAMP.value,
                               self.connector.get_exchange_current_time()),
                 enums.ExchangeConstantsPositionColumns.SIDE.value: position_side,
-                enums.ExchangeConstantsPositionColumns.MARGIN_TYPE.value:
-                    fixed.get(ccxt_enums.ExchangePositionCCXTColumns.MARGIN_TYPE.value, None),
+                enums.ExchangeConstantsPositionColumns.MARGIN_TYPE.value: margin_type,
                 enums.ExchangeConstantsPositionColumns.SIZE.value:
                     contract_size * contracts if original_side == enums.PositionSide.LONG.value
                     else -contract_size * contracts,
                 enums.ExchangeConstantsPositionColumns.CONTRACT_TYPE.value:
                     self.connector.exchange_manager.exchange.get_contract_type(symbol),
                 enums.ExchangeConstantsPositionColumns.LEVERAGE.value:
                     self.safe_decimal(fixed, ccxt_enums.ExchangePositionCCXTColumns.LEVERAGE.value,
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 
 import octobot_commons.time_frame_manager as time_frame_manager
 import octobot_trading.constants as constants
 import octobot_trading.exchanges.connectors.ccxt.enums as ccxt_enums
 import octobot_trading.exchanges.util.exchange_util as exchange_util
 
 
-def create_client(exchange_class, exchange_name, exchange_manager, logger, 
+def create_client(exchange_class, exchange_manager, logger,
                   options, headers, additional_config, 
                   should_authenticate, unauthenticated_exchange_fallback=None):
     """
     Exchange instance creation
     :return: the created ccxt (pro, async or sync) client
     """
     is_authenticated = False
     if not exchange_manager.exchange_only:
         # avoid logging version on temporary exchange_only exchanges
         exchange_type = exchange_util.get_exchange_type(exchange_manager)
         logger.info(f"Creating {exchange_class.__name__} {exchange_type.name} "
                     f"exchange with ccxt in version {ccxt.__version__}")
-    if exchange_manager.ignore_config or exchange_manager.check_config(exchange_name):
+    if exchange_manager.ignore_config or exchange_manager.check_config(exchange_manager.exchange_name):
         try:
-            key, secret, password = exchange_manager.get_exchange_credentials(exchange_name)
-            if not (key and secret) and not exchange_manager.is_simulated:
+            key, secret, password = exchange_manager.get_exchange_credentials(exchange_manager.exchange_name)
+            if not (key and secret) and not exchange_manager.is_simulated and not exchange_manager.ignore_config:
                 logger.warning(f"No exchange API key set for {exchange_manager.exchange_name}. "
                                f"Enter your account details to enable real trading on this exchange.")
             if should_authenticate:
                 client = exchange_class(_get_client_config(options, headers, additional_config,
                                                            key, secret, password))
                 is_authenticated = True
                 if exchange_manager.check_credentials:
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Uses self.adapter to parse (and fix if necessary) ccxt raw data.
 
     Always returns adapted data. Always throws octobot_trading errors
     Never returns row ccxt data or throw ccxt errors
     """
 
     def __init__(
-            self, config, exchange_manager, adapter_class=None, additional_config=None, rest_name=None, force_auth=False
+        self, config, exchange_manager, adapter_class=None, additional_config=None, rest_name=None, force_auth=False
     ):
         super().__init__(config, exchange_manager)
         self.client = None
         self.exchange_type = None
         self.adapter = self.get_adapter_class(adapter_class)(self)
         self.all_currencies_price_ticker = None
         self.is_authenticated = False
@@ -78,15 +78,16 @@
         self._create_exchange_type()
         self._create_client()
 
     async def initialize_impl(self):
         try:
             if self.exchange_manager.exchange.is_supporting_sandbox():
                 ccxt_client_util.set_sandbox_mode(
-                    self, self.exchange_manager.is_sandboxed)
+                    self, self.exchange_manager.is_sandboxed
+                )
                 
             if self.force_authentication or (
                 self._should_authenticate() and not self.exchange_manager.exchange_only
             ):
                 await self._ensure_auth()
 
             if self.exchange_manager.is_loading_markets:
@@ -155,15 +156,15 @@
             self.unauthenticated_exchange_fallback(e)
         except Exception as e:
             # Is probably handled in exchange tentacles, important thing here is that authentication worked
             self.logger.debug(f"Error when checking exchange connection: {e}. This should not be an issue.")
 
     def _create_client(self):
         self.client, self.is_authenticated = ccxt_client_util.create_client(
-            self.exchange_type, self.name, self.exchange_manager, self.logger,
+            self.exchange_type, self.exchange_manager, self.logger,
             self.options, self.headers, self.additional_config,
             self._should_authenticate(), self.unauthenticated_exchange_fallback
         )
 
     def _should_authenticate(self):
         return self.force_authentication or not (
             self.exchange_manager.is_simulated or
@@ -400,15 +401,16 @@
                 return self.adapter.adapt_order(
                     await self.client.createStopMarketOrder(
                         symbol,
                         side=side,
                         amount=quantity,
                         stopPrice=price,
                         params=params,
-                    )
+                    ),
+                    symbol=symbol, quantity=quantity
                 )
             except ccxt.OrderImmediatelyFillable:
                 # make sure stop always stops
                 created_order = await self.exchange_manager.exchange.create_order(
                     order_type=(enums.TraderOrderType.BUY_MARKET
                                 if side == enums.TradeOrderSide.BUY.value
                                 else enums.TraderOrderType.SELL_MARKET),
@@ -429,15 +431,16 @@
                 await self.client.create_stop_limit_order(
                     symbol,
                     side=side,
                     amount=quantity,
                     price=price,
                     stopPrice=stop_price,
                     params=params,
-                )
+                ),
+                symbol=symbol, quantity=quantity
             )
         raise NotImplementedError("create_limit_stop_loss_order is not implemented")
 
     async def create_market_take_profit_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
         raise NotImplementedError("create_market_take_profit_order is not implemented")
 
     async def create_limit_take_profit_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
@@ -458,15 +461,15 @@
             # can't set price in market orders
             price_to_use = None
         # do not use keyword arguments here as default ccxt edit order is passing *args (and not **kwargs)
         return self.adapter.adapt_order(
             await self.client.edit_order(
                 exchange_order_id, symbol, ccxt_order_type, side, quantity, price_to_use, params
             ),
-            symbol=symbol
+            symbol=symbol, quantity=quantity
         )
 
     async def cancel_order(
         self, exchange_order_id: str, symbol: str, order_type: enums.TraderOrderType, **kwargs: dict
     ) -> enums.OrderStatus:
         try:
             with self.error_describer():
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 
     def _create_client(self):
         """
         Creates ccxt client instance
         """
         client_class = getattr(ccxtpro, self.get_feed_name())
         self.client, self.is_authenticated = ccxt_client_util.create_client(
-            client_class, self.name, self.exchange_manager, self.logger,
+            client_class, self.exchange_manager, self.logger,
             self.options, self.headers, self.additional_config,
             self._should_authenticate()
         )
         if self.exchange_manager.exchange.is_supporting_sandbox():
             ccxt_client_util.set_sandbox_mode(self, self.exchange_manager.is_sandboxed)
 
     def _should_authenticate(self):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/constants.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/ccxt/enums.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/ccxt/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,10 +106,19 @@
 
 
 class ExchangeWrapperLibs(enum.Enum):
     ASYNC_CCXT = "async_ccxt"
     CCXT = "ccxt"
 
 
+class ExchangeColumns(enum.Enum):
+    WEBSITE = "www"
+    URLS = "urls"
+    API = "api"
+    REST = "rest"
+    WEBSOCKET = "ws"
+    LOGO_URL = "logo"
+
+
 class ExchangeMarginTypes(enum.Enum):
     ISOLATED = "isolated"
     CROSS = "cross"
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_builder.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,17 @@
 
                 # create trading modes
                 await self._build_trading_modes_if_required(trading_mode_class)
 
             # add to global exchanges
             self.exchange_manager.update_debug_info()
         except Exception:
-            exchanges.Exchanges.instance().del_exchange(self.exchange_manager.exchange_name, self.exchange_manager.id)
+            exchanges.Exchanges.instance().del_exchange(
+                self.exchange_manager.exchange_name, self.exchange_manager.id, should_warn=False
+            )
             raise
 
     async def _build_trader(self):
         try:
             # check traders activation
             if not util.is_trader_enabled(self.config) and not util.is_trader_simulator_enabled(self.config):
                 raise ValueError(f"No trader simulator nor real trader activated on "
@@ -127,15 +129,18 @@
             raise e
 
     def _ensure_exchange_compatibility(self):
         if self.exchange_manager.is_backtesting or self.exchange_manager.exchange_only:
             # allow backtesting and collecting on incompatible exchange types
             return
         # live exchange: ensure the exchange to be created supports the trading type
-        supported_exchange_types = exchanges.get_supported_exchange_types(self.exchange_manager.exchange_name)
+        supported_exchange_types = exchanges.get_supported_exchange_types(
+            self.exchange_manager.exchange_name,
+            self.exchange_manager.tentacles_setup_config
+        )
         exchange_type = exchanges.get_exchange_type(self.exchange_manager)
         if exchange_type not in supported_exchange_types:
             raise errors.NotSupported(f"{self.exchange_manager.exchange_name} does not support {exchange_type.value}"
                                       f" trading. "
                                       f"Supported exchange types are {[t.value for t in supported_exchange_types]}.")
 
     def _ensure_trading_mode_compatibility(self, trading_mode_class):
@@ -206,16 +211,16 @@
         self.exchange_manager.exchange_only = True
         return self
 
     def is_loading_markets(self, is_loading_markets):
         self.exchange_manager.is_loading_markets = is_loading_markets
         return self
 
-    def is_ignoring_config(self):
-        self.exchange_manager.ignore_config = True
+    def is_ignoring_config(self, ignore_config=True):
+        self.exchange_manager.ignore_config = ignore_config
         return self
 
     def is_without_auth(self):
         self.exchange_manager.without_auth = True
         return self
 
     def is_checking_credentials(self, check_credentials):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_channels.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,17 @@
         # stop exchange channels
         if enable_logs:
             self.logger.debug(f"Stopping exchange channels for exchange_id: {self.id} ...")
         if self.exchange is not None:
             if not self.exchange_only:
                 await exchange_channel.stop_exchange_channels(self, should_warn=warning_on_missing_elements)
             await self.exchange.stop()
-            exchanges.Exchanges.instance().del_exchange(self.exchange.name, self.id,
-                                                        should_warn=warning_on_missing_elements)
+            exchanges.Exchanges.instance().del_exchange(
+                self.exchange.name, self.id, should_warn=warning_on_missing_elements
+            )
             self.exchange.exchange_manager = None
             self.exchange = None
         if self.exchange_personal_data is not None:
             await self.exchange_personal_data.stop()
         if self.exchange_symbols_data is not None:
             await self.exchange_symbols_data.stop()
         if enable_logs:
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchange_websocket_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchange_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/exchanges.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/exchanges.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,17 @@
         try:
             self.exchanges[exchange_name].pop(exchange_manager_id, None)
 
             if not self.exchanges[exchange_name]:
                 self.exchanges.pop(exchange_name, None)
         except KeyError:
             if should_warn:
-                logging.get_logger(self.__class__.__name__).warning(f"Can't del exchange {exchange_name} "
-                                                                    f"with id {exchange_manager_id}")
+                logging.get_logger(self.__class__.__name__).warning(
+                    "Can't del exchange {exchange_name} with id {exchange_manager_id}"
+                )
 
     def get_exchange_names(self) -> typing.KeysView:
         return self.exchanges.keys()
 
     def get_exchange_ids(self) -> list:
         return [exchange_id
                 for exchange_managers in self.exchanges.values()
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/default_rest_exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/default_websocket_exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/default_websocket_exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class DefaultWebSocketExchange(exchanges_types.WebSocketExchange):
     DEFAULT_CONNECTOR_CLASS = ccxt_websocket_connector.CCXTWebsocketConnector
 
     @classmethod
     def get_exchange_connector_class(cls, exchange_manager):
         return api.get_class_from_name_with_activated_required_tentacles(
-            name=exchange_manager.exchange_name,
+            name=exchange_manager.exchange.get_associated_websocket_exchange_name(),
             tentacles_setup_config=exchange_manager.tentacles_setup_config,
             parent_class=cls.DEFAULT_CONNECTOR_CLASS
         )
 
     def create_feeds(self):
         try:
             connector = self.websocket_connector(config=self.config, exchange_manager=self.exchange_manager,
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/implementations/exchange_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/implementations/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/trader.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,16 @@
                             params=order_params
                         )
                         # apply new values from returned order (even order id might have changed)
                         self.logger.debug(f"Successfully edited order on {self.exchange_manager.exchange_name}, "
                                           f"new order values: {edited_order}")
                         changed = order.update_from_raw(edited_order)
                         # update portfolio from exchange
-                        await self.exchange_manager.exchange_personal_data.handle_portfolio_update_from_order(order)
+                        await self.exchange_manager.exchange_personal_data.\
+                            handle_portfolio_and_position_update_from_order(order)
                 else:
                     # consider order as cancelled to release portfolio amounts
                     self.exchange_manager.exchange_personal_data.portfolio_manager.portfolio.update_portfolio_available(
                         order, is_new_order=False
                     )
                     changed = order.update(
                         order.symbol,
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/traders/trader_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/traders/trader_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/rest_exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/rest_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,26 +50,29 @@
     DUMP_INCOMPLETE_LAST_CANDLE = False  # set True in tentacle when the exchange can return incomplete last candles
     # Set True when exchange is not returning empty position details when fetching a position with a specified symbol
     # Exchange will then fallback to self.get_mocked_empty_position when having get_position returning None
     REQUIRES_MOCKED_EMPTY_POSITION = False
     # set True when get_positions() is not returning empty positions and should use get_position() instead
     REQUIRES_SYMBOL_FOR_EMPTY_POSITION = False
     SUPPORTS_SET_MARGIN_TYPE = True  # set False when there is no API to switch between cross and isolated margin types
+    SUPPORTS_SET_MARGIN_TYPE_ON_OPEN_POSITIONS = True  # set False when the exchange refuses to change margin type
+    # when an associated position is open
     EXPECT_POSSIBLE_ORDER_NOT_FOUND_DURING_ORDER_CREATION = False  # set True when get_order() can return None
     # (order not found) when orders are being created on exchange and are not fully processed on the exchange side.
     REQUIRES_AUTHENTICATION = False  # set True when even normally public apis require authentication
+    HAS_FETCHED_DETAILS = False  # set True when this exchange details (urls etc) have to be fetched before
+    # starting the exchange
     """
     RestExchange is using its exchange connector to interact with the exchange.
     It should be used regardless of the exchange or the exchange library (ccxt or other)
     Always take and returns octobot formatted data and errors
     Is used request regardless of the trading type (spot / future / other)
 
     Is extended in exchange tentacles to define custom behaviors or exchange adapter (override of get_adapter_class)
     """
-
     # Mark price params
     MARK_PRICE_IN_POSITION = False
     MARK_PRICE_IN_TICKER = False
 
     # Funding rate params
     FUNDING_WITH_MARK_PRICE = False
     FUNDING_IN_TICKER = False
@@ -77,17 +80,18 @@
     # Set when order cost is not (yet) accurately computed for a given exchange
     MAX_INCREASED_POSITION_QUANTITY_MULTIPLIER = constants.ONE
 
     DEFAULT_CONNECTOR_CLASS = ccxt_connector.CCXTConnector
 
     def __init__(self, config, exchange_manager, connector_class=None):
         super().__init__(config, exchange_manager)
+        if self.HAS_FETCHED_DETAILS:
+            self._fetch_details(config, exchange_manager)
         self.connector = self._create_connector(config, exchange_manager, connector_class)
         self.pair_contracts = {}
-        self.update_supported_elements(exchange_manager)
 
     def _create_connector(self, config, exchange_manager, connector_class):
         return (connector_class or self.DEFAULT_CONNECTOR_CLASS)(
             config,
             exchange_manager,
             adapter_class=self.get_adapter_class(),
             additional_config=self.get_additional_connector_config(),
@@ -105,31 +109,30 @@
         self.exchange_manager = None
 
     @classmethod
     def get_name(cls):
         return cls.__name__
 
     @classmethod
-    def update_supported_elements(cls, exchange_manager):
-        pass
-
-    @classmethod
     def is_supporting_exchange(cls, exchange_candidate_name) -> bool:
         return cls.get_name() == exchange_candidate_name
 
     @classmethod
     def get_supported_exchange_types(cls) -> list:
         """
         :return: The list of supported exchange types. Override if necessary
         """
         return [enums.ExchangeTypes.SPOT]
 
     def get_rest_name(self):
         return self.exchange_manager.exchange_class_string
 
+    def get_associated_websocket_exchange_name(self):
+        return self.exchange_manager.exchange_name
+
     def get_adapter_class(self):
         # Override in tentacles when using a custom adapter
         return None
 
     async def create_order(self, order_type: enums.TraderOrderType, symbol: str, quantity: decimal.Decimal,
                            price: decimal.Decimal = None, stop_price: decimal.Decimal = None,
                            side: enums.TradeOrderSide = None, current_price: decimal.Decimal = None,
@@ -828,14 +831,29 @@
         """
         :param symbol: the symbol
         :return: True if the symbol is related to a contract having an expiration date
         """
         return self.connector.is_expirable_symbol(symbol)
 
     """
+    Auto fetched and filled exchanges
+    """
+    def _fetch_details(self, config, exchange_manager):
+        raise NotImplementedError("_fetch_details is not implemented")
+
+    @staticmethod
+    def supported_autofill_exchanges(tentacle_config):
+        raise NotImplementedError("supported_autofill_exchanges is not implemented")
+
+    @classmethod
+    async def get_autofilled_exchange_details(cls, aiohttp_session, tentacle_config, exchange_name):
+        raise NotImplementedError("get_autofilled_exchange_details is not implemented")
+
+
+    """
     Parsers todo remove ?
     """
 
     def parse_order_book_ticker(self, order_book_ticker):
         return self.connector.parse_order_book_ticker(order_book_ticker)
 
     def parse_exhange_order_id(self, order):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/types/websocket_exchange.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/types/websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,23 +22,26 @@
 from octobot_trading.exchanges.util import exchange_util
 from octobot_trading.exchanges.util.exchange_util import (
     get_rest_exchange_class,
     get_order_side,
     log_time_sync_error,
     get_partners_explanation_message,
     get_enabled_exchanges,
+    get_local_exchange_manager,
     is_compatible_account,
     get_historical_ohlcv,
     get_exchange_type,
     get_default_exchange_type,
     get_supported_exchange_types,
     update_raw_order_from_raw_trade,
     is_missing_trading_fees,
     apply_trades_fees,
     get_exchange_class_from_name,
+    get_auto_filled_exchange_names,
+    get_exchange_details,
 )
 from octobot_trading.exchanges.util import websockets_util
 from octobot_trading.exchanges.util.websockets_util import (
     force_disable_web_socket,
     check_web_socket_config,
     search_websocket_class,
     supports_websocket,
@@ -48,21 +51,24 @@
     "ExchangeMarketStatusFixer",
     "is_ms_valid",
     "get_rest_exchange_class",
     "get_order_side",
     "log_time_sync_error",
     "get_partners_explanation_message",
     "get_enabled_exchanges",
+    "get_local_exchange_manager",
     "is_compatible_account",
     "get_historical_ohlcv",
     "get_exchange_type",
     "get_default_exchange_type",
     "get_supported_exchange_types",
     "update_raw_order_from_raw_trade",
     "is_missing_trading_fees",
     "apply_trades_fees",
     "get_exchange_class_from_name",
+    "get_auto_filled_exchange_names",
+    "get_exchange_details",
     "force_disable_web_socket",
     "check_web_socket_config",
     "search_websocket_class",
     "supports_websocket",
 ]
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/exchange_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/exchange_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import contextlib
+import ccxt
 import trading_backend
 
 import octobot_commons.logging as logging
 import octobot_commons.constants as common_constants
 import octobot_commons.enums as common_enums
 import octobot_commons.tentacles_management as tentacles_management
 
 import octobot_tentacles_manager.api as api
 
 import octobot_trading.enums as enums
 import octobot_trading.constants as constants
 import octobot_trading.exchanges.types as exchanges_types
 import octobot_trading.exchanges.implementations as exchanges_implementations
+import octobot_trading.exchanges.connectors.ccxt.enums as ccxt_enums
+import octobot_trading.exchanges.exchange_details as exchange_details
 import octobot_trading.exchanges.exchange_builder as exchange_builder
 
 
 def get_rest_exchange_class(exchange_name, tentacles_setup_config):
     return search_exchange_class_from_exchange_name(exchanges_types.RestExchange, exchange_name, tentacles_setup_config)
 
 
@@ -47,35 +51,90 @@
     if children_classes:
         # last one is the most advanced one
         return children_classes[-1]
     # fallback to DefaultRestExchange
     return exchanges_implementations.DefaultRestExchange
 
 
-def get_exchange_class_from_name(exchange_parent_class, exchange_name, tentacles_setup_config, enable_default,
-                                 strict_name_matching=False):
+def get_exchange_class_from_name(exchange_parent_class, exchange_name, tentacles_setup_config,
+                                 enable_default_implementation, strict_name_matching=False):
     for exchange_candidate in tentacles_management.get_all_classes_from_parent(exchange_parent_class):
         try:
-            if _is_exchange_candidate_matching(exchange_candidate, exchange_name,
-                                               tentacles_setup_config, enable_default=enable_default) and \
-               (not strict_name_matching or exchange_candidate.get_name() == exchange_name):
+            if _is_exchange_candidate_matching(
+                exchange_candidate, exchange_name, tentacles_setup_config,
+                enable_default_implementation=enable_default_implementation
+            ) and (not strict_name_matching or exchange_candidate.get_name() == exchange_name):
                 return exchange_candidate
         except NotImplementedError:
             # A subclass of AbstractExchange will raise a NotImplementedError when calling its get_name() method
             # Here we are returning only a subclass that matches the expected name
             # Only Exchange Tentacles are implementing get_name() to specify the related exchange
             # As we are searching for an exchange_type specific subclass
             # We should ignore classes that raises NotImplementedError
             pass
+    auto_filled_exchanges = _get_auto_filled_exchanges(tentacles_setup_config)
+    if exchange_name in auto_filled_exchanges:
+        return auto_filled_exchanges[exchange_name][0]
     return None
 
 
-def _is_exchange_candidate_matching(exchange_candidate, exchange_name, tentacles_setup_config, enable_default=False):
+def _get_auto_filled_exchanges(tentacles_setup_config):
+    auto_filled_exchanges = {}
+    for exchange_candidate in _get_auto_filled_exchanges_tentacles():
+        if tentacles_setup_config is None:
+            # tentacles_setup_config is required for auto-filled exchanges
+            continue
+        config = api.get_tentacle_config(
+            tentacles_setup_config, exchange_candidate
+        )
+        for exchange_name in exchange_candidate.supported_autofill_exchanges(config):
+            auto_filled_exchanges[exchange_name] = (exchange_candidate, config)
+    return auto_filled_exchanges
+
+
+def get_auto_filled_exchange_names(tentacles_setup_config):
+    return list(_get_auto_filled_exchanges(tentacles_setup_config))
+
+
+def _get_auto_filled_exchanges_tentacles():
+    return [
+        exchange_candidate
+        for exchange_candidate in tentacles_management.get_all_classes_from_parent(exchanges_types.RestExchange)
+        if exchange_candidate.HAS_FETCHED_DETAILS
+    ]
+
+
+async def get_exchange_details(
+    exchange_name, is_autofilled, tentacles_setup_config, aiohttp_session
+) -> exchange_details.ExchangeDetails:
+    if is_autofilled:
+        auto_filled_exchanges = _get_auto_filled_exchanges(tentacles_setup_config)
+        if exchange_name in auto_filled_exchanges:
+            return await auto_filled_exchanges[exchange_name][0].get_autofilled_exchange_details(
+                aiohttp_session, auto_filled_exchanges[exchange_name][1], exchange_name
+            )
+    try:
+        exchange = getattr(ccxt, exchange_name)()
+        return exchange_details.ExchangeDetails(
+            exchange.id,
+            exchange.name,
+            exchange.urls[ccxt_enums.ExchangeColumns.WEBSITE.value],
+            exchange.urls[ccxt_enums.ExchangeColumns.API.value],
+            exchange.urls[ccxt_enums.ExchangeColumns.LOGO_URL.value],
+            False,
+        )
+    except AttributeError as err:
+        raise KeyError from err
+
+
+def _is_exchange_candidate_matching(
+    exchange_candidate, exchange_name, tentacles_setup_config, enable_default_implementation=False
+):
     return not exchange_candidate.is_simulated_exchange() and \
-           (not exchange_candidate.is_default_exchange() or enable_default) and \
+           (not exchange_candidate.is_default_exchange() or enable_default_implementation) and \
            exchange_candidate.is_supporting_exchange(exchange_name) and \
            (tentacles_setup_config is None or
             api.is_tentacle_activated_in_tentacles_setup_config(tentacles_setup_config,
                                                                 exchange_candidate.__name__))
 
 
 def get_order_side(order_type):
@@ -137,61 +196,72 @@
         for exchange_name in config[common_constants.CONFIG_EXCHANGES]
         if config[common_constants.CONFIG_EXCHANGES][exchange_name].get(
                 common_constants.CONFIG_ENABLED_OPTION, True
         )
     ]
 
 
-async def is_compatible_account(exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool) \
-        -> (bool, bool, str):
-    """
-    Returns details regarding the compatibility of the account given in parameters
-    :return: (True if compatible, True if successful login, error explanation if any)
-    """
+@contextlib.asynccontextmanager
+async def get_local_exchange_manager(
+    exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool, ignore_config=False
+):
     exchange_type = exchange_config.get(common_constants.CONFIG_EXCHANGE_TYPE, get_default_exchange_type(exchange_name))
     builder = exchange_builder.ExchangeBuilder(
         _get_minimal_exchange_config(exchange_name, exchange_config),
         exchange_name
     )
-    local_exchange_manager = await builder.use_tentacles_setup_config(tentacles_setup_config) \
+    exchange_manager = await builder.use_tentacles_setup_config(tentacles_setup_config) \
         .is_checking_credentials(False) \
         .is_sandboxed(is_sandboxed) \
         .is_using_exchange_type(exchange_type) \
         .is_exchange_only() \
         .is_rest_only() \
         .is_loading_markets(False) \
+        .is_ignoring_config(ignore_config) \
         .disable_trading_mode() \
         .build()
-    backend = trading_backend.exchange_factory.create_exchange_backend(local_exchange_manager.exchange)
     try:
-        is_compatible, error = await backend.is_valid_account()
-        if not local_exchange_manager.is_spot_only:
-            message = f"Future trading on {exchange_name.capitalize()} requires a supporting account. {error}." \
-                      f"Please create a new {exchange_name.capitalize()} account to use futures trading. "
-            # only ensure compatibility for non spot trading
-            return is_compatible, True, message if error else error
-        else:
-            # auth didn't fail, spot trading is always allowed
-            return True, True, None
-    except trading_backend.TimeSyncError:
-        return False, False, _get_time_sync_error_message(exchange_name, "backend.is_valid_account")
-    except trading_backend.ExchangeAuthError:
-        return False, False, f"Invalid {exchange_name.capitalize()} authentication details"
-    except (AttributeError, Exception) as e:
-        return True, False, f"Error when loading exchange account: {e}"
+        yield exchange_manager
     finally:
         # do not log stopping message
-        logger = local_exchange_manager.exchange.connector.logger
+        logger = exchange_manager.exchange.connector.logger
         logger.disable(True)
-        await local_exchange_manager.stop(enable_logs=False)
         builder.clear()
-        builder = local_exchange_manager = None
+        await exchange_manager.stop(enable_logs=False)
         logger.disable(False)
 
 
+async def is_compatible_account(exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool) \
+        -> (bool, bool, str):
+    """
+    Returns details regarding the compatibility of the account given in parameters
+    :return: (True if compatible, True if successful login, error explanation if any)
+    """
+    async with get_local_exchange_manager(
+        exchange_name, exchange_config, tentacles_setup_config, is_sandboxed, ignore_config=False
+    ) as local_exchange_manager:
+        backend = trading_backend.exchange_factory.create_exchange_backend(local_exchange_manager.exchange)
+        try:
+            is_compatible, error = await backend.is_valid_account()
+            if not local_exchange_manager.is_spot_only:
+                message = f"Future trading on {exchange_name.capitalize()} requires a supporting account. {error}." \
+                          f"Please create a new {exchange_name.capitalize()} account to use futures trading. "
+                # only ensure compatibility for non spot trading
+                return is_compatible, True, message if error else error
+            else:
+                # auth didn't fail, spot trading is always allowed
+                return True, True, None
+        except trading_backend.TimeSyncError:
+            return False, False, _get_time_sync_error_message(exchange_name, "backend.is_valid_account")
+        except trading_backend.ExchangeAuthError:
+            return False, False, f"Invalid {exchange_name.capitalize()} authentication details"
+        except (AttributeError, Exception) as e:
+            return True, False, f"Error when loading exchange account: {e}"
+
+
 async def get_historical_ohlcv(
     local_exchange_manager, symbol, time_frame, start_time, end_time,
         request_retry_timeout=constants.HISTORICAL_CANDLES_FETCH_DEFAULT_TIMEOUT
 ):
     """
     Async generator, use as follows:
         async for candles in get_historical_ohlcv(exchange_manager, pair, time_frame, start_time, end_time):
@@ -233,17 +303,18 @@
 
 def get_default_exchange_type(exchange_name):
     if exchange_name in constants.DEFAULT_FUTURE_EXCHANGES:
         return common_constants.CONFIG_EXCHANGE_FUTURE
     return common_constants.DEFAULT_EXCHANGE_TYPE
 
 
-def get_supported_exchange_types(exchange_name):
-    exchange_class = get_exchange_class_from_name(exchanges_types.RestExchange, exchange_name, None, False,
-                                                  strict_name_matching=True)
+def get_supported_exchange_types(exchange_name, tentacles_setup_config):
+    exchange_class = get_exchange_class_from_name(
+        exchanges_types.RestExchange, exchange_name, tentacles_setup_config, False, strict_name_matching=True
+    )
     if exchange_class is None:
         # default
         return [enums.ExchangeTypes.SPOT]
     return exchange_class.get_supported_exchange_types()
 
 
 def update_raw_order_from_raw_trade(order_to_update, raw_trade):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/exchanges/util/websockets_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/exchanges/util/websockets_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/abstract_trading_mode.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/channel/abstract_mode_consumer.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/channel/abstract_mode_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,26 +127,38 @@
                                                        portfolio_type=commons_constants.PORTFOLIO_AVAILABLE)
             side = enums.TradeOrderSide.SELL \
                 if state == enums.EvaluatorStates.VERY_SHORT.value or state == enums.EvaluatorStates.SHORT.value \
                 else enums.TradeOrderSide.BUY
             max_order_size, _ = personal_data.get_futures_max_order_size(
                 self.exchange_manager, symbol, side, current_price, False, current_symbol_holding, market_quantity
             )
+            self.logger.debug(
+                f"can_create_order: max_order_size > symbol_min_amount: {max_order_size} > {symbol_min_amount}"
+            )
             return max_order_size > symbol_min_amount
 
         # spot, trade asset directly
         # short cases => sell => need this currency
         if state == enums.EvaluatorStates.VERY_SHORT.value or state == enums.EvaluatorStates.SHORT.value:
+            self.logger.debug(
+                f"can_create_order: portfolio.get_currency_portfolio(currency).available > symbol_min_amount: "
+                f"{portfolio.get_currency_portfolio(currency).available} > {symbol_min_amount}"
+            )
             return portfolio.get_currency_portfolio(currency).available > symbol_min_amount
 
         # long cases => buy => need money(aka other currency in the pair) to buy this currency
         elif state == enums.EvaluatorStates.LONG.value or state == enums.EvaluatorStates.VERY_LONG.value:
+            self.logger.debug(
+                f"can_create_order: portfolio.get_currency_portfolio(market).available > order_min_amount: "
+                f"{portfolio.get_currency_portfolio(market).available} > {order_min_amount}"
+            )
             return portfolio.get_currency_portfolio(market).available > order_min_amount
 
         # other cases like neutral state or unfulfilled previous conditions
+        self.logger.debug("can_create_order: return False")
         return False
 
     def get_holdings_ratio(self, currency):
         return self.exchange_manager.exchange_personal_data.portfolio_manager.portfolio_value_holder \
             .get_currency_holding_ratio(currency)
 
     def get_number_of_traded_assets(self):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/channel/abstract_mode_producer.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/channel/abstract_mode_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,18 @@
                 common_enums.ActivationTopics.IN_CONSTRUCTION_CANDLES.value
             ]
             await script_keywords.get_activation_topics(
                 context,
                 common_enums.ActivationTopics.EVALUATION_CYCLE.value,
                 activation_topic_values
             )
-        await self._apply_exchange_side_config(context)
+        try:
+            await self._apply_exchange_side_config(context)
+        except Exception as err:
+            self.logger.exception(err, True, f"Error when applying exchange side config: {err}")
 
     async def _apply_exchange_side_config(self, context):
         # can be slow, call in a task if necessary
         if context.exchange_manager.is_future:
             if not self._is_ready_to_trade.is_set():
                 await util.wait_for_topic_init(self.exchange_manager, self.CONFIG_INIT_TIMEOUT,
                                                common_enums.InitializationEventExchangeTopics.CONTRACTS.value)
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/channel/mode.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/channel/mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/mode_config.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/mode_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/modes_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/modes_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/modes_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/modes_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/amount.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/configuration.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,21 @@
         try:
             await ctx.exchange_manager.trader.set_leverage(ctx.symbol, side, decimal.Decimal(str(leverage)))
         except errors.ContractExistsError as e:
             ctx.logger.debug(str(e))
         except NotImplementedError as e:
             ctx.logger.exception(e, True, str(e))
         except Exception as e:
-            ctx.logger.exception(e, True, str(e))
+            contract = ctx.exchange_manager.exchange.get_pair_future_contract(ctx.symbol)
+            ctx.logger.exception(
+                e,
+                True,
+                f"Impossible to set leverage to {leverage}, using current "
+                f"value instead: {contract.current_leverage} ({e})"
+            )
 
 
 async def set_partial_take_profit_stop_loss(ctx, tp_sl_mode=enums.TakeProfitStopLossMode.PARTIAL.value):
     if ctx.exchange_manager.is_future:
         await ctx.exchange_manager.trader.set_symbol_take_profit_stop_loss_mode(
             ctx.symbol, enums.TakeProfitStopLossMode(tp_sl_mode)
         )
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/context_management.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/context_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/quantity.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/script_keywords/dsl/values.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/script_keywords/dsl/values.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/scripted_trading_mode/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/scripted_trading_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py` & `OctoBot-Trading-2.4.5/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/octobot_channel_consumer.py` & `OctoBot-Trading-2.4.5/octobot_trading/octobot_channel_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,43 +59,49 @@
     """
     if subject == enums.OctoBotChannelSubjects.CREATION.value:
         await _handle_creation(bot_id, action, data)
 
 
 async def _handle_creation(bot_id, action, data):
     if action == OctoBotChannelTradingActions.EXCHANGE.value:
+        exchange_name = data.get(OctoBotChannelTradingDataKeys.EXCHANGE_NAME.value, None)
         try:
-            exchange_name = data.get(OctoBotChannelTradingDataKeys.EXCHANGE_NAME.value, None)
             config = data[OctoBotChannelTradingDataKeys.EXCHANGE_CONFIG.value]
             exchange_builder = exchanges.create_exchange_builder_instance(config, exchange_name) \
                 .has_matrix(data[OctoBotChannelTradingDataKeys.MATRIX_ID.value]) \
                 .use_tentacles_setup_config(data[OctoBotChannelTradingDataKeys.TENTACLES_SETUP_CONFIG.value]) \
                 .set_bot_id(bot_id)
             _set_exchange_type_details(exchange_builder, config, data[OctoBotChannelTradingDataKeys.BACKTESTING.value])
             await exchange_builder.build()
-            await channel_instances.get_chan_at_id(channels_name.OctoBotChannelsName.OCTOBOT_CHANNEL.value,
-                                                   bot_id).get_internal_producer() \
-                .send(bot_id=bot_id,
-                      subject=enums.OctoBotChannelSubjects.NOTIFICATION.value,
-                      action=action,
-                      data={OctoBotChannelTradingDataKeys.EXCHANGE_ID.value: exchange_builder.exchange_manager.id})
+            await channel_instances.get_chan_at_id(
+                channels_name.OctoBotChannelsName.OCTOBOT_CHANNEL.value, bot_id
+            ).get_internal_producer().send(
+                bot_id=bot_id,
+                subject=enums.OctoBotChannelSubjects.NOTIFICATION.value,
+                action=action,
+                data={OctoBotChannelTradingDataKeys.EXCHANGE_ID.value: exchange_builder.exchange_manager.id}
+            )
         except errors.TradingModeIncompatibility as e:
             logging.get_logger(OCTOBOT_CHANNEL_TRADING_CONSUMER_LOGGER_TAG).error(
                 f"Error when initializing trading mode, {exchange_name} "
                 f"exchange connection is closed to increase performances: {e}")
         except errors.UnreachableExchange as e:
             logging.get_logger(OCTOBOT_CHANNEL_TRADING_CONSUMER_LOGGER_TAG).exception(
                 e,
                 True,
-                f"Error when connecting to {exchange_name} exchange, please check your internet connection ({e}).")
+                f"Error when connecting to {exchange_name} exchange, please check your internet connection ({e})."
+            )
+        except errors.NotSupported as e:
+            logging.get_logger(OCTOBOT_CHANNEL_TRADING_CONSUMER_LOGGER_TAG).exception(e, True, str(e))
         except Exception as e:
             logging.get_logger(OCTOBOT_CHANNEL_TRADING_CONSUMER_LOGGER_TAG).exception(
                 e,
                 True,
-                f"Error when creating a new {exchange_name} exchange connexion: {e.__class__.__name__} {e}")
+                f"Error when creating a new {exchange_name} exchange connexion: {e.__class__.__name__} {e}"
+            )
 
 
 def _set_exchange_type_details(exchange_builder, config, backtesting):
     # real, simulator, backtesting
     if util.is_trader_enabled(config):
         exchange_builder.is_real()
     elif util.is_trader_simulator_enabled(config):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/exchange_personal_data.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/exchange_personal_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,25 @@
                 if should_notify:
                     await self.handle_portfolio_update_notification(balance)
                 return changed
         except AttributeError as e:
             self.logger.exception(e, True, f"Failed to update balance : {e}")
             return False
 
-    async def handle_portfolio_update_from_order(self, order,
-                                                 require_exchange_update: bool = True,
-                                                 should_notify: bool = True) -> bool:
+    async def handle_portfolio_and_position_update_from_order(
+        self, order, require_exchange_update: bool = True, should_notify: bool = True
+    ) -> bool:
         try:
-            changed: bool = await self.portfolio_manager.handle_balance_update_from_order(order,
-                                                                                          require_exchange_update)
+            changed: bool = await self.portfolio_manager.handle_balance_update_from_order(
+                order, require_exchange_update
+            )
+            if self.exchange_manager.is_future:
+                changed = await self.positions_manager.handle_position_update_from_order(
+                    order, require_exchange_update
+                ) and changed
             if should_notify:
                 await self.handle_portfolio_update_notification(self.portfolio_manager.portfolio.portfolio)
 
                 if self.exchange_manager.is_future:
                     # should this be done only "if should_notify" ?
                     await self.handle_position_instance_update(
                         order.exchange_manager.exchange_personal_data.positions_manager.get_order_position(order),
@@ -199,15 +204,19 @@
                 self.logger.debug(f"Failed to update order : Order was not found ({ke})")
             except Exception as e:
                 self.logger.exception(e, True, f"Failed to update order : {e}")
         return False, None
 
     async def update_order_from_stored_data(self, exchange_order_id, pending_groups):
         order = self.orders_manager.get_order(None, exchange_order_id=exchange_order_id)
+        previous_order_id = order.order_id
         await orders_storage_operations.apply_order_storage_details_if_any(order, self.exchange_manager, pending_groups)
+        if previous_order_id != order.order_id:
+            # order_id got restored to its original value
+            self.orders_manager.replace_order(previous_order_id, order)
 
     async def on_order_refresh_success(self, order, should_notify, is_new_order):
         if order.state is not None:
             asyncio.create_task(order.state.on_refresh_successful())
 
         if should_notify:
             update_type = enums.OrderUpdateType.NEW if is_new_order else enums.OrderUpdateType.STATE_CHANGE
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/orders.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/orders_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/orders_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 
 import octobot_commons.async_job as async_job
 import octobot_commons.tree as commons_tree
 import octobot_commons.enums as commons_enums
-import octobot_commons.constants as commons_constants
 
 import octobot_trading.errors as errors
 import octobot_trading.personal_data.orders.channel.orders as orders_channel
 import octobot_trading.constants as constants
 
 
 class OrdersUpdater(orders_channel.OrdersProducer):
@@ -35,15 +34,15 @@
     CHANNEL_NAME = constants.ORDERS_CHANNEL
     ORDERS_UPDATE_LIMIT = None
     ORDERS_STARTING_REFRESH_TIME = 10
     OPEN_ORDER_REFRESH_TIME = 7
     CLOSE_ORDER_REFRESH_TIME = 81
     TIME_BETWEEN_ORDERS_REFRESH = 2
     DEPENDENCIES_TIMEOUT = 30
-    OPEN_ORDER_INITIAL_FETCH_GIVE_UP_TIMEOUT = 3 * commons_constants.MINUTE_TO_SECONDS
+    OPEN_ORDER_INITIAL_FETCH_GIVE_UP_TIMEOUT = 30
 
     def __init__(self, channel):
         super().__init__(channel)
 
         self._is_initialized_event_set = False
         # create async jobs
         self.open_orders_job = async_job.AsyncJob(self._open_orders_fetch_and_push,
@@ -85,15 +84,15 @@
 
     async def start(self) -> None:
         """
         Start updater jobs
         """
         await self.initialize()
         await asyncio.sleep(self.ORDERS_STARTING_REFRESH_TIME)
-        await self.open_orders_job.run()
+        await self.open_orders_job.run(retry_attempts=1)
         # await self.closed_orders_job.run()
 
     async def fetch_and_push(self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT, retry_till_success=False):
         """
         Update open and closed orders from exchange
         :param is_from_bot: True if the order was created by OctoBot
         :param limit: the exchange request orders count limit
@@ -109,26 +108,34 @@
         await asyncio.sleep(self.TIME_BETWEEN_ORDERS_REFRESH)
         try:
             # can raise, closed orders are not critical data
             await self._closed_orders_fetch_and_push(limit=limit)
         except errors.NotSupported:
             self.logger.debug(f"{self.channel.exchange_manager.exchange_name} is not supporting closed orders updates")
 
-    async def _open_orders_fetch_and_push(self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT, retry_till_success=False):
+    async def _open_orders_fetch_and_push(
+        self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT, retry_till_success=False, retry_attempts=0
+    ):
         """
         Update open orders from exchange
         :param is_from_bot: True if the order was created by OctoBot
         :param limit: the exchange request orders count limit
         :param retry_till_success: retry request till it works. Should be rarely used as it might take some time
+        :param retry_attempts: how many times to retry before failing
         """
         for symbol in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
             if retry_till_success:
                 open_orders: list = await self.channel.exchange_manager.exchange.retry_till_success(
                     self.OPEN_ORDER_INITIAL_FETCH_GIVE_UP_TIMEOUT,
-                    self.channel.exchange_manager.exchange.get_open_orders, symbol=symbol, limit=limit
+                    self.channel.exchange_manager.exchange.get_open_orders, symbol=symbol, limit=limit,
+                )
+            elif retry_attempts:
+                open_orders: list = await self.channel.exchange_manager.exchange.retry_n_time(
+                    retry_attempts,
+                    self.channel.exchange_manager.exchange.get_open_orders, symbol=symbol, limit=limit,
                 )
             else:
                 open_orders: list = await self.channel.exchange_manager.exchange.get_open_orders(
                     symbol=symbol, limit=limit
                 )
             if open_orders:
                 await self.push(open_orders, is_from_bot=is_from_bot)
@@ -181,15 +188,15 @@
     async def _order_fetch_and_push(self, order, should_notify=False):
         """
         Update Order from exchange
         :param order: the order to update
         :param should_notify: if Orders channel consumers should be notified
         :return: True if the order was updated
         """
-        exchange_name = order.exchange_manager.exchange_name if order.exchange_manager else "cleared order's exchange"
+        exchange_name = self.channel.exchange_manager.exchange_name
         self.logger.debug(f"Requested update for {order} on {exchange_name}")
         raw_order = await self.channel.exchange_manager.exchange.get_order(order.exchange_order_id, order.symbol)
 
         if raw_order is not None:
             self.logger.debug(f"Received update for {order} on {exchange_name}: {raw_order}")
 
             await self.channel.exchange_manager.exchange_personal_data.handle_order_update_from_raw(
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/decimal_order_adapter.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/group_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/group_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 def get_or_create_order_group_from_storage_order_details(order_details, exchange_manager):
     group = order_details.get(enums.StoredOrdersAttr.GROUP.value, None)
     if group:
         try:
             group_name = group.get(enums.StoredOrdersAttr.GROUP_ID.value, None)
             if group_name:
-                return exchange_manager.exchange_personal_data.orders_manager.get_or_create_group(
+                group = exchange_manager.exchange_personal_data.orders_manager.get_or_create_group(
                     get_group_class(group[enums.StoredOrdersAttr.GROUP_TYPE.value]),
                     group_name,
                 )
+                logging.get_logger("GroupUtil").debug(f"Restored {group} order group")
+                return group
         except KeyError as err:
             logging.get_logger("GroupUtil").error(f"Unhandled group type: {err}")
     return None
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,15 +746,15 @@
         tag = f" | tag: {self.tag}" if self.tag else ""
         return (f"{self.symbol} | "
                 f"{chained_order}"
                 f"{self.order_type.name if self.order_type is not None else 'Unknown'} | "
                 f"Price : {str(self.origin_price)} | "
                 f"Quantity : {str(self.origin_quantity)} | "
                 f"State : {self.state.state.value if self.state is not None else 'Unknown'} | "
-                f"id : {self.order_id}{tag}"
+                f"id : {self.order_id}{tag} "
                 f"exchange id: {self.exchange_order_id}")
 
     def __str__(self):
         return self.to_string()
 
     def is_to_be_maintained(self):
         return self.trader is not None
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_adapter.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_group.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/order_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/order_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,23 +417,23 @@
     current_symbol_holding, current_market_holding, market_quantity, _, _ = \
         await get_pre_order_data(exchange_manager,
                                  symbol=symbol,
                                  timeout=constants.ORDER_DATA_FETCHING_TIMEOUT,
                                  portfolio_type=commons_constants.PORTFOLIO_TOTAL)
     if exchange_manager.is_future:
         # TODO check inverse
-        if market_quantity is constants.ZERO:
+        if market_quantity == constants.ZERO:
             return constants.ZERO
         return min(order_amount / market_quantity, constants.ONE) * constants.ONE_HUNDRED
     if side is enums.TradeOrderSide.SELL:
-        if current_symbol_holding is constants.ZERO:
+        if current_symbol_holding == constants.ZERO:
             return constants.ZERO
         return min(order_amount / current_symbol_holding, constants.ONE) * constants.ONE_HUNDRED
     if side is enums.TradeOrderSide.BUY:
-        if current_market_holding is constants.ZERO:
+        if current_market_holding == constants.ZERO:
             return constants.ZERO
         return min(order_amount / market_quantity, constants.ONE) * constants.ONE_HUNDRED
     raise errors.InvalidArgumentError(f"Unhandled side: {side}")
 
 
 def generate_order_id():
     return str(uuid.uuid4())
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/orders_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/orders_storage_operations.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/orders_storage_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,27 @@
 
 
 async def apply_order_storage_details_if_any(order, exchange_manager, pending_groups):
     # only real orders can be updated by stored orders
     if not exchange_manager.storage_manager.orders_storage \
             or not exchange_manager.storage_manager.orders_storage.should_store_date():
         return
-    order_details = await exchange_manager.storage_manager.orders_storage.get_startup_order_details(order.order_id)
+    order_details = await exchange_manager.storage_manager.orders_storage.get_startup_order_details(
+        order.exchange_order_id
+    )
     if order_details:
         order.update_from_storage_order_details(order_details)
         await create_orders_storage_related_elements(order, order_details, exchange_manager, pending_groups)
 
 
 async def create_orders_storage_related_elements(order, order_storage_details, exchange_manager, pending_groups):
     group = group_util.get_or_create_order_group_from_storage_order_details(order_storage_details, exchange_manager)
     if group:
         order.add_to_order_group(group)
+        logging.get_logger(LOGGER_NAME).debug(f"Adding {order} to restored group {group}")
         pending_groups[group.name] = group
     await order_factory.restore_chained_orders_from_storage_order_details(
         order, order_storage_details, exchange_manager, pending_groups
     )
 
 
 async def _create_storage_self_managed_orders_from_group(pending_group_id, exchange_manager, pending_groups):
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/cancel_order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/cancel_order_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
 
             # set cancel time
             self.order.canceled_time = self.order.exchange_manager.exchange.get_exchange_current_time()
 
             # update portfolio after close
             async with self.order.exchange_manager.exchange_personal_data.portfolio_manager.portfolio.lock:
                 self.ensure_not_cleared(self.order)
-                await self.order.exchange_manager.exchange_personal_data.handle_portfolio_update_from_order(self.order,
-                                                                                                            False)
+                await self.order.exchange_manager.exchange_personal_data.\
+                    handle_portfolio_and_position_update_from_order(self.order, False)
 
             # notify order cancelled
             await self.order.exchange_manager.exchange_personal_data.handle_order_update_notification(
                 self.order, enums.OrderUpdateType.STATE_CHANGE
             )
 
             # set close state
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/close_order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/fill_order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/fill_order_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,16 +101,16 @@
                     await self.order.order_group.on_fill(self.order)
 
                 # always make sure this order has not been cleared when the is a risk to avoid AttributeError
                 self.ensure_not_cleared(self.order)
                 # update portfolio with filled order and position if any
                 async with self.order.exchange_manager.exchange_personal_data.portfolio_manager.portfolio.lock:
                     self.ensure_not_cleared(self.order)
-                    await self.order.exchange_manager.exchange_personal_data.handle_portfolio_update_from_order(
-                        self.order)
+                    await self.order.exchange_manager.exchange_personal_data.\
+                        handle_portfolio_and_position_update_from_order(self.order)
 
                 # notify order filled
                 await self.order.exchange_manager.exchange_personal_data.handle_order_update_notification(
                     self.order, enums.OrderUpdateType.STATE_CHANGE
                 )
 
                 # call order on_filled callback
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/open_order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/order_state_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/states/pending_creation_order_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/states/pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/limit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/limit/take_profit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/limit/take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/buy_market_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/market_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/market/sell_market_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/market/sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/unknown_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/orders/types/unsupported_order.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/orders/types/unsupported_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/asset.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/future_asset.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/margin_asset.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/assets/spot_asset.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/assets/spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/balance.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/balance_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/balance_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/historical_asset_value.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/historical_asset_value.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,25 +73,26 @@
         if not self._is_initialized_event_set:
             self._set_initialized_event()
             self._is_initialized_event_set = True
         return changed
 
     async def handle_balance_update_from_order(self, order, require_exchange_update: bool) -> bool:
         """
-        Handle a balance update from an order request
+        Handle a balance update from an order update
         :param order: the order
         :param require_exchange_update: when True, will sync with exchange portfolio, otherwise will predict the
         portfolio changes using order data (as in trading simulator)
         :return: True if the portfolio was updated
         """
         if self.trader.is_enabled:
             async with self.portfolio_history_update():
                 if self.trader.simulate or not require_exchange_update:
                     return self._refresh_simulated_trader_portfolio_from_order(order)
-                # on real trading: reload portfolio to ensure portfolio sync
+                # on real trading only:
+                # reload portfolio to ensure portfolio sync
                 return await self._refresh_real_trader_portfolio()
         return False
 
     async def handle_balance_update_from_funding(self, position, funding_rate, require_exchange_update: bool) -> bool:
         """
         Handle a balance update from a funding update
         :param position: the position
@@ -201,17 +202,17 @@
                                  update_origin_crypto_currencies_values(symbol, mark_price))
 
     async def _refresh_real_trader_portfolio(self) -> bool:
         """
         Call BALANCE_CHANNEL producer to refresh real trader portfolio
         :return: True if the portfolio was updated
         """
-        return await exchange_channel.get_chan(constants.BALANCE_CHANNEL,
-                                               self.exchange_manager.id).get_internal_producer().\
-            refresh_real_trader_portfolio()
+        return await exchange_channel.get_chan(
+            constants.BALANCE_CHANNEL, self.exchange_manager.id
+        ).get_internal_producer().refresh_real_trader_portfolio()
 
     async def reset_history(self):
         if self.trader.simulate:
             # reset simulated portfolio
             # save not_available assets to reapply them
             previous_assets = self.portfolio.portfolio
             self._load_portfolio(True)
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_profitability.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/portfolio_value_holder.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/sub_portfolio.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/sub_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/future_portfolio.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/future_portfolio.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,18 @@
 
 class FuturePortfolio(portfolio_class.Portfolio):
     def create_currency_asset(self, currency, available=constants.ZERO, total=constants.ZERO):
         return future_asset.FutureAsset(name=currency, available=available, total=total)
 
     def update_portfolio_data_from_order(self, order):
         """
-        Call update_portfolio_data for order currency and market
+        Nothing to do on futures, the portfolio will be updated once the position is updated
+        from the order.
         :param order: the order that updated the portfolio
         """
-        # Don't update if order filled quantity is null
-        if order.filled_quantity == 0:
-            return False
-
-        position_instance = order.exchange_manager.exchange_personal_data.positions_manager.get_order_position(
-            order, contract=order.exchange_manager.exchange.get_pair_future_contract(order.symbol))
-        position_instance.update_from_order(order)
 
     def update_portfolio_data_from_withdrawal(self, amount, currency):
         """
         Call update_portfolio_data for order currency and market
         :param amount: the withdrawal amount
         :param currency: the withdrawal currency
         """
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/margin_portfolio.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/types/spot_portfolio.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/types/spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/portfolios/value_converter.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/portfolios/value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/positions.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/trades.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,53 +11,54 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 
+import async_channel.constants as channel_constants
+
 import octobot_trading.exchange_channel as exchanges_channel
 import octobot_trading.enums as enums
 
 
-class PositionsProducer(exchanges_channel.ExchangeChannelProducer):
-    async def push(self, positions):
-        await self.perform(positions)
+class TradesProducer(exchanges_channel.ExchangeChannelProducer):
+    async def push(self, trades, old_trade=False):
+        await self.perform(trades, old_trade=old_trade)
 
-    async def perform(self, positions):
+    async def perform(self, trades, old_trade=False):
         try:
-            for position in positions:
-                if not position:
+            for trade in trades:
+                if not trade:
                     continue
-                symbol: str = position[enums.ExchangeConstantsPositionColumns.SYMBOL.value]
-                changed = await self.channel.exchange_manager.exchange_personal_data. \
-                    handle_position_update(symbol=symbol,
-                                           side=position[enums.ExchangeConstantsPositionColumns.SIDE.value],
-                                           position=position,
-                                           should_notify=False)
-
-                if changed:
-                    await self.send(cryptocurrency=self.channel.exchange_manager.exchange.
-                                    get_pair_cryptocurrency(symbol),
-                                    symbol=symbol,
-                                    position=position,
-                                    is_updated=changed)
+                symbol: str = self.channel.exchange_manager.get_exchange_symbol(
+                    trade[enums.ExchangeConstantsOrderColumns.SYMBOL.value])
+                if self.channel.get_filtered_consumers(symbol=channel_constants.CHANNEL_WILDCARD) or \
+                        self.channel.get_filtered_consumers(symbol=symbol):
+                    trade_id: str = trade[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value]
+
+                    await self.channel.exchange_manager.exchange_personal_data.handle_trade_update(
+                        symbol,
+                        trade_id,
+                        trade,
+                        is_old_trade=old_trade,
+                        should_notify=True)
         except asyncio.CancelledError:
             self.logger.info("Update tasks cancelled.")
         except Exception as e:
             self.logger.exception(e, True, f"Exception when triggering update: {e}")
 
-    async def send(self, cryptocurrency, symbol, position, is_updated=False):
+    async def send(self, cryptocurrency, symbol, trade, old_trade=False):
         for consumer in self.channel.get_filtered_consumers(symbol=symbol):
             await consumer.queue.put({
                 "exchange": self.channel.exchange_manager.exchange_name,
                 "exchange_id": self.channel.exchange_manager.id,
                 "cryptocurrency": cryptocurrency,
                 "symbol": symbol,
-                "position": position,
-                "is_updated": is_updated
+                "trade": trade,
+                "old_trade": old_trade
             })
 
 
-class PositionsChannel(exchanges_channel.ExchangeChannel):
-    PRODUCER_CLASS = PositionsProducer
+class TradesChannel(exchanges_channel.ExchangeChannel):
+    PRODUCER_CLASS = TradesProducer
     CONSUMER_CLASS = exchanges_channel.ExchangeChannelConsumer
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/positions_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/positions_updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,26 @@
     POSITIONS_STARTING_REFRESH_TIME = 12
     POSITION_REFRESH_TIME = 9
     TIME_BETWEEN_POSITIONS_REFRESH = 3
 
     def __init__(self, channel):
         super().__init__(channel)
         # create async jobs
-        self.position_update_job = async_job.AsyncJob(self.fetch_and_push_positions,
-                                                      execution_interval_delay=self.POSITION_REFRESH_TIME,
-                                                      min_execution_delay=self.TIME_BETWEEN_POSITIONS_REFRESH)
+        self.positions_update_job = async_job.AsyncJob(
+            self.fetch_and_push_positions,
+            execution_interval_delay=self.POSITION_REFRESH_TIME,
+            min_execution_delay=self.TIME_BETWEEN_POSITIONS_REFRESH
+        )
+        self.position_update_job = async_job.AsyncJob(
+            self._position_fetch_and_push,
+            is_periodic=False,
+            enable_multiple_runs=True
+        )
+        self.position_update_job.add_job_dependency(self.positions_update_job)
+        self.positions_update_job.add_job_dependency(self.position_update_job)
 
     async def initialize(self) -> None:
         """
         Initialize positions and future contracts
         """
         # fetch future contracts from exchange
         await self.initialize_contracts()
@@ -97,15 +106,15 @@
         Start updater jobs
         """
         if not self._should_run():
             return
 
         await self.initialize()
         await asyncio.sleep(self.POSITIONS_STARTING_REFRESH_TIME)
-        await self.position_update_job.run()
+        await self.positions_update_job.run()
 
     async def fetch_and_push(self):
         """
         Update positions from exchange
         """
         await self.fetch_and_push_positions()
         await asyncio.sleep(self.TIME_BETWEEN_POSITIONS_REFRESH)
@@ -113,21 +122,24 @@
     def _should_run(self):
         return self.channel.exchange_manager.is_future
 
     def _is_relevant_position(self, position_dict):
         return position_dict and position_dict.get(enums.ExchangeConstantsPositionColumns.SYMBOL.value, None) \
                in self.channel.exchange_manager.exchange_config.traded_symbol_pairs
 
-    async def fetch_and_push_positions(self):
+    async def fetch_and_push_positions(self, retry_attempts=1):
         """
         Update positions from exchange
         """
         symbols = self.channel.exchange_manager.exchange_config.traded_symbol_pairs \
             if self.channel.exchange_manager.exchange.REQUIRES_SYMBOL_FOR_EMPTY_POSITION else None
-        positions = await self.channel.exchange_manager.exchange.get_positions(symbols=symbols)
+        positions = await self.channel.exchange_manager.exchange.retry_n_time(
+            retry_attempts,
+            self.channel.exchange_manager.exchange.get_positions, symbols=symbols,
+        )
         if positions:
             relevant_positions = [
                 position
                 for position in positions
                 if self._is_relevant_position(position)
             ]
             # initialize relevant contracts first as they might be waited for
@@ -143,15 +155,15 @@
         if self._should_push_mark_price():
             for position in positions:
                 await self.extract_mark_price(position)
 
     async def _update_positions_contract_settings(self, positions):
         for position in positions:
             symbol = position.get(enums.ExchangeConstantsPositionColumns.SYMBOL.value, None)
-            if symbol is not None:
+            if symbol is not None and symbol in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
                 await self._update_contract_settings(symbol)
 
     async def _update_contract_settings(self, symbol):
         try:
             if constants.FORCED_MARGIN_TYPE:
                 await self.channel.exchange_manager.trader.set_margin_type(
                     symbol, enums.PositionSide.BOTH, constants.FORCED_MARGIN_TYPE
@@ -171,26 +183,43 @@
             self.logger.exception(e, True, f"Fail to update mark price from position : {e}")
 
     async def update_position_from_exchange(self, position,
                                             should_notify=False,
                                             wait_for_refresh=False,
                                             force_job_execution=False,
                                             create_position_producer_if_missing=True):
+        await self.position_update_job.run(force=True, wait_for_task_execution=wait_for_refresh,
+                                           ignore_dependencies_check=force_job_execution,
+                                           position=position, should_notify=should_notify)
+
+    async def _position_fetch_and_push(self, position, should_notify=False):
         """
-        Trigger position job refresh from exchange
+        Update Position from exchange
         :param position: the position to update
-        :param wait_for_refresh: if True, wait until the position refresh task to finish
         :param should_notify: if Positions channel consumers should be notified
-        :param force_job_execution: When True, position_update_job will bypass its dependencies check
-        :param create_position_producer_if_missing: Should be set to False when called by self to prevent spamming
         :return: True if the position was updated
         """
-        await self.position_update_job.run(force=True, wait_for_task_execution=wait_for_refresh,
-                                           ignore_dependencies_check=force_job_execution,
-                                           position=position, should_notify=should_notify)
+        exchange_name = self.channel.exchange_manager.exchange_name
+        self.logger.debug(f"Requested update for position: {position} on {exchange_name}")
+        raw_position = await self.channel.exchange_manager.exchange.get_position(position.symbol)
+
+        if raw_position:
+            self.logger.debug(f"Received update for {position} on {exchange_name}: {raw_position}")
+
+            await self.channel.exchange_manager.exchange_personal_data.handle_position_update(
+                symbol=raw_position[enums.ExchangeConstantsPositionColumns.SYMBOL.value],
+                side=raw_position[enums.ExchangeConstantsPositionColumns.SIDE.value],
+                position=raw_position,
+                should_notify=should_notify
+            )
+        else:
+            self.logger.debug(
+                f"Can't received update for {position} on {exchange_name}: received position is {raw_position}"
+            )
+
 
     def _should_push_mark_price(self):
         return self._has_mark_price_in_position()
 
     def _has_mark_price_in_position(self):
         return self.channel.exchange_manager.exchange.MARK_PRICE_IN_POSITION
 
@@ -208,14 +237,15 @@
     async def stop(self) -> None:
         """
         Stop producer by stopping its jobs
         """
         await super().stop()
         if not self._should_run():
             return
+        self.positions_update_job.stop()
         self.position_update_job.stop()
 
     async def resume(self) -> None:
         """
         Resume producer by restarting its jobs
         """
         await super().resume()
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
             raise errors.InvalidPosition(f"This position requires a "
                                          f"{'inverse' if symbol_contract.is_inverse_contract else 'linear'} contract")
         self.trader = trader
         self.exchange_manager = trader.exchange_manager
         self.simulated = trader.simulate
 
         self.logger_name = None
-        self.position_id = None
+        self.position_id = None             # position id within OctoBot
+        self.exchange_position_id = None    # position id as fetched from exchange, local to the user account
         self.timestamp = 0
         self.symbol = None
         self.currency, self.market = None, None
         self.status = enums.PositionStatus.OPEN
         self.side = enums.PositionSide.UNKNOWN
 
         # Contract
@@ -124,24 +125,27 @@
         """
         self.state = positions_states.LiquidatePositionState(self, is_from_exchange_data=is_from_exchange_data)
 
     def _should_change(self, original_value, new_value):
         if new_value is not None and original_value != new_value:
             return True
 
-    def _update(self, position_id, symbol, currency, market, timestamp,
+    def _update(self, position_id, exchange_position_id, symbol, currency, market, timestamp,
                 entry_price, mark_price, liquidation_price,
                 quantity, size, value, initial_margin,
                 unrealized_pnl, realised_pnl, fee_to_close,
                 status=None):
         changed: bool = False
 
         if self._should_change(self.position_id, position_id):
             self.position_id = position_id
 
+        if self._should_change(self.exchange_position_id, exchange_position_id):
+            self.exchange_position_id = exchange_position_id
+
         if self._should_change(self.symbol, symbol):
             self.symbol, self.currency, self.market = symbol, currency, market
 
         if self._should_change(self.timestamp, timestamp):
             self.timestamp = timestamp
         if not self.timestamp:
             if not timestamp:
@@ -728,15 +732,16 @@
             liquidation_price=raw_position.get(enums.ExchangeConstantsPositionColumns.LIQUIDATION_PRICE.value,
                                                constants.ZERO),
             quantity=raw_position.get(enums.ExchangeConstantsPositionColumns.QUANTITY.value, constants.ZERO),
             size=raw_position.get(enums.ExchangeConstantsPositionColumns.SIZE.value, constants.ZERO),
             value=raw_position.get(enums.ExchangeConstantsPositionColumns.NOTIONAL.value, constants.ZERO),
             initial_margin=raw_position.get(enums.ExchangeConstantsPositionColumns.INITIAL_MARGIN.value,
                                             constants.ZERO),
-            position_id=str(raw_position.get(enums.ExchangeConstantsPositionColumns.ID.value, None) or symbol),
+            position_id=self.position_id or symbol,
+            exchange_position_id=str(raw_position.get(enums.ExchangeConstantsPositionColumns.ID.value, None) or symbol),
             timestamp=raw_position.get(enums.ExchangeConstantsPositionColumns.TIMESTAMP.value, 0),
             unrealized_pnl=raw_position.get(enums.ExchangeConstantsPositionColumns.UNREALIZED_PNL.value,
                                             constants.ZERO),
             realised_pnl=raw_position.get(enums.ExchangeConstantsPositionColumns.REALISED_PNL.value, constants.ZERO),
             fee_to_close=raw_position.get(enums.ExchangeConstantsPositionColumns.CLOSING_FEE.value, constants.ZERO),
             status=position_util.parse_position_status(raw_position)
         )
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 
-import octobot_trading.constants
 import octobot_trading.enums as enums
-import octobot_trading.errors
-import octobot_trading.exchange_channel as exchange_channel
 import octobot_trading.personal_data.state as state_class
 
 
 class PositionState(state_class.State):
     def __init__(self, position, is_from_exchange_data):
         super().__init__(is_from_exchange_data)
 
@@ -60,19 +57,16 @@
 
     async def _synchronize_with_exchange(self, force_synchronization: bool = False) -> None:
         """
         Ask PositionsChannel Internal producer to refresh the position from the exchange
         :param force_synchronization: When True, for the update of the position from the exchange
         :return: the result of PositionsProducer.update_position_from_exchange()
         """
-        return (await exchange_channel.get_chan(octobot_trading.constants.POSITIONS_CHANNEL,
-                                                self.position.exchange_manager.id).get_internal_producer().
-                update_position_from_exchange(position=self.position,
-                                              wait_for_refresh=True,
-                                              force_job_execution=force_synchronization))
+        return self.position.exchange_manager.exchange_personal_data.positions_manager.\
+            refresh_real_trader_position(self.position, force_job_execution=force_synchronization)
 
     def set_is_changing_state(self):
         if not self._has_state_changed.is_set():
             self._has_state_changed.set()
 
     def __del__(self):
         """
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/position_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/position_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/active_position_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/active_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/idle_position_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/idle_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/liquidate_position_state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/liquidate_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/states/position_state_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/states/position_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/inverse_position.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/positions/types/linear_position.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/positions/types/linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/state.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/trades.py` & `OctoBot-Trading-2.4.5/octobot_trading/supervisors/abstract_portfolio_supervisor.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,56 +9,44 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import asyncio
-
-import async_channel.constants as channel_constants
-
+import octobot_trading.constants as trading_constants
 import octobot_trading.exchange_channel as exchanges_channel
-import octobot_trading.enums as enums
-
-
-class TradesProducer(exchanges_channel.ExchangeChannelProducer):
-    async def push(self, trades, old_trade=False):
-        await self.perform(trades, old_trade=old_trade)
-
-    async def perform(self, trades, old_trade=False):
-        try:
-            for trade in trades:
-                if not trade:
-                    continue
-                symbol: str = self.channel.exchange_manager.get_exchange_symbol(
-                    trade[enums.ExchangeConstantsOrderColumns.SYMBOL.value])
-                if self.channel.get_filtered_consumers(symbol=channel_constants.CHANNEL_WILDCARD) or \
-                        self.channel.get_filtered_consumers(symbol=symbol):
-                    trade_id: str = trade[enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value]
-
-                    await self.channel.exchange_manager.exchange_personal_data.handle_trade_update(
-                        symbol,
-                        trade_id,
-                        trade,
-                        is_old_trade=old_trade,
-                        should_notify=True)
-        except asyncio.CancelledError:
-            self.logger.info("Update tasks cancelled.")
-        except Exception as e:
-            self.logger.exception(e, True, f"Exception when triggering update: {e}")
-
-    async def send(self, cryptocurrency, symbol, trade, old_trade=False):
-        for consumer in self.channel.get_filtered_consumers(symbol=symbol):
-            await consumer.queue.put({
-                "exchange": self.channel.exchange_manager.exchange_name,
-                "exchange_id": self.channel.exchange_manager.id,
-                "cryptocurrency": cryptocurrency,
-                "symbol": symbol,
-                "trade": trade,
-                "old_trade": old_trade
-            })
+import octobot_trading.supervisors.abstract_supervisor as abstract_supervisor
 
 
-class TradesChannel(exchanges_channel.ExchangeChannel):
-    PRODUCER_CLASS = TradesProducer
-    CONSUMER_CLASS = exchanges_channel.ExchangeChannelConsumer
+class AbstractPortfolioSupervisor(abstract_supervisor.AbstractSupervisor):
+    @staticmethod
+    def is_backtestable() -> bool:
+        return True
+
+    async def initialize(self) -> None:
+        """
+        Initialize balance channel consumer
+        """
+        self.consumers.append(await exchanges_channel.get_chan(
+            trading_constants.BALANCE_CHANNEL, self.exchange_manager.id).new_consumer(self.on_balance_update))
+        self.consumers.append(await exchanges_channel.get_chan(
+            trading_constants.BALANCE_PROFITABILITY_CHANNEL, self.exchange_manager.id).new_consumer(
+            self.on_balance_profitability_update))
+
+    async def on_balance_update(self, exchange: str, exchange_id: str, balance):
+        """
+        Should be overwritten
+        """
+
+    async def on_balance_profitability_update(
+            self,
+            exchange: str,
+            exchange_id: str,
+            profitability,
+            profitability_percent,
+            market_profitability_percent,
+            initial_portfolio_current_profitability,
+    ):
+        """
+        Should be overwritten
+        """
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/channel/trades_updater.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/channel/trades_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trade.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trade_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trade_pnl.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trades_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/trades/trades_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/trades/trades_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/transaction.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/transaction_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/transactions_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/blockchain_transaction.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/blockchain_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/fee_transaction.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/fee_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/personal_data/transactions/types/transfer_transaction.py` & `OctoBot-Trading-2.4.5/octobot_trading/personal_data/transactions/types/transfer_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/channel/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/channel/remote_trading_signal.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/channel/remote_trading_signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/channel/signal_producer.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/channel/signal_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/signal_creation.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/signal_creation.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/signals/util.py` & `OctoBot-Trading-2.4.5/octobot_trading/signals/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/abstract_storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/candles_storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/candles_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/orders_storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/orders_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,22 +94,21 @@
             storage_util.get_account_type_suffix_from_exchange_manager(self.exchange_manager),
             self.exchange_manager.exchange_name,
         )
 
     async def get_historical_orders_updates(self):
         return copy.deepcopy(await self._get_db().all(self.HISTORICAL_OPEN_ORDERS_TABLE))
 
-    async def get_startup_order_details(self, order_id):
-        return self.startup_orders.get(order_id, None)
+    async def get_startup_order_details(self, order_exchange__id):
+        return self.startup_orders.get(order_exchange__id, None)
 
     async def _load_startup_orders(self):
         if self.should_store_date():
             self.startup_orders = {
-                order[OrdersStorage.ORIGIN_VALUE_KEY][enums.ExchangeConstantsOrderColumns.ID.value]:
-                    self._from_order_document(order)
+                _get_startup_order_key(order): self._from_order_document(order)
                 for order in copy.deepcopy(await self._get_db().all(self.HISTORY_TABLE))
                 if order    # skip empty order details (error when serializing)
             }
         else:
             self.startup_orders = {}
 
     def get_startup_self_managed_orders_details_from_group(self, group_id):
@@ -217,7 +216,12 @@
             # ensure order details are present in open orders
             details = {
                 OrdersStorage.ORIGIN_VALUE_KEY: OrdersStorage.sanitize_for_storage(order_dict),
             }
     order_update[enums.StoredOrdersAttr.ORDER_DETAILS.value] = details
     return order_update
 
+
+def _get_startup_order_key(order_dict):
+    # use exchange id if available, fallback to order_id (for self managed orders)
+    return order_dict[OrdersStorage.ORIGIN_VALUE_KEY][enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] or \
+        order_dict[OrdersStorage.ORIGIN_VALUE_KEY][enums.ExchangeConstantsOrderColumns.ID.value]
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/portfolio_storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/portfolio_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/storage_manager.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/trades_storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/trades_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/transactions_storage.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/transactions_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/storage/util.py` & `OctoBot-Trading-2.4.5/octobot_trading/storage/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/supervisors/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/supervisors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/supervisors/abstract_supervisor.py` & `OctoBot-Trading-2.4.5/octobot_trading/supervisors/abstract_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 )
 from octobot_trading.util.config_util import (
     is_trader_enabled,
     is_trader_simulator_enabled,
     is_trade_history_loading_enabled,
     is_currency_enabled,
     get_symbols,
+    get_symbol_trading_type,
+    get_symbol_types_counts,
     get_all_currencies,
     get_pairs,
     get_market_pair,
     get_reference_market,
     get_traded_pairs_by_currency,
     get_current_bot_live_id,
 )
@@ -52,14 +54,16 @@
     "resume_time_consumer",
     "Initializable",
     "is_trader_enabled",
     "is_trader_simulator_enabled",
     "is_trade_history_loading_enabled",
     "is_currency_enabled",
     "get_symbols",
+    "get_symbol_trading_type",
+    "get_symbol_types_counts",
     "get_all_currencies",
     "get_pairs",
     "get_market_pair",
     "get_reference_market",
     "get_traded_pairs_by_currency",
     "get_current_bot_live_id",
 ]
```

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/initializable.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/initializable.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/initialization_util.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/initialization_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/simulator_updater_utils.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/simulator_updater_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/__init__.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/exchanges_test_tools.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/exchanges_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/octobot_trading/util/test_tools/websocket_test_tools.py` & `OctoBot-Trading-2.4.5/octobot_trading/util/test_tools/websocket_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/requirements.txt` & `OctoBot-Trading-2.4.5/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 OctoBot-Backtesting>=1.9, <1.10
 Async-Channel>=2.2, <2.3
 OctoBot-Commons>=1.9, <1.10
 OctoBot-Tentacles-Manager>=2.9, <2.10
 trading-backend>=1.2.3
 
 # Exchange connection requirements
-ccxt==3.0.74 # always ensure real exchanges tests (in tests_additional and authenticated exchange tests) are passing before changing the ccxt version
+ccxt==3.1.52 # always ensure real exchanges tests (in tests_additional and authenticated exchange tests) are passing before changing the ccxt version
 
 cryptography # Never specify a version (managed by https://github.com/Drakkar-Software/OctoBot-PyPi-Linux-Deployer)
 
 # OrderBook requirement
 sortedcontainers==2.4.0
 
 # Scripting requirements
```

### Comparing `OctoBot-Trading-2.4.4/setup.py` & `OctoBot-Trading-2.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/__init__.py` & `OctoBot-Trading-2.4.5/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_channels.py` & `OctoBot-Trading-2.4.5/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_exchange.py` & `OctoBot-Trading-2.4.5/tests/api/test_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_modes.py` & `OctoBot-Trading-2.4.5/tests/api/test_modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_orders.py` & `OctoBot-Trading-2.4.5/tests/api/test_orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_portfolio.py` & `OctoBot-Trading-2.4.5/tests/api/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_profitability.py` & `OctoBot-Trading-2.4.5/tests/api/test_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_symbol_data.py` & `OctoBot-Trading-2.4.5/tests/api/test_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_trader.py` & `OctoBot-Trading-2.4.5/tests/api/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/api/test_trades.py` & `OctoBot-Trading-2.4.5/tests/api/test_trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/cli/__init__.py` & `OctoBot-Trading-2.4.5/tests/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/contracts/test_future_contract.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/contracts/test_future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/contracts/test_margin_contract.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/contracts/test_margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/funding/test_funding_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/funding/test_funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/kline/test_kline_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/kline/test_kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/test_candles_adapter.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/test_candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/ohlcv/test_candles_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/ohlcv/test_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/order_book/test_order_book_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/order_book/test_order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/prices/test_price_events_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/prices/test_price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/prices/test_prices_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/prices/test_prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/recent_trades/test_recent_trades_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/recent_trades/test_recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/test_exchange_symbols_data.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/test_exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchange_data/ticker/test_ticker_manager.py` & `OctoBot-Trading-2.4.5/tests/exchange_data/ticker/test_ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchanges/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import contextlib
 import os
 import mock
 import pytest
 import pytest_asyncio
 
 import octobot_commons.constants as commons_constants
 from octobot_backtesting.backtesting import Backtesting
@@ -24,27 +25,77 @@
 import octobot_backtesting.time as backtesting_time
 from octobot_commons.asyncio_tools import wait_asyncio_next_cycle
 from octobot_commons.enums import TimeFrames
 
 from octobot_commons.tests.test_config import load_test_config
 from octobot_trading.api.exchange import create_exchange_builder, cancel_ccxt_throttle_task
 from octobot_trading.exchanges.exchange_manager import ExchangeManager
+from octobot_trading.exchanges.implementations.default_rest_exchange import DefaultRestExchange
+from octobot_trading.exchanges.connectors.ccxt.ccxt_connector import CCXTConnector
 from octobot_trading.exchanges.traders.trader_simulator import TraderSimulator
 import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import FeePropertyColumns, ExchangeConstantsMarketPropertyColumns, \
     ExchangeConstantsMarketPropertyColumns
 
 pytestmark = pytest.mark.asyncio
 
 TESTS_FOLDER = "tests"
 TESTS_STATIC_FOLDER = os.path.join(TESTS_FOLDER, "static")
 DEFAULT_EXCHANGE_NAME = "binanceus"
 DEFAULT_FUTURE_EXCHANGE_NAME = "bybit"
 
 
+class MockedCCXTConnector(CCXTConnector):
+    @classmethod
+    def get_name(cls):
+        return DEFAULT_EXCHANGE_NAME
+
+
+class MockedRestExchange(DefaultRestExchange):
+    DEFAULT_CONNECTOR_CLASS = MockedCCXTConnector
+
+    @classmethod
+    def get_exchange_connector_class(cls, exchange_manager):
+        return cls.DEFAULT_CONNECTOR_CLASS
+
+    @classmethod
+    def is_default_exchange(cls) -> bool:
+        return False
+
+
+class MockedAutoFillRestExchange(MockedRestExchange):
+    HAS_FETCHED_DETAILS = True
+    _SUPPORTED_EXCHANGE_MOCK = []
+    _EXCHANGE_DETAILS_MOCK = {}
+
+    def _fetch_details(self, config, exchange_manager):
+        pass
+
+    @staticmethod
+    def supported_autofill_exchanges(tentacle_config):
+        return MockedAutoFillRestExchange._SUPPORTED_EXCHANGE_MOCK
+
+    @classmethod
+    async def get_autofilled_exchange_details(cls, aiohttp_session, tentacle_config, exchange_name):
+        return MockedAutoFillRestExchange._EXCHANGE_DETAILS_MOCK[exchange_name]
+
+    @classmethod
+    @contextlib.contextmanager
+    def patched_supported_exchanges(cls, exchange_details_by_exchange_name):
+        previous_exchanges = cls._SUPPORTED_EXCHANGE_MOCK
+        previous_details = cls._EXCHANGE_DETAILS_MOCK
+        try:
+            cls._SUPPORTED_EXCHANGE_MOCK = list(exchange_details_by_exchange_name)
+            cls._EXCHANGE_DETAILS_MOCK = exchange_details_by_exchange_name
+            yield
+        finally:
+            cls._SUPPORTED_EXCHANGE_MOCK = previous_exchanges
+            cls._EXCHANGE_DETAILS_MOCK = previous_details
+
+
 @pytest_asyncio.fixture
 async def exchange_manager():
     exchange_manager_instance = ExchangeManager(load_test_config(), DEFAULT_EXCHANGE_NAME)
     exchange_manager_instance.is_spot_only = True
     exchange_manager_instance.is_simulated = False
     await exchange_manager_instance.initialize()
     try:
```

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/connectors/ccxt/test_ccxt_connector.py` & `OctoBot-Trading-2.4.5/tests/exchanges/connectors/ccxt/test_ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/implementations/test_default_rest_exchange.py` & `OctoBot-Trading-2.4.5/tests/exchanges/implementations/test_default_rest_exchange.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,34 +14,20 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import octobot_trading.exchanges as exchanges
 import octobot_commons.enums as commons_enums
 import pytest
 
-from tests.exchanges import exchange_manager, DEFAULT_EXCHANGE_NAME
+from tests.exchanges import exchange_manager, DEFAULT_EXCHANGE_NAME, MockedRestExchange
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class MockedCCXTConnector(exchanges.CCXTConnector):
-    @classmethod
-    def get_name(cls):
-        return DEFAULT_EXCHANGE_NAME
-
-
-class MockedRestExchange(exchanges.DefaultRestExchange):
-    DEFAULT_CONNECTOR_CLASS = MockedCCXTConnector
-
-    @classmethod
-    def get_exchange_connector_class(cls, exchange_manager):
-        return cls.DEFAULT_CONNECTOR_CLASS
-
-
 @pytest.fixture
 def default_rest_exchange(exchange_manager):
     return MockedRestExchange(exchange_manager.config, exchange_manager)
 
 
 async def test_start_request_data_and_stop(default_rest_exchange):
     await default_rest_exchange.initialize()
```

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/implementations/test_default_websocket_exchange.py` & `OctoBot-Trading-2.4.5/tests/exchanges/implementations/test_default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_abstract_exchange.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_abstract_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,17 @@
 
 
 async def test_supports_bundled_order_on_order_creation(abstract_exchange):
     order_mock = mock.Mock()
     order_mock.order_type = enums.TraderOrderType.SELL_MARKET
     assert abstract_exchange.supports_bundled_order_on_order_creation(order_mock, enums.TraderOrderType.STOP_LOSS) \
            is False
-    abstract_exchange.SUPPORTED_BUNDLED_ORDERS[enums.TraderOrderType.SELL_MARKET] = [enums.TraderOrderType.SELL_MARKET,
-                                                                                     enums.TraderOrderType.BUY_LIMIT]
+    abstract_exchange.get_supported_elements(enums.ExchangeSupportedElements.SUPPORTED_BUNDLED_ORDERS)[
+        enums.TraderOrderType.SELL_MARKET
+    ] = [enums.TraderOrderType.SELL_MARKET, enums.TraderOrderType.BUY_LIMIT]
     assert abstract_exchange.supports_bundled_order_on_order_creation(order_mock, enums.TraderOrderType.STOP_LOSS) \
            is False
     assert abstract_exchange.supports_bundled_order_on_order_creation(order_mock, enums.TraderOrderType.BUY_LIMIT) \
            is True
 
 
 async def test_get_order_additional_params(abstract_exchange):
```

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_basic_exchange_wrapper.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,50 +10,54 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import pytest
-import pytest_asyncio
-import mock
-import ccxt.async_support
 
+from octobot_commons.errors import ConfigTradingError
 
-import octobot_trading.exchanges as exchanges
-import octobot_trading.exchanges.connectors.ccxt.enums as ccxt_enums
+# Import required fixtures
+from tests import event_loop, install_tentacles
+from tests.exchanges import exchange_builder
+from octobot_trading.api.exchange import cancel_ccxt_throttle_task
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-@pytest_asyncio.fixture
-async def basic_exchange_wrapper():
-    async with exchanges.temporary_exchange_wrapper("binanceus", ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT) as wrapper:
-        return wrapper
+@pytest.mark.usefixtures("event_loop", "exchange_builder")
+async def test_create_without_trading_config(exchange_builder):
+    with pytest.raises(ConfigTradingError):
+        await exchange_builder.build()
 
 
-async def test_constructor(basic_exchange_wrapper):
-    assert isinstance(basic_exchange_wrapper.exchange, ccxt.async_support.binanceus)
-    async with exchanges.temporary_exchange_wrapper("okx", ccxt_enums.ExchangeWrapperLibs.CCXT) as wrapper:
-        assert isinstance(wrapper.exchange, ccxt.okx)
+@pytest.mark.usefixtures("event_loop", "exchange_builder")
+async def test_create_without_installed_trading_mode(exchange_builder):
+    with pytest.raises(ConfigTradingError):
+        await exchange_builder.build()
 
 
-async def test_temporary_exchange_wrapper():
-    with mock.patch.object(ccxt.async_support.okx, "close", mock.AsyncMock()) as close_mock:
-        with pytest.raises(ZeroDivisionError):
-            async with exchanges.temporary_exchange_wrapper("okx", ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT) as wrapper:
-                assert isinstance(wrapper.exchange, ccxt.async_support.okx)
-                close_mock.assert_not_called()
-                1/0
-        close_mock.assert_called_once()
+@pytest.mark.usefixtures("event_loop", "exchange_builder", "install_tentacles")
+async def test_create_without_installed_trading_mode(exchange_builder):
+    with pytest.raises(ConfigTradingError):
+        await exchange_builder.build()
 
 
-async def test_unsupported_lib():
-    with pytest.raises(NotImplementedError):
-        exchanges.BasicExchangeWrapper("binanceus", "plop")
+@pytest.mark.usefixtures("event_loop", "exchange_builder", "install_tentacles")
+async def test_create(exchange_builder):
+    # await exchange_builder.build() # TODO
+    pass
 
 
-async def test_get_available_time_frames(basic_exchange_wrapper):
-    assert len(await basic_exchange_wrapper.get_available_time_frames()) > 10
-    basic_exchange_wrapper.exchange.timeframes = ["1m"]
-    assert await basic_exchange_wrapper.get_available_time_frames() == ["1m"]
+@pytest.mark.usefixtures("event_loop", "exchange_builder")
+@pytest.mark.parametrize("exchange_builder", [(None, "binanceus")], indirect=["exchange_builder"])
+async def test_create_basic(exchange_builder):
+    exchange_builder.disable_trading_mode()
+    exchange_manager = await exchange_builder.build()
+
+    assert exchange_manager is not None
+    assert exchange_manager.exchange_name == "binanceus"
+
+    cancel_ccxt_throttle_task()
+    await exchange_manager.stop()
```

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_builder.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_config_data.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_manager.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_exchange_simulator.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/test_exchanges.py` & `OctoBot-Trading-2.4.5/tests/exchanges/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/traders/test_trader.py` & `OctoBot-Trading-2.4.5/tests/exchanges/traders/test_trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from octobot_trading.errors import TooManyOpenPositionError, InvalidLeverageValue, OrderEditError
 from octobot_trading.personal_data import LinearPosition
 import octobot_commons.constants as commons_constants
 from octobot_commons.asyncio_tools import wait_asyncio_next_cycle
 from octobot_commons.tests.test_config import load_test_config
 from octobot_trading.personal_data.orders import Order
 from octobot_trading.enums import TraderOrderType, TradeOrderSide, TradeOrderType, OrderStatus, \
-    ExchangeConstantsPositionColumns, PositionMode, MarginType, TakeProfitStopLossMode
+    ExchangeConstantsPositionColumns, PositionMode, MarginType, TakeProfitStopLossMode, ExchangeSupportedElements
 from octobot_trading.exchanges.exchange_manager import ExchangeManager
 from octobot_trading.personal_data.orders.order_factory import create_order_instance, create_order_instance_from_raw
 from octobot_trading.personal_data.orders import BuyLimitOrder, BuyMarketOrder, SellLimitOrder, StopLossOrder
 from octobot_trading.personal_data.orders.types.market.sell_market_order import SellMarketOrder
 import octobot_trading.personal_data.portfolios.assets as portfolio_assets
 import octobot_trading.personal_data.orders.groups as order_groups
 from octobot_trading.exchanges.traders.trader import Trader
@@ -934,15 +934,16 @@
         assert chained_order.trader_creation_kwargs == {"kw1": 1, "kw2": "hello"}
         assert chained_order.is_waiting_for_chained_trigger is True
         assert chained_order.is_created() is False
 
         base_order = BuyLimitOrder(trader_inst)
         chained_order = StopLossOrder(trader_inst)
         # with bundle support
-        exchange_manager.exchange.SUPPORTED_BUNDLED_ORDERS[base_order.order_type] = [chained_order.order_type]
+        exchange_manager.exchange.get_supported_elements(ExchangeSupportedElements.SUPPORTED_BUNDLED_ORDERS)[
+            base_order.order_type] = [chained_order.order_type]
         assert await trader_inst.bundle_chained_order_with_uncreated_order(base_order, chained_order, False, kw1=1, kw2="hello") \
                == {}
         # bundled chained_order to base_order
         assert chained_order in base_order.chained_orders
         assert chained_order.triggered_by is base_order
         assert chained_order.has_been_bundled is True
         assert chained_order.update_with_triggering_order_fees is False
@@ -1062,26 +1063,25 @@
 
 async def test__has_open_position(future_trader_simulator_with_default_linear):
     _, exchange_manager_inst, trader_inst, default_contract = future_trader_simulator_with_default_linear
 
     contract = default_contract
     exchange_manager_inst.exchange.set_pair_future_contract(DEFAULT_FUTURE_SYMBOL, contract)
 
-    if not os.getenv('CYTHON_IGNORE'):
-        assert not trader_inst._has_open_position(DEFAULT_FUTURE_SYMBOL)
+    assert not trader_inst._has_open_position(DEFAULT_FUTURE_SYMBOL)
 
-        position_inst = LinearPosition(trader_inst, contract)
-        await position_inst.initialize()
-        position_inst.update_from_raw(
-            {
-                ExchangeConstantsPositionColumns.SYMBOL.value: DEFAULT_FUTURE_SYMBOL
-            }
-        )
-        exchange_manager_inst.exchange_personal_data.positions_manager.upsert_position_instance(position_inst)
-        assert trader_inst._has_open_position(DEFAULT_FUTURE_SYMBOL)
+    position_inst = LinearPosition(trader_inst, contract)
+    await position_inst.initialize()
+    position_inst.update_from_raw(
+        {
+            ExchangeConstantsPositionColumns.SYMBOL.value: DEFAULT_FUTURE_SYMBOL
+        }
+    )
+    exchange_manager_inst.exchange_personal_data.positions_manager.upsert_position_instance(position_inst)
+    assert trader_inst._has_open_position(DEFAULT_FUTURE_SYMBOL)
 
 
 def make_coroutine(response):
     async def coroutine(*args, **kwargs):
         return response
 
     return coroutine
```

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/types/test_websocket_exchange.py` & `OctoBot-Trading-2.4.5/tests/exchanges/types/test_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.5/tests/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/exchanges/util/test_exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.5/tests/exchanges/util/test_exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/__init__.py` & `OctoBot-Trading-2.4.5/tests/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.5/tests/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/script_keywords/basic_keywords/test_account_balance.py` & `OctoBot-Trading-2.4.5/tests/modes/script_keywords/basic_keywords/test_account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/script_keywords/basic_keywords/test_amount.py` & `OctoBot-Trading-2.4.5/tests/modes/script_keywords/basic_keywords/test_amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.5/tests/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/script_keywords/dsl/test_quantity.py` & `OctoBot-Trading-2.4.5/tests/modes/script_keywords/dsl/test_quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/test_abstract_mode_consumer.py` & `OctoBot-Trading-2.4.5/tests/modes/test_abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/modes/test_abstract_trading_mode.py` & `OctoBot-Trading-2.4.5/tests/modes/test_abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/test_group_util.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/test_group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_cancel_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_close_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_fill_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_open_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_order_state_factory.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/states/test_pending_creation_order_state.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/states/test_pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_decimal_order_adapter.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_double_filled_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_double_filled_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order_adapter.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order_factory.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_order_util.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_orders_manager.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/test_orders_storage_operations.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/test_orders_storage_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,34 +47,35 @@
     mocked_order_storage.should_store_date = mock.Mock(return_value=False)
 
     order = personal_data.BuyLimitOrder(trader_inst)
     order.update(order_type=enums.TraderOrderType.BUY_LIMIT,
                  symbol="BTC/USDT",
                  current_price=decimal.Decimal("70"),
                  quantity=decimal.Decimal("10"),
-                 price=decimal.Decimal("70"))
+                 price=decimal.Decimal("70"),
+                 exchange_order_id="plop exchange_id")
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
     # disabled in trader simulator
     mocked_order_storage.get_startup_order_details.assert_not_awaited()
 
     mocked_order_storage.should_store_date = mock.Mock(return_value=True)
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
-    mocked_order_storage.get_startup_order_details.assert_awaited_once()
+    mocked_order_storage.get_startup_order_details.assert_awaited_once_with("plop exchange_id")
 
     # ensure no crash with not well formatted order_details
     mocked_order_storage.get_startup_order_details = mock.AsyncMock(return_value={"hello": "hi there"})
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
-    mocked_order_storage.get_startup_order_details.assert_awaited_once()
+    mocked_order_storage.get_startup_order_details.assert_awaited_once_with("plop exchange_id")
 
     # ensure order update is done
     assert order.order_id != "new id 123"
     assert order.exchange_order_id != "new exchange id 123"
     mocked_order_storage.get_startup_order_details = mock.AsyncMock(return_value={
         storage.OrdersStorage.ORIGIN_VALUE_KEY: {
             enums.ExchangeConstantsOrderColumns.ID.value: "new id 123",
             enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: "new exchange id 123"
         }
     })
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
-    mocked_order_storage.get_startup_order_details.assert_awaited_once()
+    mocked_order_storage.get_startup_order_details.assert_awaited_once_with("plop exchange_id")
     assert order.order_id == "new id 123"
     assert order.exchange_order_id == "new exchange id 123"
```

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_buy_limit_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_sell_limit_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_stop_loss_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/limit/test_take_profit_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/limit/test_take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/market/test_buy_market_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/market/test_buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/market/test_sell_market_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/market/test_sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/test_unknown_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/test_unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py` & `OctoBot-Trading-2.4.5/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/test_future_asset.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/test_future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/test_margin_asset.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/test_margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/assets/test_spot_asset.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/assets/test_spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_asset.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio_manager.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio_profitability.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_portfolio_value_holder.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/test_value_converter.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/test_value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/test_future_portfolio.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/test_future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/test_margin_portfolio.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/test_margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/portfolios/types/test_spot_portfolio.py` & `OctoBot-Trading-2.4.5/tests/personal_data/portfolios/types/test_spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/test_position.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/test_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/test_position_factory.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/test_position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/test_positions_manager.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/test_positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/types/test_inverse_position.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/types/test_inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/positions/types/test_linear_position.py` & `OctoBot-Trading-2.4.5/tests/personal_data/positions/types/test_linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/trades/test_trade_factory.py` & `OctoBot-Trading-2.4.5/tests/personal_data/trades/test_trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/trades/test_trade_manager.py` & `OctoBot-Trading-2.4.5/tests/personal_data/trades/test_trade_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/trades/test_trade_pnl.py` & `OctoBot-Trading-2.4.5/tests/personal_data/trades/test_trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.5/tests/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/transactions/test_transaction_factory.py` & `OctoBot-Trading-2.4.5/tests/personal_data/transactions/test_transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/personal_data/transactions/test_transactions_manager.py` & `OctoBot-Trading-2.4.5/tests/personal_data/transactions/test_transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/signals/__init__.py` & `OctoBot-Trading-2.4.5/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/signals/test_trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.5/tests/signals/test_trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/signals/test_util.py` & `OctoBot-Trading-2.4.5/tests/signals/test_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/test_utils/order_util.py` & `OctoBot-Trading-2.4.5/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/test_utils/random_numbers.py` & `OctoBot-Trading-2.4.5/tests/test_utils/random_numbers.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/util/__init__.py` & `OctoBot-Trading-2.4.5/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests/util/test_config_util.py` & `OctoBot-Trading-2.4.5/tests/util/test_config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/__init__.py` & `OctoBot-Trading-2.4.5/tests_additional/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/__init__.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/real_exchange_tester.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/real_exchange_tester.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import contextlib
+
 from ccxt import Exchange
 
 import octobot_commons.constants as constants
 import octobot_commons.enums as commons_enums
 import octobot_trading.enums as trading_enums
 from octobot_trading.enums import ExchangeConstantsTickersColumns as Ectc, \
     ExchangeConstantsMarketStatusColumns as Ecmsc
@@ -99,58 +101,56 @@
         return {
             constants.CONFIG_EXCHANGES: {
                 self.EXCHANGE_NAME: {
                     constants.CONFIG_EXCHANGE_TYPE: self.EXCHANGE_TYPE
                 }
             }
         }
+    
+    @contextlib.asynccontextmanager
+    async def get_exchange_manager(self):
+        async with get_exchange_manager(self.EXCHANGE_NAME, config=self.get_config(),
+                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+            yield exchange_manager
 
     async def time_frames(self):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return exchange_manager.exchange.time_frames
 
     async def get_market_statuses(self):
         # return 2 different market status with different traded pairs to reduce possible
         # side effects using only one pair.
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return exchange_manager.exchange.get_market_status(self.SYMBOL), \
                 exchange_manager.exchange.get_market_status(self.SYMBOL_2), \
                 exchange_manager.exchange.get_market_status(self.SYMBOL_3)
 
     async def get_symbol_prices(self, limit=None, **kwargs):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return await exchange_manager.exchange.get_symbol_prices(self.SYMBOL, self.TIME_FRAME,
                                                                      limit=limit, **kwargs)
 
     async def get_kline_price(self, **kwargs):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return await exchange_manager.exchange.get_kline_price(self.SYMBOL, self.TIME_FRAME, **kwargs)
 
     async def get_order_book(self, **kwargs):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return await exchange_manager.exchange.get_order_book(self.SYMBOL, **kwargs)
 
     async def get_recent_trades(self, limit=50):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return await exchange_manager.exchange.get_recent_trades(self.SYMBOL, limit=limit)
 
     async def get_price_ticker(self):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return await exchange_manager.exchange.get_price_ticker(self.SYMBOL)
 
     async def get_all_currencies_price_ticker(self, **kwargs):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config(),
-                                        authenticated=self.REQUIRES_AUTH) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return await exchange_manager.exchange.get_all_currencies_price_ticker(**kwargs)
 
     def get_allowed_time_delta(self):
         return (self.ALLOWED_TIMEFRAMES_WITHOUT_CANDLE + 1) * \
             commons_enums.TimeFramesMinutes[self.TIME_FRAME] * \
             constants.MINUTE_TO_SECONDS * 1.3
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/real_futures_exchange_tester.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/real_futures_exchange_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class RealFuturesExchangeTester(RealExchangeTester):
     EXCHANGE_TYPE = enums.ExchangeTypes.FUTURE.value
 
     async def test_get_funding_rate(self):
         pass
 
     async def get_funding_rate(self, **kwargs):
-        async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config()) as exchange_manager:
+        async with self.get_exchange_manager() as exchange_manager:
             return (
                 await exchange_manager.exchange.get_funding_rate(self.SYMBOL, **kwargs),
                 exchange_manager.exchange.parse_funding(
                     await exchange_manager.exchange.get_price_ticker(self.SYMBOL),
                     from_ticker=True
                 )
             )
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_ascendex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_binance.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitfinex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitfinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitget.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitget.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 assert market_status[Ecmsc.LIMITS.value][Ecmsc.LIMITS_COST.value][val] in (None, 0, 5)
             # can't use normal checker
             # self.check_market_status_limits(market_status, expect_invalid_price_limit_values=True)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 100
+        assert len(symbol_prices) == 1000
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
         symbol_prices = await self.get_symbol_prices(limit=50)
@@ -159,17 +159,17 @@
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
             assert ticker[Ectc.BID.value]
-            assert ticker[Ectc.BID_VOLUME.value] is None
+            assert ticker[Ectc.BID_VOLUME.value]
             assert ticker[Ectc.ASK.value]
-            assert ticker[Ectc.ASK_VOLUME.value] is None
-            assert ticker[Ectc.OPEN.value] is None
+            assert ticker[Ectc.ASK_VOLUME.value]
+            assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
             assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
-            RealExchangeTester.check_ticker_typing(ticker, check_open=False)
+            RealExchangeTester.check_ticker_typing(ticker)
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bithumb.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bithumb.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitso.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitso.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bitstamp.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bitstamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,18 +122,17 @@
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
     async def test_get_all_currencies_price_ticker(self):
-        with pytest.raises(errors.NotSupported):
-            tickers = await self.get_all_currencies_price_ticker()
-            for symbol, ticker in tickers.items():
-                self._check_ticker(ticker, symbol)
+        tickers = await self.get_all_currencies_price_ticker()
+        for symbol, ticker in tickers.items():
+            self._check_ticker(ticker, symbol)
 
     @staticmethod
     def _check_ticker(ticker, symbol, check_content=False):
         assert ticker[Ectc.SYMBOL.value] == symbol
         assert all(key in ticker for key in (
             Ectc.HIGH.value,
             Ectc.LOW.value,
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bittrex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_ndax.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,41 +10,49 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import pytest
-from ccxt.async_support import bittrex
 
 from octobot_commons.enums import TimeFrames, PriceIndexes
+import octobot_trading.errors as errors
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
 from tests_additional.real_exchanges.real_exchange_tester import RealExchangeTester
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestBittrexRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "bittrex"
+class TestNdaxRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "ndax"
     SYMBOL = "BTC/USDT"
-    SYMBOL_2 = "ETH/BTC"
-    SYMBOL_3 = "XRP/BTC"
+    SYMBOL_2 = "ETH/CAD"
+    SYMBOL_3 = "XRP/CAD"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
             TimeFrames.FIVE_MINUTES.value,
+            TimeFrames.FIFTEEN_MINUTES.value,
+            TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
-            TimeFrames.ONE_DAY.value
+            TimeFrames.TWO_HOURS.value,
+            TimeFrames.FOUR_HOURS.value,
+            TimeFrames.SIX_HOURS.value,
+            TimeFrames.TWELVE_HOURS.value,
+            TimeFrames.ONE_DAY.value,
+            TimeFrames.ONE_WEEK.value,
+            TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
@@ -53,28 +61,30 @@
                 Ecmsc.PRECISION_AMOUNT.value] <= 1  # to be fixed in this exchange tentacle
             assert 0 < market_status[Ecmsc.PRECISION.value][
                 Ecmsc.PRECISION_PRICE.value] <= 1  # to be fixed in this exchange tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
-            self.check_market_status_limits(market_status, has_price_limits=False)
+            self.check_market_status_limits(market_status,
+                                            low_price_max=1e-03,
+                                            low_price_min=1e-05,
+                                            normal_cost_min=1e-07,
+                                            low_cost_max=1e-02,
+                                            low_cost_min=1e-04,
+                                            expect_invalid_price_limit_values=False,
+                                            enable_price_and_cost_comparison=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) >= 744
-        # check candles order (oldest first)
-        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
-        # check last candle is the current candle
-        assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
+        assert len(symbol_prices) == 0  # limit has to be set in tentacle or on candle is returns by default
 
-        # candle limit is not supported, replaced by (await self.get_symbol_prices())[-limit:] in bittrex tentacle
         # try with candles limit (used in candled updater)
-        symbol_prices = (await self.get_symbol_prices())[-200:]
+        symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_historical_symbol_prices(self):
@@ -86,52 +96,50 @@
             else:
                 assert len(symbol_prices) > 5
             # check candles order (oldest first)
             self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
             # check that fetched candles are historical candles
             max_candle_time = self.get_time_after_time_frames(self.CANDLE_SINCE_SEC, len(symbol_prices))
             assert max_candle_time <= self.get_time()
-            for candle in symbol_prices:
-                assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
+            if limit is None:
+                with pytest.raises(AssertionError):  # not supported
+                    for candle in symbol_prices:
+                        assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
+            else:
+                for candle in symbol_prices:
+                    assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
 
     async def test_get_kline_price(self):
-        # kline_price = await self.get_kline_price()
-        client = bittrex()
-        await client.fetch_markets()
-        kline_price = [(await client.fetch_ohlcv(TestBittrexRealExchangeTester.SYMBOL, TimeFrames.ONE_HOUR.value))[-1]]
-
+        kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
-        await client.close()
 
     async def test_get_order_book(self):
-        # fetchOrderBook() limit argument must be None, 1, 25 or 500, default is 25
-        order_book = await self.get_order_book(limit=25)
-        assert len(order_book[Ecobic.ASKS.value]) == 25
+        order_book = await self.get_order_book()
+        assert len(order_book[Ecobic.ASKS.value]) == 5
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 25
+        assert len(order_book[Ecobic.BIDS.value]) == 5
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
     async def test_get_all_currencies_price_ticker(self):
-        tickers = await self.get_all_currencies_price_ticker()
-        for symbol, ticker in tickers.items():
-            self._check_ticker(ticker, symbol)
+        with pytest.raises(errors.NotSupported):
+            await self.get_all_currencies_price_ticker()
 
     @staticmethod
     def _check_ticker(ticker, symbol, check_content=False):
         assert ticker[Ectc.SYMBOL.value] == symbol
         assert all(key in ticker for key in (
             Ectc.HIGH.value,
             Ectc.LOW.value,
@@ -141,21 +149,21 @@
             Ectc.ASK_VOLUME.value,
             Ectc.OPEN.value,
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
+            # todo fix in tentacle: replace 0.0 by None
             assert ticker[Ectc.HIGH.value] is None
             assert ticker[Ectc.LOW.value] is None
             assert ticker[Ectc.BID.value]
             assert ticker[Ectc.BID_VOLUME.value] is None
             assert ticker[Ectc.ASK.value]
             assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value] is None
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
-            assert ticker[Ectc.TIMESTAMP.value]
             assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
-            assert ticker[Ectc.BASE_VOLUME.value] is None
-            RealExchangeTester.check_ticker_typing(ticker, check_open=False, check_high=False,
-                                                   check_low=False, check_base_volume=False, check_timestamp=False)
+            assert ticker[Ectc.BASE_VOLUME.value] is not None
+            assert ticker[Ectc.TIMESTAMP.value]
+            RealExchangeTester.check_ticker_typing(ticker, check_high=False, check_low=False, check_open=False)
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bybit.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_bybit_futures.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bybit_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_coinbase.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_coinbase.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_coinex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_coinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_cryptocom.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_cryptocom.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,20 +61,21 @@
                 Ecmsc.PRECISION_PRICE.value] <= 1  # to be fixed in CryptoCom tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
             self.check_market_status_limits(market_status, expect_invalid_price_limit_values=False,
                                             enable_price_and_cost_comparison=False,
-                                            normal_cost_min=1e-10, low_cost_min=1e-9)
+                                            normal_cost_min=1e-10, low_cost_min=1e-9,
+                                            has_price_limits=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 300
+        assert len(symbol_prices) == 25
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
         symbol_prices = await self.get_symbol_prices(limit=200)
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_gateio.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_hitbtc.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_hitbtc.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_hollaex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_hollaex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_huobi.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_huobipro.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_kraken.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_kraken.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_kucoin.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_kucoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_kucoin_futures.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_kucoin_futures.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pytest
 
 import octobot_commons.constants as commons_constants
 from octobot_commons.enums import TimeFrames, PriceIndexes
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
+import octobot_trading.errors as errors
 from tests_additional.real_exchanges.real_futures_exchange_tester import RealFuturesExchangeTester
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
@@ -136,17 +137,18 @@
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
     async def test_get_all_currencies_price_ticker(self):
-        tickers = await self.get_all_currencies_price_ticker()
-        for symbol, ticker in tickers.items():
-            self._check_ticker(ticker, symbol)
+        with pytest.raises(errors.NotSupported):
+            tickers = await self.get_all_currencies_price_ticker()
+            for symbol, ticker in tickers.items():
+                self._check_ticker(ticker, symbol)
 
     async def test_get_funding_rate(self):
         funding_rate, ticker_funding_rate = await self.get_funding_rate()
         # patch NEXT_FUNDING_TIME in tentacle
         self._check_funding_rate(funding_rate, has_next_time=False)
         # no funding info in ticker
         self._check_funding_rate(ticker_funding_rate, has_rate=False, has_last_time=False,
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_ndax.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_bittrex.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,49 +10,41 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import pytest
+from ccxt.async_support import bittrex
 
 from octobot_commons.enums import TimeFrames, PriceIndexes
-import octobot_trading.errors as errors
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
 from tests_additional.real_exchanges.real_exchange_tester import RealExchangeTester
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestNdaxRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "ndax"
+class TestBittrexRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "bittrex"
     SYMBOL = "BTC/USDT"
-    SYMBOL_2 = "ETH/CAD"
-    SYMBOL_3 = "XRP/CAD"
+    SYMBOL_2 = "ETH/BTC"
+    SYMBOL_3 = "XRP/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
             TimeFrames.FIVE_MINUTES.value,
-            TimeFrames.FIFTEEN_MINUTES.value,
-            TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
-            TimeFrames.TWO_HOURS.value,
-            TimeFrames.FOUR_HOURS.value,
-            TimeFrames.SIX_HOURS.value,
-            TimeFrames.TWELVE_HOURS.value,
-            TimeFrames.ONE_DAY.value,
-            TimeFrames.ONE_WEEK.value,
-            TimeFrames.ONE_MONTH.value
+            TimeFrames.ONE_DAY.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
@@ -61,30 +53,28 @@
                 Ecmsc.PRECISION_AMOUNT.value] <= 1  # to be fixed in this exchange tentacle
             assert 0 < market_status[Ecmsc.PRECISION.value][
                 Ecmsc.PRECISION_PRICE.value] <= 1  # to be fixed in this exchange tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
-            self.check_market_status_limits(market_status,
-                                            low_price_max=1e-03,
-                                            low_price_min=1e-05,
-                                            normal_cost_min=1e-07,
-                                            low_cost_max=1e-02,
-                                            low_cost_min=1e-04,
-                                            expect_invalid_price_limit_values=False,
-                                            enable_price_and_cost_comparison=False)
+            self.check_market_status_limits(market_status, has_price_limits=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 0  # limit has to be set in tentacle or on candle is returns by default
+        assert len(symbol_prices) >= 744
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # candle limit is not supported, replaced by (await self.get_symbol_prices())[-limit:] in bittrex tentacle
         # try with candles limit (used in candled updater)
-        symbol_prices = await self.get_symbol_prices(limit=200)
+        symbol_prices = (await self.get_symbol_prices())[-200:]
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_historical_symbol_prices(self):
@@ -96,50 +86,57 @@
             else:
                 assert len(symbol_prices) > 5
             # check candles order (oldest first)
             self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
             # check that fetched candles are historical candles
             max_candle_time = self.get_time_after_time_frames(self.CANDLE_SINCE_SEC, len(symbol_prices))
             assert max_candle_time <= self.get_time()
-            if limit is None:
-                with pytest.raises(AssertionError):  # not supported
-                    for candle in symbol_prices:
-                        assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
-            else:
-                for candle in symbol_prices:
-                    assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
+            for candle in symbol_prices:
+                assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value]
+                if limit is None:
+                    assert candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
+                else:
+                    with pytest.raises(AssertionError):  # not supported: candles are after the max time requested
+                        assert candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
 
     async def test_get_kline_price(self):
-        kline_price = await self.get_kline_price()
+        # kline_price = await self.get_kline_price()
+        client = bittrex()
+        await client.fetch_markets()
+        kline_price = [(await client.fetch_ohlcv(TestBittrexRealExchangeTester.SYMBOL, TimeFrames.ONE_HOUR.value))[-1]]
+
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
+        await client.close()
 
     async def test_get_order_book(self):
-        order_book = await self.get_order_book()
-        assert len(order_book[Ecobic.ASKS.value]) == 5
+        # fetchOrderBook() limit argument must be None, 1, 25 or 500, default is 25
+        order_book = await self.get_order_book(limit=25)
+        assert len(order_book[Ecobic.ASKS.value]) == 25
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 5
+        assert len(order_book[Ecobic.BIDS.value]) == 25
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
     async def test_get_all_currencies_price_ticker(self):
-        with pytest.raises(errors.NotSupported):
-            await self.get_all_currencies_price_ticker()
+        tickers = await self.get_all_currencies_price_ticker()
+        for symbol, ticker in tickers.items():
+            self._check_ticker(ticker, symbol)
 
     @staticmethod
     def _check_ticker(ticker, symbol, check_content=False):
         assert ticker[Ectc.SYMBOL.value] == symbol
         assert all(key in ticker for key in (
             Ectc.HIGH.value,
             Ectc.LOW.value,
@@ -149,21 +146,21 @@
             Ectc.ASK_VOLUME.value,
             Ectc.OPEN.value,
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
-            # todo fix in tentacle: replace 0.0 by None
-            assert ticker[Ectc.HIGH.value]
-            assert ticker[Ectc.LOW.value]
+            assert ticker[Ectc.HIGH.value] is None
+            assert ticker[Ectc.LOW.value] is None
             assert ticker[Ectc.BID.value]
             assert ticker[Ectc.BID_VOLUME.value] is None
             assert ticker[Ectc.ASK.value]
             assert ticker[Ectc.ASK_VOLUME.value] is None
-            assert ticker[Ectc.OPEN.value]
+            assert ticker[Ectc.OPEN.value] is None
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
-            assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
-            assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
-            RealExchangeTester.check_ticker_typing(ticker)
+            assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
+            assert ticker[Ectc.BASE_VOLUME.value] is None
+            RealExchangeTester.check_ticker_typing(ticker, check_open=False, check_high=False,
+                                                   check_low=False, check_base_volume=False, check_timestamp=False)
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_okcoin.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_okcoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_okx.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_okx_futures.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_okx_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_phemex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_phemex.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,42 +74,53 @@
                                             low_cost_min=0.01,
                                             low_cost_max=1,
                                             expect_invalid_price_limit_values=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 100
+        assert len(symbol_prices) == 1000
         symbol_prices = await self.get_symbol_prices(limit=100)
         assert len(symbol_prices) == 100
         symbol_prices = await self.get_symbol_prices(limit=500)
         assert len(symbol_prices) == 500
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
         symbol_prices = await self.get_symbol_prices(limit=200)
-        assert len(symbol_prices) == 100    # see possibleLimitValues
+        assert len(symbol_prices) == 200    # see possibleLimitValues
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_historical_symbol_prices(self):
+        # try with since and limit (used in data collector)
         for limit in (100, None):
-            assert len(await self.get_symbol_prices(since=self.CANDLE_SINCE_SEC, limit=limit)) == 5    # not supported
+            symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=limit)
+            if limit:
+                assert len(symbol_prices) == limit
+            else:
+                assert len(symbol_prices) > 5
+            # check candles order (oldest first)
+            self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+            # check that fetched candles are historical candles
+            max_candle_time = self.get_time_after_time_frames(self.CANDLE_SINCE_SEC, len(symbol_prices))
+            assert max_candle_time <= self.get_time()
+            for candle in symbol_prices:
+                assert self.CANDLE_SINCE_SEC <= candle[PriceIndexes.IND_PRICE_TIME.value]
+                with pytest.raises(AssertionError):  # not supported: candles are after the max time requested
+                    assert candle[PriceIndexes.IND_PRICE_TIME.value] <= max_candle_time
 
     async def test_get_kline_price(self):
-        # todo add param in tentacle
         kline_price = await self.get_kline_price()
-        # get_kline_price is returning the last 100 candles on phemex
-        assert len(kline_price) == 100
-        kline_price = [kline_price[-1]]
+        assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
         order_book = await self.get_order_book()
@@ -125,16 +136,17 @@
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
     async def test_get_all_currencies_price_ticker(self):
-        with pytest.raises(errors.NotSupported):
-            await self.get_all_currencies_price_ticker()
+        tickers = await self.get_all_currencies_price_ticker()
+        for symbol, ticker in tickers.items():
+            self._check_ticker(ticker, symbol)
 
     @staticmethod
     def _check_ticker(ticker, symbol, check_content=False):
         assert ticker[Ectc.SYMBOL.value] == symbol
         assert all(key in ticker for key in (
             Ectc.HIGH.value,
             Ectc.LOW.value,
```

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_poloniex.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_poloniex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_upbit.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_upbit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.4/tests_additional/real_exchanges/test_wavesexchange.py` & `OctoBot-Trading-2.4.5/tests_additional/real_exchanges/test_wavesexchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
 class TestWavesExchangeRealExchangeTester(RealExchangeTester):
     EXCHANGE_NAME = "wavesexchange"
-    SYMBOL = "ETH/USDT"
-    SYMBOL_2 = "CRO/XTN"
-    SYMBOL_3 = "SHIB/XTN"
+    SYMBOL = "ETH/USDT-ERC20"
+    SYMBOL_2 = "CRO-WXG/XTN"
+    SYMBOL_3 = "SHIB-WXG/XTN"
     ALLOWED_TIMEFRAMES_WITHOUT_CANDLE = RealExchangeTester.ALLOWED_TIMEFRAMES_WITHOUT_CANDLE + 1    # account for dumped candle
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
             TimeFrames.FIVE_MINUTES.value,
```

