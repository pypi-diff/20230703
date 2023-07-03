# Comparing `tmp/coinlib-2.2.6.tar.gz` & `tmp/coinlib-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coinlib-2.2.6.tar", last modified: Thu Jun  8 10:25:35 2023, max compression
+gzip compressed data, was "dist/coinlib-2.2.7.tar", last modified: Mon Jul  3 07:38:35 2023, max compression
```

## Comparing `coinlib-2.2.6.tar` & `coinlib-2.2.7.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.676814 coinlib-2.2.6/
--rw-r--r--   0 root         (0) root         (0)      642 2023-06-08 10:25:35.676814 coinlib-2.2.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.655814 coinlib-2.2.6/coinlib/
--rw-rw-rw-   0 root         (0) root         (0)    28406 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/BasicJob.py
--rw-rw-rw-   0 root         (0) root         (0)     7820 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/BasicJobSessionStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/ChartsFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9523 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/ChartsIndicatorJob.py
--rw-rw-rw-   0 root         (0) root         (0)     9404 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/ChartsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/CoinlibCrypto.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/CoinlibDataInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/CoinlibWorkspace.py
--rw-rw-rw-   0 root         (0) root         (0)    26721 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/DataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/InfluxDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/PluginLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     6388 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/PluginsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5960 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/Registrar.py
--rw-rw-rw-   0 root         (0) root         (0)    17647 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/Simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    13006 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/WorkerJobProcess.py
--rw-rw-rw-   0 root         (0) root         (0)     5812 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.659814 coinlib-2.2.6/coinlib/broker/
--rw-rw-rw-   0 root         (0) root         (0)     7229 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/Broker.py
--rw-rw-rw-   0 root         (0) root         (0)     4411 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/BrokerDTO.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBrokerFuture.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBrokerMargin.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBrokerSpot.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibSessionManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.660814 coinlib-2.2.6/coinlib/brokerWorker/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     7841 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerSession.py
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerSessionWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/TestProtocolResult.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/coinlibFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.661814 coinlib-2.2.6/coinlib/data/
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/data/CollectionInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    11600 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/data/DataTable.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    78694 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/dataWorker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   164353 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/dataWorker_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.662814 coinlib-2.2.6/coinlib/drawable/
--rw-rw-rw-   0 root         (0) root         (0)     3528 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/CoinlibDrawable.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/DrawableComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/WindowGrid.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.662814 coinlib-2.2.6/coinlib/event/
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/event/EventConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/event/EventInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.664814 coinlib-2.2.6/coinlib/feature/
--rw-rw-rw-   0 root         (0) root         (0)    17646 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeature.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeatureFetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeatureLake.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeatureProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/FeatureDTO.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/FeatureFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9545 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/FeatureWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     6088 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/Features.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/helper.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/index.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.669814 coinlib-2.2.6/coinlib/logics/
--rw-rw-rw-   0 root         (0) root         (0)    13495 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/Logic.py
--rw-rw-rw-   0 root         (0) root         (0)     8794 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicBasicWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicDTo.py
--rw-rw-rw-   0 root         (0) root         (0)     7564 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicJob.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineJob.py
--rw-rw-rw-   0 root         (0) root         (0)    10121 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerData.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerScreener.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerTrader.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineDataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineJob.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineScreenerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineTraderWorker.py
--rw-rw-rw-   0 root         (0) root         (0)    14919 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8512 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicRegistrationInstance.py
--rw-rw-rw-   0 root         (0) root         (0)    16758 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicTestBrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.669814 coinlib-2.2.6/coinlib/logics/broker/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/broker/LogicBrokerInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.670814 coinlib-2.2.6/coinlib/logics/manager/
--rw-rw-rw-   0 root         (0) root         (0)     7098 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/LogicJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/LogicManager.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/PortfolioModel.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.671814 coinlib-2.2.6/coinlib/logics/offlineManager/
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
--rw-rw-rw-   0 root         (0) root         (0)    11492 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.671814 coinlib-2.2.6/coinlib/logics/onlineManager/
--rw-rw-rw-   0 root         (0) root         (0)     6706 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/onlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.672814 coinlib-2.2.6/coinlib/notification/
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/Notification.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/NotificationFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/NotificationWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.674814 coinlib-2.2.6/coinlib/statistics/
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticMethodJob.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticRuleJob.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/Statistics.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsMethodFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsMethodWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsRuleFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     6204 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsRuleWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.675814 coinlib-2.2.6/coinlib/symbols/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/SymbolFactory.py
--rw-rw-rw-   0 root         (0) root         (0)    14991 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/SymbolWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/Symbols.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.657814 coinlib-2.2.6/coinlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3789 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 10:25:35.676814 coinlib-2.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-08 10:25:22.000000 coinlib-2.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.676814 coinlib-2.2.6/test/
--rw-rw-rw-   0 root         (0) root         (0)     4048 2023-06-08 10:25:22.000000 coinlib-2.2.6/test/testchartworker.py
--rw-rw-rw-   0 root         (0) root         (0)    10860 2023-06-08 10:25:22.000000 coinlib-2.2.6/test/testcross.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-06-08 10:25:22.000000 coinlib-2.2.6/test/testplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.403538 coinlib-2.2.7/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-03 07:38:35.403538 coinlib-2.2.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.383539 coinlib-2.2.7/coinlib/
+-rw-rw-rw-   0 root         (0) root         (0)    29350 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/BasicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     7828 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/BasicJobSessionStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/ChartsFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)    13707 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/ChartsIndicatorJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     9404 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/ChartsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/CoinlibCrypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/CoinlibDataInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/CoinlibWorkspace.py
+-rw-rw-rw-   0 root         (0) root         (0)    26721 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/DataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/InfluxDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/PluginLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/PluginsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5960 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/Registrar.py
+-rw-rw-rw-   0 root         (0) root         (0)    17647 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/Simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    13066 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/WorkerJobProcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.386538 coinlib-2.2.7/coinlib/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     7229 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/Broker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/BrokerDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/CoinlibBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/CoinlibBrokerFuture.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/CoinlibBrokerMargin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/CoinlibBrokerSpot.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/CoinlibSessionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.387539 coinlib-2.2.7/coinlib/brokerWorker/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/brokerWorker/BrokerFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7841 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/brokerWorker/BrokerSession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/brokerWorker/BrokerSessionWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/brokerWorker/BrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/brokerWorker/TestProtocolResult.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/brokerWorker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/coinlibFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.388538 coinlib-2.2.7/coinlib/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/data/CollectionInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)    11693 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/data/DataTable.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    78694 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/dataWorker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   164353 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/dataWorker_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.389538 coinlib-2.2.7/coinlib/drawable/
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/drawable/CoinlibDrawable.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/drawable/DrawableComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/drawable/WindowGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/drawable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.389538 coinlib-2.2.7/coinlib/event/
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/event/EventConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/event/EventInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.391538 coinlib-2.2.7/coinlib/feature/
+-rw-rw-rw-   0 root         (0) root         (0)    17646 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/CoinlibFeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/CoinlibFeatureFetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/CoinlibFeatureLake.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/CoinlibFeatureProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/FeatureDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/FeatureFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9545 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/FeatureWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6088 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/Features.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/feature/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15693 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.396538 coinlib-2.2.7/coinlib/logics/
+-rw-rw-rw-   0 root         (0) root         (0)    13495 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/Logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicBasicWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicDTo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7564 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOfflineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    10120 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOfflineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOfflineWorkerData.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOfflineWorkerScreener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOfflineWorkerTrader.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOnlineDataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOnlineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOnlineScreenerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOnlineTraderWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)    15009 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOnlineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8512 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicRegistrationInstance.py
+-rw-rw-rw-   0 root         (0) root         (0)    16758 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/LogicTestBrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.396538 coinlib-2.2.7/coinlib/logics/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/broker/LogicBrokerInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.397538 coinlib-2.2.7/coinlib/logics/manager/
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/manager/LogicJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/manager/LogicManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/manager/PortfolioModel.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.398538 coinlib-2.2.7/coinlib/logics/offlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)    20274 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11492 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/offlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.399538 coinlib-2.2.7/coinlib/logics/onlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)     6706 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/logics/onlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.399538 coinlib-2.2.7/coinlib/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/notification/Notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/notification/NotificationFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/notification/NotificationWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.401538 coinlib-2.2.7/coinlib/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/StatisticMethodJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/StatisticRuleJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/Statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/StatisticsMethodFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/StatisticsMethodWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/StatisticsRuleFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/StatisticsRuleWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/statistics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.402538 coinlib-2.2.7/coinlib/symbols/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/symbols/SymbolFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14991 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/symbols/SymbolWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/symbols/Symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 07:38:23.000000 coinlib-2.2.7/coinlib/symbols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.384539 coinlib-2.2.7/coinlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-03 07:38:35.000000 coinlib-2.2.7/coinlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-07-03 07:38:35.000000 coinlib-2.2.7/coinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 07:38:35.000000 coinlib-2.2.7/coinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-03 07:38:35.000000 coinlib-2.2.7/coinlib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-03 07:38:35.000000 coinlib-2.2.7/coinlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 07:38:35.000000 coinlib-2.2.7/coinlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 07:38:35.403538 coinlib-2.2.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-07-03 07:38:23.000000 coinlib-2.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:38:35.403538 coinlib-2.2.7/test/
+-rw-rw-rw-   0 root         (0) root         (0)     4048 2023-07-03 07:38:23.000000 coinlib-2.2.7/test/testchartworker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10860 2023-07-03 07:38:23.000000 coinlib-2.2.7/test/testcross.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-07-03 07:38:23.000000 coinlib-2.2.7/test/testplot.py
```

### Comparing `coinlib-2.2.6/PKG-INFO` & `coinlib-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.6
+Version: 2.2.7
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.6/coinlib/BasicJob.py` & `coinlib-2.2.7/coinlib/BasicJob.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,31 @@
 
         return input
 
 
     def getNow(self, name):
         return self.current(name)
 
+
+    def is_new_day(self, i=-1, offset=0):
+        if i == 0:
+            return False
+        dt1 = self.table.index[i] + datetime.timedelta(hours=offset)
+        dt2 = self.table.index[i-1] + datetime.timedelta(hours=offset)
+        # check if there is a new day between the two dates
+        return (dt1.day != dt2.day)
+
+    def is_new_week(self, i=-1, offset=0):
+        if i == 0:
+            return False
+        dt1 = self.table.index[i] + datetime.timedelta(hours=offset)
+        dt2 = self.table.index[i-1] + datetime.timedelta(hours=offset)
+        # check if there is a new week between the two dates
+        return (dt1.week != dt2.week)
+
     def getCurrent(self, name):
         return self.current(name)
 
     def logger(self):
         return self.registrar.logger
 
     def functions(self):
@@ -262,19 +279,21 @@
             if mode == CrossMode.both or mode == CrossMode.down:
                 if currentline[-1] < y:
                     return True
 
         return False
 
     def isDateGreater(self, date, time=None):
+        formatter = "%Y-%m-%d"
         if time is not None:
             date = date +" "+ time
+            formatter = formatter + " %H:%M:%S"
 
         curdate = self.date(index=-1)
-        testdate = parser.parse(date)
+        testdate = datetime.datetime.fromisoformat(date)
         if testdate is None:
             raise(Exception("The date u gave can not be parsed to a date."))
 
         if curdate > testdate:
             return True
         return False
 
@@ -688,16 +707,19 @@
             self.logger().error(e)
 
         if data is not None:
             return data
 
         return data
 
-    def getNow_date(self):
-        dt = self.table.index[-1]
+    def getNow_date(self, index=-1):
+        # when index is not integer
+        if not isinstance(index, int):
+            return index
+        dt = self.table.index[index]
         return dt
 
     def current(self, name):
         return self.get(name, index=-1)
 
     def statistic(self, name="r_master"):
 
@@ -733,26 +755,27 @@
             if self.isNaN(data):
                 return None
             return data
 
         return None
 
     def date(self, index=-1):
-        date = pd.to_datetime(self.table.index[index]).to_pydatetime()
+        #date = pd.to_datetime(self.table.index[index]).to_pydatetime()
+        date = self.table.index[index]
         return date
 
     def closeDate(self):
-        if len(self.table.index) > 0:
-            date = pd.to_datetime(self.table.index[-1]).to_pydatetime()
-            return date
-        return None
+        #if len(self.table.index) > 0:
+        #    date = pd.to_datetime(self.table.index[-1]).to_pydatetime()
+        date = self.table.index[-1]
+        return date
 
     def time(self):
         if len(self.table.index) > 0:
-            date = pd.to_datetime(self.table.index[-1])
+            date = pd.to_datetime(self.table.index[-1], infer_datetime_format=True)
             return date
         return None
 
 
     def varInfo(self, name, logicId=None):
         d = self.getLastData(logicId+".var."+name)
         return d
```

### Comparing `coinlib-2.2.6/coinlib/BasicJobSessionStorage.py` & `coinlib-2.2.7/coinlib/BasicJobSessionStorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import json
 import time
 
 import numpy as np
 
 from coinlib import Registrar
+from coinlib.helper import faster_strftime
 
 
 class LastSignalValue:
     found: bool
     value: any
     distanceTicks: int
     distanceSeconds: int
@@ -48,18 +49,18 @@
                 for key in self._storage[k_index]:
                     value = self._storage[k_index][key]
                     try:
                         if value is not None and not np.isnan(value):
                             last = LastSignalValue()
                             last.value = self._storage[k_index][key]
                             last.distanceTicks = ticks
-                            lastTime = datetime.datetime.strptime(k_index, "%Y-%m-%d-%H:%M:%S")
+                            lastTime = datetime.datetime.fromisoformat(k_index, "%Y-%m-%d %H:%M:%S")
                             last.time = lastTime
                             last.ticks = ticks
-                            currentTime = datetime.datetime.strptime(self._lastIndex, "%Y-%m-%d-%H:%M:%S")
+                            currentTime = datetime.datetime.fromisoformat(self._lastIndex, "%Y-%m-%d %H:%M:%S")
                             last.distanceSeconds = (currentTime - lastTime).total_seconds()
                             last.found = True
                             if key not in self._lastStorage:
                                 self._lastStorage[key] = last
                                 self.registrar.logger.info("Last Storage set: "+key+": "+json.dumps(last))
 
                     except Exception as e:
@@ -73,15 +74,15 @@
         return list(self._lastStorage.keys())
 
     def saveInfo(self, group, key, value):
         self.setData(group+"."+key, value)
 
     def setCurrentIndex(self, index, moveLastValues=False):
         if index is not None:
-            index = index.strftime("%Y-%m-%d-%H:%M:%S")
+            index = faster_strftime(index)
             if self._currentIndex == index:
                 return
             """ if moveLastValues:
                 self._changed = False
                 if self._lastIndex in self._storage:
                     self._storage[index] = {}
                     for key in self._storage[self._lastIndex]:
@@ -140,16 +141,16 @@
 
     def getLastData(self, key, maxSecondsDistance=None) -> LastSignalValue:
         last = LastSignalValue()
         last.found = False
         last.value = None
         if key in self._lastStorage:
             nv = self._lastStorage[key]
-            lastTime = datetime.datetime.strptime(nv.time, "%Y-%m-%d-%H:%M:%S") if isinstance(nv.time, str) else nv.time
-            currentTime = datetime.datetime.strptime(self._currentIndex, "%Y-%m-%d-%H:%M:%S")
+            lastTime = datetime.datetime.fromisoformat(nv.time) if isinstance(nv.time, str) else nv.time
+            currentTime = datetime.datetime.fromisoformat(self._currentIndex)
             ticks = self._currentTicks - nv.ticks if self._currentTicks > 0 else nv.ticks
             distance = (currentTime - lastTime).total_seconds()
             if maxSecondsDistance is not None:
                 if distance > maxSecondsDistance:
                     return last
 
             last.time = nv.time
```

### Comparing `coinlib-2.2.6/coinlib/ChartsIndicatorJob.py` & `coinlib-2.2.7/coinlib/ChartsIndicatorJob.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,34 @@
+import copy
+import datetime
+
+import datetime
+import pytz
 import pandas as pd
 import numpy as np
+
+from coinlib.helper import taBox
 from coinlib.BasicJob import BasicJob
 import time
 
 from coinlib.data.DataTable import DataTable
 import json
 
 def isFullOHLC(row):
     return (row.close != 0 and row.close != None and row.open != 0 and row.open != None and
             row.high != 0 and row.high != None and row.low != None and row.low != 0)
 
 
+def is_in_list(allboxes, box):
+    for b in allboxes:
+        if b.top == box.top and b.bottom == box.bottom and b.left == box.left and b.right == box.right:
+            return True
+    return False
+
+
 class ChartsIndicatorJob(BasicJob):
     def __init__(self, name, group, inputs, df, indicator, worker):
         super(ChartsIndicatorJob, self).__init__(df if type(df) == DataTable else DataTable(df), inputs)
         self.name = name
         self.group = group
         self.send = False
         self.chunked = False
@@ -95,14 +109,61 @@
         except:
             c = color
         c = colorsys.rgb_to_hls(*mc.to_rgb(c))
         rgbs = colorsys.hls_to_rgb(c[0], 1 - higher_lower * (1 - c[1]), c[2])
 
         rgbhex = self.rgb2hex(int(rgbs[0] * 255), int(rgbs[1] * 255), int(rgbs[2] * 255))
         return rgbhex
+
+    def convertBoxes(self, boxesList: [[{"top": float, "bottom": float}]]):
+        eboxes = self.emptyList(len(boxesList))
+
+        for i in range(len(boxesList)):
+            boxes = boxesList[i]
+            if boxes is None:
+                continue
+            eboxes[i] = json.dumps(boxes)
+        return eboxes
+
+    def emptySeries(self, l=None, emptyData=np.nan):
+        if l is None:
+            l = self.table.length()
+        d = np.empty(l)
+        d[:] = emptyData
+        return d
+
+    def emptyList(self, l=None, emptyData=None):
+        if l is None:
+            l = self.table.length()
+        d = []
+        for i in range(l):
+            d.append(emptyData)
+        return d
+
+    def fillBoxSequentialInList(self, data: list, box: taBox, paddingleft=0):
+        for i in range(box.left+paddingleft, box.right+paddingleft):
+            if box.get_top() <= 0 or box.get_bottom() <= 0:
+                continue
+
+            if data[i] == np.nan or data[i] is None:
+                data[i] = []
+
+            # when the box does not exist in the list
+            # by the same top and bottom values
+            # then we add it to the list
+            if len(data[i]) > 0:
+                ignore = False
+                for b in data[i]:
+                    if b["top"] == box.top and b["bottom"] == box.bottom:
+                        ignore = True
+                if not ignore:
+                    data[i].append(box.get_HLBox())
+            else:
+                data[i].append(box.get_HLBox())
+        return data
     
     def series(self, chartType, name, data, color=None,
                opacity=None,
                chartTypeIcon=None,
                size=None, tooltip=True, chart=None,
                fill=None, fill_from=None,
                fill_to=None, connectGaps=False):
@@ -124,16 +185,14 @@
         @opacity: This is the opacity of the chart data
         @chartTypeIcon: Only available for "marker" - you ca select the icon for the marker
         @size: The size of the marker
         @tooltip: The tooltip if needed - for example this is a text when mouse is over marker
         """
         if color is None:
             color = "#ccffcc"
-        import datetime
-        import pytz
 
 
         utc=pytz.UTC
         latestDate = datetime.datetime(1971, 3, 19, 13, 0, 9, 351812)
         latestDate = utc.localize(latestDate)
         additional = {}
 
@@ -151,14 +210,55 @@
             elif chartType == "marker" or chartType == "cross":
                 # it is a numpy array
                 if isinstance(data, (pd.core.series.Series)):
                     self.table.setColumn(":marker", data.values, type=str)
                 else:
                     self.table.setColumn(":marker", data, type=str)
                 column_names = [":marker"]
+            elif chartType == "boxes":
+                listdata = self.emptyList()
+                allboxes = []
+                padding_from_left = len(listdata) - len(data)
+                # we want to iterate over all data and select the boxes
+                # than we check and modify create small boxes for each index
+                # when its not a box we just add None
+                for i in range(len(data)):
+                    if data[i] is not None:
+                        if isinstance(data[i], list) or isinstance(data[i], np.ndarray):
+                            for box in data[i]:
+                                listdata = self.fillBoxSequentialInList(listdata, box, padding_from_left)
+                                if not is_in_list(allboxes, box):
+                                    allboxes.append(box)
+                        else:
+                            listdata = self.fillBoxSequentialInList(listdata, data[i], padding_from_left)
+                listdata = self.convertBoxes(listdata)
+                self.table.setColumn(":boxes", listdata, type=str)
+                drawableList = self.emptyList()
+                for b in allboxes:
+                    if drawableList[b.left+padding_from_left] is None:
+                        drawableList[b.left+padding_from_left] = []
+                    drawableList[b.left+padding_from_left].append(b)
+
+                drawableListJsoned = self.emptyList()
+                for i in range(len(drawableList)):
+                    dw = drawableList[i]
+                    if dw is not None:
+                        nlist = []
+                        for b in dw:
+                            if b.top == 0 or b.bottom == 0:
+                                continue
+                            # lets deepcopy the box
+                            bc = copy.deepcopy(b)
+                            bc.left = datetime.datetime.strftime(self.getNow_date(b.left+padding_from_left), "%Y-%m-%dT%H:%M:%S.%fZ")
+                            bc.right = datetime.datetime.strftime(self.getNow_date(b.right+padding_from_left), "%Y-%m-%dT%H:%M:%S.%fZ")
+                            nlist.append(bc)
+                        drawableListJsoned[i] = json.dumps(nlist, default=lambda o: o.__dict__)
+
+                self.table.setColumn(":boxes_drawables", drawableListJsoned, type=str)
+                column_names = [":boxes", ":boxes_drawables"]
 
             elif chartType == "trendline" or chartType == "rayline":
                 # it is a numpy array
                 if isinstance(data, (pd.core.series.Series)):
                     self.table.setColumn(":marker", data.values, type=str)
                 else:
                     self.table.setColumn(":marker", data, type=str)
```

### Comparing `coinlib-2.2.6/coinlib/ChartsWorker.py` & `coinlib-2.2.7/coinlib/ChartsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/CoinlibCrypto.py` & `coinlib-2.2.7/coinlib/CoinlibCrypto.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/CoinlibDataInterface.py` & `coinlib-2.2.7/coinlib/CoinlibDataInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/CoinlibWorkspace.py` & `coinlib-2.2.7/coinlib/CoinlibWorkspace.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/DataWorker.py` & `coinlib-2.2.7/coinlib/DataWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/Functions.py` & `coinlib-2.2.7/coinlib/Functions.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/InfluxDatabase.py` & `coinlib-2.2.7/coinlib/InfluxDatabase.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/PluginLoader.py` & `coinlib-2.2.7/coinlib/PluginLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/PluginsWorker.py` & `coinlib-2.2.7/coinlib/PluginsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/Registrar.py` & `coinlib-2.2.7/coinlib/Registrar.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/Simulator.py` & `coinlib-2.2.7/coinlib/Simulator.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/WorkerJobProcess.py` & `coinlib-2.2.7/coinlib/WorkerJobProcess.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import queue
 import grpc
 import simplejson as json
 import traceback
 import zlib
 import binascii
 import base64
+
+from coinlib import ChartsIndicatorJob
 from coinlib.Registrar import Registrar
 from coinlib.InfluxDatabase import InfluxDatabase
 from chipmunkdb.ChipmunkDb import ChipmunkDb
 
 
 class Indicator:
     feature: str
@@ -202,15 +204,15 @@
     
     def getDf(self):
         return self.dataFrame
     
     def getChannel(self):
         return self.workerChannel
 
-    def callIndicator(self, targetIndicatorFunction, raw_inputs, chart):
+    def callIndicator(self, targetIndicatorFunction, raw_inputs, chart: ChartsIndicatorJob):
         process = None
 
         start = time.time()
         if (inspect.iscoroutinefunction(targetIndicatorFunction["process"])):
             async def runandwait():
                 try:
                     task = asyncio.ensure_future(targetIndicatorFunction["process"](raw_inputs, chart))
```

### Comparing `coinlib-2.2.6/coinlib/__init__.py` & `coinlib-2.2.7/coinlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from coinlib.CoinlibWorkspace import CoinlibWorkspace
 from coinlib.statistics.Statistics import Statistics
 from coinlib.Simulator import Simulator
 from coinlib.ChartsIndicatorJob import ChartsIndicatorJob
 from coinlib.broker.Broker import Broker
 from coinlib.notification.Notification import Notification
 from coinlib.symbols.Symbols import Symbols
-from coinlib.helper import trendline, to_trendline
+from coinlib.helper import trendline, to_trendline, taBox
 
 registrar = Registrar()
 
 if registrar.features is None:
     registrar.features = Features.Features()
     registrar.logic = Logic()
     registrar.functions = Functions()
@@ -146,9 +146,10 @@
         try:
             loop.run_forever()
         finally:
             loop.close()
 
 to_trendline = to_trendline
 trendline = trendline
+taBox = taBox
 
 set_loglevel("INFO")
```

### Comparing `coinlib-2.2.6/coinlib/broker/Broker.py` & `coinlib-2.2.7/coinlib/broker/Broker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/broker/BrokerDTO.py` & `coinlib-2.2.7/coinlib/broker/BrokerDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/broker/CoinlibBroker.py` & `coinlib-2.2.7/coinlib/broker/CoinlibBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/broker/CoinlibBrokerFuture.py` & `coinlib-2.2.7/coinlib/broker/CoinlibBrokerFuture.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/broker/CoinlibBrokerMargin.py` & `coinlib-2.2.7/coinlib/broker/CoinlibBrokerMargin.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/broker/CoinlibBrokerSpot.py` & `coinlib-2.2.7/coinlib/broker/CoinlibBrokerSpot.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/brokerWorker/BrokerSession.py` & `coinlib-2.2.7/coinlib/brokerWorker/BrokerSession.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/brokerWorker/BrokerSessionWorker.py` & `coinlib-2.2.7/coinlib/brokerWorker/BrokerSessionWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/brokerWorker/BrokerWorker.py` & `coinlib-2.2.7/coinlib/brokerWorker/BrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/brokerWorker/TestProtocolResult.py` & `coinlib-2.2.7/coinlib/brokerWorker/TestProtocolResult.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/coinlibFactory.py` & `coinlib-2.2.7/coinlib/coinlibFactory.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/config.py` & `coinlib-2.2.7/coinlib/config.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/data/CollectionInterface.py` & `coinlib-2.2.7/coinlib/data/CollectionInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/data/DataTable.py` & `coinlib-2.2.7/coinlib/data/DataTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,38 +121,40 @@
     def subTable(self, index=0, length=None, columns=None):
         sub = DataTable()
         sub._df = self._df
         sub.columns = self.columns
         sub.col = self.col
         if length is None:
             length = len(self.index)
-        sub.index = self.index[index:index+index]
-        #copy_np = self._np.copy()
+        #sub.index = self.index[index:index+index]
+        sub.index = self.index[index:index+length]
+
+        # copy_np = self._np.copy()
         try:
             if columns is not None:
                 sub.columns = columns
                 list = []
                 i = 0
                 cols = {}
                 for c in columns:
-                    list.append(self._np[self.col[c], index: index+length].copy())
+                    list.append(self._np[self.col[c], index: index + length].copy())
                     cols[c] = i
                     i = i + 1
                 sub._np = np.array(list)
                 sub.col = cols
             else:
-                sub._np = self._np[:, index: index+length].copy()
+                sub._np = self._np[:, index: index + length]
                 sub.col_chart = self.col_chart
                 for chart in self.col_chart:
-                    convertedIndex = int(self._index_reference_by_chart[chart][index+length])
+                    convertedIndex = int(self._index_reference_by_chart[chart][index + length])
                     sub._index_by_chart = self._index_reference_by_chart
-                    sub._np_by_chart[chart] = self._np_by_chart[chart][:, convertedIndex: convertedIndex+length].copy()
+                    sub._np_by_chart[chart] = self._np_by_chart[chart][:,
+                                              convertedIndex: convertedIndex + length]
         except Exception as e:
             print("Error while subtable ", e)
-
         return sub
 
     def setColumn(self, name, data, index=None, pad=True, type=float):
         ## padding needed maybe
 
         length = len(self.index)
         if length <= 0 and len(data) > 0:
```

### Comparing `coinlib-2.2.6/coinlib/dataWorker_pb2.py` & `coinlib-2.2.7/coinlib/dataWorker_pb2.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/dataWorker_pb2_grpc.py` & `coinlib-2.2.7/coinlib/dataWorker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/drawable/CoinlibDrawable.py` & `coinlib-2.2.7/coinlib/drawable/CoinlibDrawable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/drawable/WindowGrid.py` & `coinlib-2.2.7/coinlib/drawable/WindowGrid.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/event/EventConsumer.py` & `coinlib-2.2.7/coinlib/event/EventConsumer.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/event/EventInterface.py` & `coinlib-2.2.7/coinlib/event/EventInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/feature/CoinlibFeature.py` & `coinlib-2.2.7/coinlib/feature/CoinlibFeature.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/feature/CoinlibFeatureFetcher.py` & `coinlib-2.2.7/coinlib/feature/CoinlibFeatureFetcher.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/feature/CoinlibFeatureLake.py` & `coinlib-2.2.7/coinlib/feature/CoinlibFeatureLake.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/feature/FeatureDTO.py` & `coinlib-2.2.7/coinlib/feature/FeatureDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/feature/FeatureWorker.py` & `coinlib-2.2.7/coinlib/feature/FeatureWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/feature/Features.py` & `coinlib-2.2.7/coinlib/feature/Features.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/helper.py` & `coinlib-2.2.7/coinlib/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import calendar
+import copy
 import datetime
 import json
 import os
 import sys
 from dataclasses import dataclass
 
 import importlib
@@ -69,14 +70,21 @@
             return True
         else:
             return False
     except Exception:
         return False
 
 
+def faster_strftime(date, basicFormat="{:04d}-{:02d}-{:02d} {:02d}:{:02d}:{:02d}"):
+    return basicFormat.format(date.year, date.month, date.day, date.hour, date.minute, date.second)
+
+def faster_strftime_iso(date):
+    return "{:04d}-{:02d}-{:02d}T{:02d}:{:02d}:{:02d}.{:06d}Z".format(date.year, date.month, date.day, date.hour, date.minute, date.second, date.microsecond)
+
+
 is_in_ipynb = in_ipynb()
 
 if not 'workbookDir' in globals():
     workbookDir = os.getcwd()
 
 
 def get_current_plugin_code_type():
@@ -367,7 +375,89 @@
     }
 
 
 def trendline(x2: datetime, y2, x1: datetime, y1, name: str = ""):
     x2_d = datetime.datetime.strftime(x2, "%Y-%m-%dT%H:%M:%S.%fZ")
     x1_d = datetime.datetime.strftime(x1, "%Y-%m-%dT%H:%M:%S.%fZ")
     return "" + str(x1_d) + "," + str(float(y1)) + "," + str(x2_d) + "," + str(float(y2)) + "," + name
+
+
+
+# Create a class for pinescripts corresponding box object
+class taBox:
+    # Constructor
+    def __init__(self):
+        pass
+
+    # attributes from pinescript tradingview
+    left = 0
+    top = 0
+    right = 0
+    bottom = 0
+    border_color = None
+    border_width = None
+    border_style = None
+    extend = None
+    bgcolor = None
+    opacity = None
+
+
+    def copy(self):
+        return taBox.new(self.left, self.top, self.right, self.bottom, self.border_color,
+                         self.border_width, self.border_style, self.extend, self.bgcolor, self.opacity)
+
+    def get_HLBox(self):
+        return {
+            "top": self.top,
+            "bottom": self.bottom,
+            "bgcolor": self.bgcolor
+        }
+
+    # methods
+    def get_top(self):
+        return self.top
+
+    def get_bottom(self):
+        return self.bottom
+
+    def get_left(self):
+        return self.left
+
+    def get_right(self):
+        return self.right
+
+    def get_border_color(self):
+        return self.border_color
+
+
+
+    @staticmethod
+    def new(left, top, right, bottom, border_color=None,
+            border_width=None, border_style=None, extend=None,
+            bgcolor=None, opacity=None):
+        self = taBox()
+        self.left = left
+        self.top = top
+        self.right = right
+        self.bottom = bottom
+        self.border_color = border_color
+        self.border_width = border_width
+        self.border_style = border_style
+        self.extend = extend
+        self.opacity = opacity
+        self.bgcolor = bgcolor
+        return self
+
+    def set_left(self, left):
+        self.left = left
+
+    def set_top(self, top):
+        self.top = top
+
+    def set_right(self, right):
+        self.right = right
+
+    def set_bottom(self, bottom):
+        self.bottom = bottom
+
+    def set_extend(self, extend):
+        self.extend = extend
```

### Comparing `coinlib-2.2.6/coinlib/logger.py` & `coinlib-2.2.7/coinlib/logger.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/Logic.py` & `coinlib-2.2.7/coinlib/logics/Logic.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicBasicWorker.py` & `coinlib-2.2.7/coinlib/logics/LogicBasicWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicJob.py` & `coinlib-2.2.7/coinlib/logics/LogicJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicLoader.py` & `coinlib-2.2.7/coinlib/logics/LogicLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicOfflineJob.py` & `coinlib-2.2.7/coinlib/logics/LogicOfflineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicOfflineWorker.py` & `coinlib-2.2.7/coinlib/logics/LogicOfflineWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
 
                     threading.Thread(target=self.broadcastCurrentPercentage, args=[lastPercentage, fakeManager], daemon=True).start()
 
                 if startDate and index_date > startDate and index > minimumPeriod:
 
                     lastindex = index-minimumPeriod if index-minimumPeriod > 0 else 0
 
-
                     subTable = table.subTable(lastindex, minimumPeriod)
 
                     fakeManager.setTable(subTable)
                     fakeManager.setTimeRunningInSec(index_date.timestamp() - startDate.timestamp())
                     self.onNextSubTableReceived(fakeManager, subTable)
                     fakeManager.updateCurrentIndexToLast()
                     fakeManager.resetChanges()
```

### Comparing `coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerTrader.py` & `coinlib-2.2.7/coinlib/logics/LogicOfflineWorkerTrader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicOnlineJob.py` & `coinlib-2.2.7/coinlib/logics/LogicOnlineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicOnlineWorker.py` & `coinlib-2.2.7/coinlib/logics/LogicOnlineWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from coinlib.PluginLoader import PluginLoader
 from coinlib.PluginsWorker import PluginConfigInfo
 from coinlib.data.DataTable import DataTable
 import asyncio
 import simplejson as json
 from coinlib.WorkerJobProcess import WorkerJobProcess
 from coinlib.Registrar import Registrar
+from coinlib.helper import faster_strftime, faster_strftime_iso
 from coinlib.logics.LogicBasicWorker import LogicBasicWorker
 from coinlib.logics.LogicOfflineJob import LogicOfflineJob
 
 import queue
 import datetime
 
 from coinlib.logics.LogicOnlineJob import LogicOnlineJob
@@ -40,14 +41,17 @@
     message: string
 
 class NotificationInteractiveEvent:
     client_id: string
     callback_id: string
     data = ""
 
+
+
+
 class LogicOnlineWorker(LogicBasicWorker):
     brokerInterface: LogicBrokerInterface
     commandCallbacks: {}
 
     def initialize(self):
         super().initialize()
         self.registrar = Registrar()
@@ -206,15 +210,16 @@
 
         table = DataTable()
         table.from_df(self.dataFrame)
 
         infoStorageRaw = self.dataFrame.loc[:, self.dataFrame.columns.str.contains('result.', case=False)].rename(columns = lambda x: x.replace('result.logics.', '')).to_dict(orient="index")
         infoStorage = {}
         for key in infoStorageRaw:
-            infoStorage[key.strftime("%Y-%m-%d-%H:%M:%S")] = infoStorageRaw[key]
+            keyindex = faster_strftime_iso(key)
+            infoStorage[keyindex] = infoStorageRaw[key]
 
         if "portfolio" in params:
             self.portfolio = self.extractPortfolio(params)
         else:
             self.portfolio = None
 
         manager = LogicManager("", self.logicConfig, self.logicConfig.brokerAccount, self.portfolio, infoStorage)
```

### Comparing `coinlib-2.2.6/coinlib/logics/LogicRegistrationInstance.py` & `coinlib-2.2.7/coinlib/logics/LogicRegistrationInstance.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/LogicTestBrokerWorker.py` & `coinlib-2.2.7/coinlib/logics/LogicTestBrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/broker/LogicBrokerInterface.py` & `coinlib-2.2.7/coinlib/logics/broker/LogicBrokerInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/manager/LogicJobBroker.py` & `coinlib-2.2.7/coinlib/logics/manager/LogicJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/manager/LogicManager.py` & `coinlib-2.2.7/coinlib/logics/manager/LogicManager.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/manager/PortfolioModel.py` & `coinlib-2.2.7/coinlib/logics/manager/PortfolioModel.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py` & `coinlib-2.2.7/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
     def getNow_date(self):
         dt = self.table.getLastIndex()
         return dt
 
     def getNow(self):
         dt = self.table.getLastIndex()
-        date =  datetime.datetime.strftime(dt, "%Y-%m-%dT%H:%M:%S.%fZ")
+        date =   datetime.datetime.strftime(dt, "%Y-%m-%dT%H:%M:%S.%fZ")
         return date
 
     def getPrice(self, symbol:str=None, base: str = None, quote: str = None):
 
         if symbol is None:
             price = self.getPrice(symbol=base+"/"+quote)
             if price is not None:
```

### Comparing `coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py` & `coinlib-2.2.7/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py` & `coinlib-2.2.7/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/logics/onlineManager/LogicOnlineJobBroker.py` & `coinlib-2.2.7/coinlib/logics/onlineManager/LogicOnlineJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/notification/Notification.py` & `coinlib-2.2.7/coinlib/notification/Notification.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/notification/NotificationWorker.py` & `coinlib-2.2.7/coinlib/notification/NotificationWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/statistics/StatisticMethodJob.py` & `coinlib-2.2.7/coinlib/statistics/StatisticMethodJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/statistics/StatisticRuleJob.py` & `coinlib-2.2.7/coinlib/statistics/StatisticRuleJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/statistics/Statistics.py` & `coinlib-2.2.7/coinlib/statistics/Statistics.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/statistics/StatisticsMethodWorker.py` & `coinlib-2.2.7/coinlib/statistics/StatisticsMethodWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/statistics/StatisticsRuleWorker.py` & `coinlib-2.2.7/coinlib/statistics/StatisticsRuleWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/symbols/SymbolWorker.py` & `coinlib-2.2.7/coinlib/symbols/SymbolWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib/symbols/Symbols.py` & `coinlib-2.2.7/coinlib/symbols/Symbols.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/coinlib.egg-info/PKG-INFO` & `coinlib-2.2.7/coinlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.6
+Version: 2.2.7
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.6/coinlib.egg-info/SOURCES.txt` & `coinlib-2.2.7/coinlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/setup.py` & `coinlib-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README_pip.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="coinlib",
-    version="2.2.6",
+    version="2.2.7",
     description="Develop new code for your coindeck environment",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/coindeck/coinlib",
     author="coindeck",
     author_email="donnercody86@gmail.com",
     license="MIT",
```

### Comparing `coinlib-2.2.6/test/testchartworker.py` & `coinlib-2.2.7/test/testchartworker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/test/testcross.py` & `coinlib-2.2.7/test/testcross.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.6/test/testplot.py` & `coinlib-2.2.7/test/testplot.py`

 * *Files identical despite different names*

