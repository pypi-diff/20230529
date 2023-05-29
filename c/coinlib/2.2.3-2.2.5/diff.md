# Comparing `tmp/coinlib-2.2.3.tar.gz` & `tmp/coinlib-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coinlib-2.2.3.tar", last modified: Fri May 19 06:58:40 2023, max compression
+gzip compressed data, was "dist/coinlib-2.2.5.tar", last modified: Mon May 29 19:12:28 2023, max compression
```

## Comparing `coinlib-2.2.3.tar` & `coinlib-2.2.5.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.357585 coinlib-2.2.3/
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-19 06:58:40.356585 coinlib-2.2.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.336585 coinlib-2.2.3/coinlib/
--rw-rw-rw-   0 root         (0) root         (0)    27933 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/BasicJob.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/BasicJobSessionStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/ChartsFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9436 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/ChartsIndicatorJob.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/ChartsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/CoinlibCrypto.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/CoinlibDataInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/CoinlibWorkspace.py
--rw-rw-rw-   0 root         (0) root         (0)    26721 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/DataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/InfluxDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/PluginLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     6388 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/PluginsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5960 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/Registrar.py
--rw-rw-rw-   0 root         (0) root         (0)    17647 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/Simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    13006 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/WorkerJobProcess.py
--rw-rw-rw-   0 root         (0) root         (0)     5812 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.340585 coinlib-2.2.3/coinlib/broker/
--rw-rw-rw-   0 root         (0) root         (0)     7229 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/Broker.py
--rw-rw-rw-   0 root         (0) root         (0)     4411 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/BrokerDTO.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBrokerFuture.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBrokerMargin.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBrokerSpot.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibSessionManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.341585 coinlib-2.2.3/coinlib/brokerWorker/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     7841 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerSession.py
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerSessionWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/TestProtocolResult.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/coinlibFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.342585 coinlib-2.2.3/coinlib/data/
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/data/CollectionInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/data/DataTable.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    78656 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/dataWorker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   164353 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/dataWorker_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.343585 coinlib-2.2.3/coinlib/drawable/
--rw-rw-rw-   0 root         (0) root         (0)     3528 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/CoinlibDrawable.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/DrawableComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/WindowGrid.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.343585 coinlib-2.2.3/coinlib/event/
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/event/EventConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/event/EventInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.345585 coinlib-2.2.3/coinlib/feature/
--rw-rw-rw-   0 root         (0) root         (0)    14475 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeature.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeatureFetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeatureLake.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeatureProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/FeatureDTO.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/FeatureFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9545 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/FeatureWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     6088 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/Features.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/helper.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/index.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.350585 coinlib-2.2.3/coinlib/logics/
--rw-rw-rw-   0 root         (0) root         (0)    13495 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/Logic.py
--rw-rw-rw-   0 root         (0) root         (0)     8794 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicBasicWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicDTo.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicJob.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineJob.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerData.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerScreener.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerTrader.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineDataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineJob.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineScreenerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineTraderWorker.py
--rw-rw-rw-   0 root         (0) root         (0)    14919 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8512 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicRegistrationInstance.py
--rw-rw-rw-   0 root         (0) root         (0)    16758 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicTestBrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.350585 coinlib-2.2.3/coinlib/logics/broker/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/broker/LogicBrokerInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.351585 coinlib-2.2.3/coinlib/logics/manager/
--rw-rw-rw-   0 root         (0) root         (0)     7098 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/LogicJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/LogicManager.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/PortfolioModel.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.352585 coinlib-2.2.3/coinlib/logics/offlineManager/
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
--rw-rw-rw-   0 root         (0) root         (0)    11492 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.352585 coinlib-2.2.3/coinlib/logics/onlineManager/
--rw-rw-rw-   0 root         (0) root         (0)     6706 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/onlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.353585 coinlib-2.2.3/coinlib/notification/
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/Notification.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/NotificationFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/NotificationWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.355585 coinlib-2.2.3/coinlib/statistics/
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticMethodJob.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticRuleJob.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/Statistics.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsMethodFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsMethodWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsRuleFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     6204 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsRuleWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.356585 coinlib-2.2.3/coinlib/symbols/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/SymbolFactory.py
--rw-rw-rw-   0 root         (0) root         (0)    14991 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/SymbolWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/Symbols.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.338585 coinlib-2.2.3/coinlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3789 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 06:58:40.357585 coinlib-2.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-19 06:58:28.000000 coinlib-2.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.356585 coinlib-2.2.3/test/
--rw-rw-rw-   0 root         (0) root         (0)     4048 2023-05-19 06:58:28.000000 coinlib-2.2.3/test/testchartworker.py
--rw-rw-rw-   0 root         (0) root         (0)    10860 2023-05-19 06:58:28.000000 coinlib-2.2.3/test/testcross.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-05-19 06:58:28.000000 coinlib-2.2.3/test/testplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.591048 coinlib-2.2.5/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-29 19:12:28.591048 coinlib-2.2.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.569049 coinlib-2.2.5/coinlib/
+-rw-rw-rw-   0 root         (0) root         (0)    27933 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/BasicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     7817 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/BasicJobSessionStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/ChartsFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9523 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/ChartsIndicatorJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     9404 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/ChartsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/CoinlibCrypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/CoinlibDataInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/CoinlibWorkspace.py
+-rw-rw-rw-   0 root         (0) root         (0)    26721 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/DataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/InfluxDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/PluginLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/PluginsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5960 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/Registrar.py
+-rw-rw-rw-   0 root         (0) root         (0)    17647 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/Simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    13006 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/WorkerJobProcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     5812 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.572049 coinlib-2.2.5/coinlib/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     7229 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/Broker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/BrokerDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBrokerFuture.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBrokerMargin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBrokerSpot.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibSessionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.574049 coinlib-2.2.5/coinlib/brokerWorker/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7841 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerSession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerSessionWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/TestProtocolResult.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/coinlibFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.574049 coinlib-2.2.5/coinlib/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/data/CollectionInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/data/DataTable.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    78694 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/dataWorker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   164353 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/dataWorker_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.575049 coinlib-2.2.5/coinlib/drawable/
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/CoinlibDrawable.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/DrawableComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/WindowGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.576048 coinlib-2.2.5/coinlib/event/
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/event/EventConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/event/EventInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.578049 coinlib-2.2.5/coinlib/feature/
+-rw-rw-rw-   0 root         (0) root         (0)    17646 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeatureFetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeatureLake.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeatureProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/FeatureDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/FeatureFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9545 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/FeatureWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6088 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/Features.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13456 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.583048 coinlib-2.2.5/coinlib/logics/
+-rw-rw-rw-   0 root         (0) root         (0)    13495 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/Logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicBasicWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicDTo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerData.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerScreener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerTrader.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineDataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineScreenerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineTraderWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14919 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8512 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicRegistrationInstance.py
+-rw-rw-rw-   0 root         (0) root         (0)    16758 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicTestBrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.583048 coinlib-2.2.5/coinlib/logics/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/broker/LogicBrokerInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.584048 coinlib-2.2.5/coinlib/logics/manager/
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/LogicJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/LogicManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/PortfolioModel.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.585048 coinlib-2.2.5/coinlib/logics/offlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)    20273 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11492 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.586048 coinlib-2.2.5/coinlib/logics/onlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)     6706 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/onlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.587048 coinlib-2.2.5/coinlib/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/Notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/NotificationFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/NotificationWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.589048 coinlib-2.2.5/coinlib/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticMethodJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticRuleJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/Statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsMethodFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsMethodWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsRuleFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsRuleWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.590048 coinlib-2.2.5/coinlib/symbols/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/SymbolFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14991 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/SymbolWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/Symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.570049 coinlib-2.2.5/coinlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 19:12:28.591048 coinlib-2.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-29 19:12:15.000000 coinlib-2.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.590048 coinlib-2.2.5/test/
+-rw-rw-rw-   0 root         (0) root         (0)     4048 2023-05-29 19:12:15.000000 coinlib-2.2.5/test/testchartworker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10860 2023-05-29 19:12:15.000000 coinlib-2.2.5/test/testcross.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-05-29 19:12:15.000000 coinlib-2.2.5/test/testplot.py
```

### Comparing `coinlib-2.2.3/PKG-INFO` & `coinlib-2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.3
+Version: 2.2.5
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.3/coinlib/BasicJob.py` & `coinlib-2.2.5/coinlib/BasicJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/BasicJobSessionStorage.py` & `coinlib-2.2.5/coinlib/BasicJobSessionStorage.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/ChartsIndicatorJob.py` & `coinlib-2.2.5/coinlib/ChartsIndicatorJob.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         return rgbhex
     
     def series(self, chartType, name, data, color=None,
                opacity=None,
                chartTypeIcon=None,
                size=None, tooltip=True, chart=None,
                fill=None, fill_from=None,
-               connectGaps=False):
+               fill_to=None, connectGaps=False):
         """
         Create a visible data series. This is the "rendered" Data in the chart.
 
         @chartType:
                     cloud,
                     series,
                     horizontal, (data can be single float or int)
@@ -214,14 +214,16 @@
             options["tooltip"] = tooltip
         if size is not None:
             options["size"] = size
         if fill is not None:
             options["fill"] = fill
         if fill_from is not None:
             options["fill_from"] = fill_from
+        if fill_to is not None:
+            options["fill_to"] = fill_to
         if chartType == "cross":
             options["chartTypeIcon"] = "\ue84a"
         if chartTypeIcon is not None:
             options["chartTypeIcon"] = chartTypeIcon
 
         options["additional"] = json.dumps(additional)
         options["connectGaps"] = connectGaps
```

### Comparing `coinlib-2.2.3/coinlib/ChartsWorker.py` & `coinlib-2.2.5/coinlib/ChartsWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
             partialData.chartInfo.color = options["color"]
         if "tooltip" in options:
             partialData.chartInfo.tooltip = options["tooltip"]
         if "size" in options:
             partialData.chartInfo.size = options["size"]
         if "fill" in options:
             partialData.chartInfo.fill = options["fill"]
+        if "fill_to" in options:
+            partialData.chartInfo.fill_to = options["fill_to"]
         if "fill_from" in options:
             partialData.chartInfo.fill_from = options["fill_from"]
         if "opacity" in options:
             partialData.chartInfo.opacity = options["opacity"]
         if "chartTypeIcon" in options:
             partialData.chartInfo.chartTypeIcon = options["chartTypeIcon"]
         if "chart" in options and options["chart"] is not None:
```

### Comparing `coinlib-2.2.3/coinlib/CoinlibCrypto.py` & `coinlib-2.2.5/coinlib/CoinlibCrypto.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/CoinlibDataInterface.py` & `coinlib-2.2.5/coinlib/CoinlibDataInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/CoinlibWorkspace.py` & `coinlib-2.2.5/coinlib/CoinlibWorkspace.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/DataWorker.py` & `coinlib-2.2.5/coinlib/DataWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/Functions.py` & `coinlib-2.2.5/coinlib/Functions.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/InfluxDatabase.py` & `coinlib-2.2.5/coinlib/InfluxDatabase.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/PluginLoader.py` & `coinlib-2.2.5/coinlib/PluginLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/PluginsWorker.py` & `coinlib-2.2.5/coinlib/PluginsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/Registrar.py` & `coinlib-2.2.5/coinlib/Registrar.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/Simulator.py` & `coinlib-2.2.5/coinlib/Simulator.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/WorkerJobProcess.py` & `coinlib-2.2.5/coinlib/WorkerJobProcess.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/__init__.py` & `coinlib-2.2.5/coinlib/__init__.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/broker/Broker.py` & `coinlib-2.2.5/coinlib/broker/Broker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/broker/BrokerDTO.py` & `coinlib-2.2.5/coinlib/broker/BrokerDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/broker/CoinlibBroker.py` & `coinlib-2.2.5/coinlib/broker/CoinlibBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/broker/CoinlibBrokerFuture.py` & `coinlib-2.2.5/coinlib/broker/CoinlibBrokerFuture.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/broker/CoinlibBrokerMargin.py` & `coinlib-2.2.5/coinlib/broker/CoinlibBrokerMargin.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/broker/CoinlibBrokerSpot.py` & `coinlib-2.2.5/coinlib/broker/CoinlibBrokerSpot.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/brokerWorker/BrokerSession.py` & `coinlib-2.2.5/coinlib/brokerWorker/BrokerSession.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/brokerWorker/BrokerSessionWorker.py` & `coinlib-2.2.5/coinlib/brokerWorker/BrokerSessionWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/brokerWorker/BrokerWorker.py` & `coinlib-2.2.5/coinlib/brokerWorker/BrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/brokerWorker/TestProtocolResult.py` & `coinlib-2.2.5/coinlib/brokerWorker/TestProtocolResult.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/coinlibFactory.py` & `coinlib-2.2.5/coinlib/coinlibFactory.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/config.py` & `coinlib-2.2.5/coinlib/config.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/data/CollectionInterface.py` & `coinlib-2.2.5/coinlib/data/CollectionInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/data/DataTable.py` & `coinlib-2.2.5/coinlib/data/DataTable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/dataWorker_pb2.py` & `coinlib-2.2.5/coinlib/dataWorker_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61taWorker.proto\x12\x07\x63oinlib\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x19google/protobuf/any.proto\"P\n\tWorkerJob\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\"k\n\x0eWorkerJobError\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\x12\x14\n\x0c\x65rrorMessage\x18\x04 \x01(\t\"E\n\x16WorkerAvailablePlugins\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\xb7\x01\n\x06Worker\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x02 \x01(\t\x12\x13\n\x0bworker_mode\x18\x03 \x01(\t\x12\x39\n\x10\x61vailablePlugins\x18\x04 \x03(\x0b\x32\x1f.coinlib.WorkerAvailablePlugins\x12\n\n\x02os\x18\x05 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x06 \x01(\t\x12\x15\n\ractiveModules\x18\x07 \x03(\t\"\x1a\n\x07RowData\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\";\n\x15WorkerJobDataResponse\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x16\n\x14WorkerJobDataPartial\"\xec\x01\n\x1a\x43hartWorkerPartialDataInfo\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x02\x12\x0f\n\x07opacity\x18\x05 \x01(\x02\x12\x15\n\rchartTypeIcon\x18\x06 \x01(\t\x12\x0f\n\x07tooltip\x18\x07 \x01(\x08\x12\r\n\x05\x63hart\x18\x08 \x01(\t\x12\x13\n\x0b\x63onnectGaps\x18\t \x01(\x08\x12\x11\n\tfill_from\x18\n \x01(\x02\x12\x0c\n\x04\x66ill\x18\x0b \x01(\t\x12\x12\n\nadditional\x18\x0c \x01(\t\"\xad\x01\n\x1d\x43hartsWorkerPartialDataLayout\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x02 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x36\n\tchartInfo\x18\x03 \x01(\x0b\x32#.coinlib.ChartWorkerPartialDataInfo\"\xdd\x01\n\x14\x43hartWorkerIndicator\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07\x66\x65\x61ture\x18\x03 \x01(\t\x12\x12\n\nsubfeature\x18\x04 \x01(\t\x12\r\n\x05short\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\x11\n\telementId\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tid_output\x18\n \x01(\t\x12\x10\n\x08\x66inished\x18\x0b \x01(\x08\x12\x0f\n\x07\x63hartId\x18\x0c \x01(\t\"\xdc\x02\n ChartWorkerIndicatorRegistration\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x11\n\tid_output\x18\x06 \x01(\t\x12\x0e\n\x06inputs\x18\x07 \x01(\x0c\x12\x0c\n\x04mode\x18\x08 \x01(\t\x12\x19\n\x11short_description\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07process\x18\x0b \x01(\t\x12\x16\n\x0eunstablePeriod\x18\x0c \x01(\x08\x12\x19\n\x11\x64ynamicTimeseries\x18\r \x01(\x08\x12\x0e\n\x06plugin\x18\x0e \x01(\t\x12\x15\n\rpluginVersion\x18\x0f \x01(\t\x12\x11\n\tcode_type\x18\x10 \x01(\t\x12\x0c\n\x04\x63ode\x18\x11 \x01(\t\"n\n!ChartWorkerIndicatorConfigElement\x12\x30\n\tindicator\x18\x01 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x17\n\x0findicatorConfig\x18\x02 \x01(\x0c\"\xac\x01\n\x12\x43hartsWorkerConfig\x12<\n\x08\x65lements\x18\x01 \x03(\x0b\x32*.coinlib.ChartWorkerIndicatorConfigElement\x12-\n\x08\x63hildren\x18\x02 \x01(\x0b\x32\x1b.coinlib.ChartsWorkerConfig\x12)\n\tchartData\x18\x03 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\"-\n\x0eStatisticInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"A\n\tDataError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x11\n\terrorCode\x18\x02 \x01(\x03\x12\x10\n\x08\x63ritical\x18\x03 \x01(\x08\"\x89\x01\n\x0eIndicatorError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x03 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\"\xa3\x01\n\x1aStatisticRuleFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa5\x01\n\x1cStatisticMethodFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xb2\x01\n\"StatisticsMethodWorkerWindowConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\x10\n\x08windowId\x18\x03 \x01(\t\x12)\n\tchartData\x18\x04 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x05 \x01(\x0b\x32\x17.coinlib.ParameterTable\"R\n\x13ParameterTableEntry\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08required\x18\x04 \x01(\x08\"B\n\x0eParameterTable\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.coinlib.ParameterTableEntry\"z\n\rChartDataInfo\x12\x10\n\x08\x63hart_id\x18\x01 \x01(\t\x12\x14\n\x0c\x63hart_prefix\x18\x02 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\t\x12\x13\n\x0b\x61\x63tivity_id\x18\x04 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x05 \x01(\t\"\xf6\x02\n\x1aStatisticsRuleWorkerConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x05rules\x18\x02 \x03(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x19\n\x11statisticFunction\x18\x03 \x01(\t\x12?\n\x06inputs\x18\x04 \x03(\x0b\x32/.coinlib.StatisticsRuleWorkerConfig.InputsEntry\x12\x12\n\ncombinator\x18\x05 \x01(\t\x12\x16\n\x0e\x63ombinator_not\x18\x06 \x01(\x08\x12\x0c\n\x04type\x18\x07 \x01(\t\x12)\n\tchartData\x18\x08 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x1a\x46\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.coinlib.StatisticInput:\x02\x38\x01\"\xa8\x01\n\x1eStatisticsRuleWorkerConfigType\x12\x33\n\x04rule\x18\x01 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfigH\x00\x12\x43\n\x0cmethodWindow\x18\x02 \x01(\x0b\x32+.coinlib.StatisticsMethodWorkerWindowConfigH\x00\x42\x0c\n\ntest_oneof\"\xb4\x01\n\x1cStatisticsBulkedWorkerConfig\x12\x38\n\x07\x63onfigs\x18\x01 \x03(\x0b\x32\'.coinlib.StatisticsRuleWorkerConfigType\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x03 \x01(\x0b\x32\x17.coinlib.ParameterTable\"\x9f\x01\n\x16StatisticFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa7\x01\n\x1cStatisticMethodPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x12\n\ndocumentId\x18\x03 \x01(\t\x12\r\n\x05width\x18\x04 \x01(\t\x12\x0e\n\x06height\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x10\n\x08windowId\x18\x07 \x01(\t\"\xa6\x01\n\x1aStatisticRulePartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12:\n\rstatisticRule\x18\x02 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x14\n\x0c\x63ollectionid\x18\x03 \x01(\t\x12\x12\n\nresultName\x18\x05 \x01(\t\"\xa2\x01\n\x1cStatisticBulkedPartiallyData\x12;\n\nmethodData\x18\x01 \x01(\x0b\x32%.coinlib.StatisticMethodPartiallyDataH\x00\x12\x37\n\x08ruleData\x18\x02 \x01(\x0b\x32#.coinlib.StatisticRulePartiallyDataH\x00\x42\x0c\n\ntest_oneof\"m\n\x11SymbolBrokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"U\n\x19SymbolBrokerConsumerError\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\"\x95\x02\n\x16SymbolBrokerMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04open\x18\x02 \x01(\x02\x12\r\n\x05\x63lose\x18\x03 \x01(\x02\x12\x0c\n\x04high\x18\x04 \x01(\x02\x12\x0b\n\x03low\x18\x05 \x01(\x02\x12\x0e\n\x06volume\x18\x06 \x01(\x02\x12\r\n\x05trade\x18\x07 \x01(\x02\x12\x10\n\x08\x64\x61tetime\x18\x08 \x01(\t\x12\x11\n\tsymbol_id\x18\t \x01(\t\x12\x0e\n\x06symbol\x18\n \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x0b \x01(\t\x12\x12\n\nevent_time\x18\x0c \x01(\t\x12\x0f\n\x07isfinal\x18\r \x01(\x08\x12\x11\n\tcloseTime\x18\x0e \x01(\t\"\x96\x01\n\x10SymbolBrokerInfo\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\texchanges\x18\x02 \x03(\x0b\x32\x1d.coinlib.SymbolBrokerExchange\x12,\n\x07symbols\x18\x03 \x03(\x0b\x32\x1b.coinlib.SymbolBrokerSymbol\";\n\x15SymbolBrokerOrderbook\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"F\n SymbolBrokerHistoricalMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\xba\x01\n\x14SymbolBrokerExchange\x12\x0c\n\x04icon\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07website\x18\x04 \x01(\t\x12\x15\n\rsymbols_count\x18\x05 \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x06 \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\x07 \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x08 \x01(\x02\"\x8c\x04\n\x12SymbolBrokerSymbol\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x38\n\tassetType\x18\x04 \x01(\x0e\x32%.coinlib.SymbolBrokerSymbol.AssetType\x12>\n\x0c\x63ontractType\x18\x05 \x01(\x0e\x32(.coinlib.SymbolBrokerSymbol.ContractType\x12\x0c\n\x04\x62\x61se\x18\x06 \x01(\t\x12\r\n\x05quote\x18\x07 \x01(\t\x12\x1a\n\x12\x65xchange_symbol_id\x18\x08 \x01(\t\x12\x16\n\x0esize_precision\x18\t \x01(\x02\x12\x17\n\x0fprice_precision\x18\n \x01(\x02\x12\r\n\x05price\x18\x0b \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x0c \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\r \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x0e \x01(\x02\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"O\n\x1cSymbolBrokerBrokerInfoConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\"\xdd\x03\n#SymbolBrokerConsumeMarketdataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12O\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x39.coinlib.SymbolBrokerConsumeMarketdataConfig.ContractType\x12I\n\tassetType\x18\t \x01(\x0e\x32\x36.coinlib.SymbolBrokerConsumeMarketdataConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xda\x03\n\"SymbolBrokerConsumeOrderbookConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12N\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x38.coinlib.SymbolBrokerConsumeOrderbookConfig.ContractType\x12H\n\tassetType\x18\t \x01(\x0e\x32\x35.coinlib.SymbolBrokerConsumeOrderbookConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xb8\x04\n#SymbolBrokerGetHistoricalDataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\t\x12\x0b\n\x03\x65nd\x18\x08 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\t \x01(\t\x12)\n\tchartData\x18\n \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12O\n\x0c\x63ontractType\x18\x0b \x01(\x0e\x32\x39.coinlib.SymbolBrokerGetHistoricalDataConfig.ContractType\x12I\n\tassetType\x18\x0c \x01(\x0e\x32\x36.coinlib.SymbolBrokerGetHistoricalDataConfig.AssetType\x12\x12\n\nreturnData\x18\r \x01(\x08\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xc5\x02\n\x18SymbolBrokerWorkerConfig\x12;\n\ninfoConfig\x18\x01 \x01(\x0b\x32%.coinlib.SymbolBrokerBrokerInfoConfigH\x00\x12\x45\n\rconsumeConfig\x18\x02 \x01(\x0b\x32,.coinlib.SymbolBrokerConsumeMarketdataConfigH\x00\x12M\n\x16\x63onsumeOrderbookConfig\x18\x03 \x01(\x0b\x32+.coinlib.SymbolBrokerConsumeOrderbookConfigH\x00\x12H\n\x10historicalConfig\x18\x04 \x01(\x0b\x32,.coinlib.SymbolBrokerGetHistoricalDataConfigH\x00\x42\x0c\n\ntest_oneof\"F\n SymbolBrokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"2\n\x1fSymbolBrokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"j\n\x15SymbolBrokerFetchData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12-\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x1f.coinlib.SymbolBrokerMarketData\"u\n$NotificationExtractMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\t\x12\x0f\n\x07options\x18\x04 \x01(\t\"\xd3\x01\n!NotificationSendMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0e\n\x06images\x18\x04 \x01(\t\x12\x0f\n\x07\x62uttons\x18\x05 \x01(\t\x12\x0f\n\x07options\x18\x06 \x01(\t\x12\x13\n\x0b\x63\x61llback_id\x18\x07 \x01(\t\x12\x14\n\x0c\x63\x61llback_url\x18\x08 \x01(\t\x12\x10\n\x08\x63hannels\x18\t \x01(\t\"\xbd\x01\n\x18NotificationWorkerConfig\x12G\n\x11sendMessageConfig\x18\x01 \x01(\x0b\x32*.coinlib.NotificationSendMessageDataConfigH\x00\x12J\n\x11\x65xtractDataConfig\x18\x02 \x01(\x0b\x32-.coinlib.NotificationExtractMessageDataConfigH\x00\x42\x0c\n\ntest_oneof\"Z\n\x11NotificationError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"b\n\x1bNotificationCallbackExtract\x12\x11\n\tbutton_id\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x98\x01\n\x0eLogicComponent\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x18\n\x10logicComponentId\x18\x03 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\x0c\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x14\n\x0clogicDetails\x18\x07 \x01(\t\"\xde\x03\n\x12\x42rokerAccountModel\x12:\n\nbrokerType\x18\x01 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerType\x12\x34\n\x04mode\x18\x02 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerMode\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x10\n\x08makerFee\x18\x04 \x01(\x02\x12\x10\n\x08takerFee\x18\x05 \x01(\x02\x12\x39\n\x0cmakerFeeMode\x18\x06 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\x12\x39\n\x0ctakerFeeMode\x18\x07 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\"Q\n\nBrokerType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"1\n\nBrokerMode\x12\x0e\n\nBACKTRADER\x10\x00\x12\t\n\x05PAPER\x10\x01\x12\x08\n\x04LIVE\x10\x02\"$\n\x07\x46\x65\x65Mode\x12\x0e\n\nPERCENTAGE\x10\x00\x12\t\n\x05\x46IXED\x10\x01\"~\n\x0ePortfolioAsset\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x03 \x01(\x02\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\x0e\n\x06locked\x18\x05 \x01(\x02\x12\x11\n\tlastPrice\x18\x06 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x07 \x01(\t\"o\n\x13\x43\x61lculatedBaseMoney\x12\r\n\x05total\x18\x01 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x0f\n\x07summary\x18\x04 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\"\xc0\x01\n\x0ePortfolioModel\x12\'\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x17.coinlib.PortfolioAsset\x12@\n\x1a\x63urrentCalculatedBaseMoney\x18\x02 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\x43\n\x1dhistoricalCalculatedBaseMoney\x18\x03 \x03(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\"\x82\x03\n\x10LogicRunnerLogic\x12)\n\tchartData\x18\x01 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x30\n\x0flogicComponents\x18\x02 \x03(\x0b\x32\x17.coinlib.LogicComponent\x12\x11\n\tstartDate\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x04 \x01(\t\x12*\n\tportfolio\x18\x05 \x01(\x0b\x32\x17.coinlib.PortfolioModel\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\x12/\n\x0eparameterTable\x18\x07 \x01(\x0b\x32\x17.coinlib.ParameterTable\x12\x11\n\tlogicMode\x18\x08 \x01(\t\x12\x15\n\rapp_worker_id\x18\t \x01(\t\x12\x1c\n\x14\x61pp_worker_runner_id\x18\n \x01(\t\x12\x14\n\x0coptions_json\x18\x0b \x01(\t\"\xd5\x01\n\x1eLogicRunnerOfflineWorkerConfig\x12,\n\tlogicInfo\x18\x01 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12+\n\tportfolio\x18\x03 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x18\n\x10\x61\x64vancedDataInfo\x18\x04 \x01(\t\x12\x13\n\x0bonlySignals\x18\x05 \x01(\x08\"\xcf\x04\n\x15LogicRunnerStatistics\x12\x1f\n\x17highestProfitPercentage\x18\x01 \x01(\x02\x12\x1d\n\x15highestLossPercentage\x18\x02 \x01(\x02\x12\x11\n\tsinceDate\x18\x03 \x01(\t\x12\x0e\n\x06\x61tDate\x18\x04 \x01(\t\x12\x11\n\ttradesCnt\x18\x05 \x01(\x02\x12\x35\n\x0f\x63\x61lculatedMoney\x18\x06 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\"\n\x1aunrealizedProfitPercentage\x18\x07 \x01(\x02\x12\x0c\n\x04\x66\x65\x65s\x18\x08 \x01(\x02\x12 \n\x18profitCompletePercentage\x18\t \x01(\x02\x12\x1d\n\x15highestProfitPerGroup\x18\n \x01(\x02\x12\x1b\n\x13highestLossPerGroup\x18\x0b \x01(\x02\x12\x18\n\x10slippagePerGroup\x18\x0c \x01(\x02\x12\x1a\n\x12\x61verageAmountQuote\x18\r \x01(\x02\x12\'\n\x1f\x61verageProfitPercentagePergroup\x18\x0e \x01(\x02\x12\x19\n\x11portfolioTimeline\x18\x0f \x01(\t\x12\x14\n\x0cwinLossRatio\x18\x10 \x01(\x02\x12\x0e\n\x06winCnt\x18\x11 \x01(\x02\x12\x0f\n\x07lossCnt\x18\x12 \x01(\x02\x12\x17\n\x0fsecondsInMarket\x18\x13 \x01(\x02\x12\x1d\n\x15\x61verageSecondsInTrade\x18\x14 \x01(\x02\x12\x10\n\x08\x64rawDown\x18\x15 \x01(\x02\"\xa6\x01\n%LogicRunnerOfflineWorkerPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\npercentage\x18\x02 \x01(\x02\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x05 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"w\n\x1dLogicRunnerOfflineWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xb4\x01\n$LogicRunnerOfflineWorkerFinishedData\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x04 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"K\n\rWorkspaceInfo\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x11\n\tdataSetId\x18\x02 \x01(\t\x12\x12\n\nactivityId\x18\x03 \x01(\t\"@\n\x17WorkerPluginInformation\x12%\n\x06plugin\x18\x01 \x03(\x0b\x32\x15.coinlib.PluginConfig\"<\n\x0eWorkerSettings\x12\x15\n\ractiveModules\x18\x01 \x03(\t\x12\x13\n\x0bworker_mode\x18\x02 \x01(\t\"\'\n\x12WorkerRegistration\x12\x11\n\tworker_id\x18\x01 \x01(\t\"b\n\x15\x43ollectionNodeRequest\x12\x16\n\x0e\x63ollectionName\x18\x01 \x01(\t\x12\r\n\x05stage\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\":\n\x16\x43ollectionNodeResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsize_in_mb\x18\x02 \x01(\t\"`\n\x0c\x45ventRequest\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\r\n\x05stage\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"t\n\x0cPluginConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x13\n\x0b\x66ilecontent\x18\x04 \x01(\t\x12\x10\n\x08testOnly\x18\x05 \x01(\x08\x12\x10\n\x08\x66iletype\x18\x06 \x01(\t\"U\n\x18PluginInstallationOutput\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x15\n\routputMessage\x18\x02 \x01(\t\"\xcb\x01\n\x1dSimulatorChartConfigIndicator\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nsubfeature\x18\x02 \x01(\t\x12\x42\n\x06inputs\x18\x03 \x03(\x0b\x32\x32.coinlib.SimulatorChartConfigIndicator.InputsEntry\x12\x12\n\nchartIndex\x18\x04 \x01(\t\x1a-\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x14SimulatorChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62roker\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\x97\x01\n\x1dSimulatorStatisticChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\xc7\x01\n\x1eSimulatorMethodCallChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\x12-\n\x07methods\x18\x07 \x03(\x0b\x32\x1c.coinlib.SimulatorMethodCall\"@\n\x11SimulatorResponse\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"\x83\x01\n\x1cSymbolBrokerSimulatorRequest\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x13\n\x0btestSymbol1\x18\x04 \x01(\t\x12\x13\n\x0btestSymbol2\x18\x05 \x01(\t\"g\n\x1dSymbolBrokerSimulatorResponse\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"@\n\x1e\x42rokerSimulatorBrokerLoginData\x12\x0e\n\x06\x61pikey\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"\x95\x01\n\x19\x42rokerSimulatorBrokerData\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12:\n\tloginInfo\x18\x02 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x11\n\tassetType\x18\x03 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x04 \x01(\t\"\x98\x01\n\x16\x42rokerSimulatorRequest\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x36\n\nbrokerInfo\x18\x04 \x01(\x0b\x32\".coinlib.BrokerSimulatorBrokerData\x12\x11\n\tpaperMode\x18\x05 \x01(\x08\"\xb2\x01\n\x17\x42rokerSimulatorResponse\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\x12\x11\n\tsessionId\x18\x04 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x05 \x01(\t\x12\x15\n\rtargetdepotId\x18\x06 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"f\n\x1cNotificationSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0e\n\x06inputs\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x10\n\x08\x63hannels\x18\x04 \x01(\t\"c\n\x1dNotificationSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"P\n\x17\x46\x65\x61tureSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\"^\n\x18\x46\x65\x61tureSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"c\n\nLogicInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x85\x02\n\x17LogicTraderRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x84\x02\n\x16LogicAlertRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x83\x02\n\x15LogicDataRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x87\x02\n\x19LogicScreenerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x91\x02\n\x1aWorkspaceLogicRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x18\n\x10logicComponentId\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\x0c\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0e\n\x06plugin\x18\x05 \x01(\t\x12\x15\n\rpluginVersion\x18\x06 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x07 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x10\n\x08workerId\x18\x0b \x01(\t\x12\x11\n\tautostart\x18\x0c \x01(\x08\x12\x16\n\x0e\x61utostartLogic\x18\r \x01(\x08\"\"\n\x0bLogicRunJob\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\"\xb3\x02\n\x0eLogicDataUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05group\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06symbol\x18\x06 \x01(\x08\x12\x10\n\x08\x65xchange\x18\x07 \x01(\x08\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf3\x01\n\x11LogicMonitorEvent\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf6\x01\n\x14LogicCollectionUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xe2\x01\n\x0fLogicEventUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\\\n\x13SymbolBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xe4\x01\n\x18SymbolBrokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12-\n\x07options\x18\x04 \x03(\x0b\x32\x1c.coinlib.SymbolBrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\"V\n\rBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xda\x03\n\x0e\x42rokerExchange\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x34\n\tloginMode\x18\x04 \x01(\x0e\x32!.coinlib.BrokerExchange.LoginMode\x12;\n\rcontractTypes\x18\x05 \x03(\x0e\x32$.coinlib.BrokerExchange.ContractType\x12\x35\n\nassetTypes\x18\x06 \x03(\x0e\x32!.coinlib.BrokerExchange.AssetType\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0bsupportDemo\x18\x08 \x01(\x08\x12\x13\n\x0bsupportLive\x18\t \x01(\x08\x12\x1a\n\x12positionModeFuture\x18\n \x01(\t\"\x18\n\tLoginMode\x12\x0b\n\x07\x41PI_KEY\x10\x00\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\xa8\x03\n\x12\x42rokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\'\n\x07options\x18\x04 \x03(\x0b\x32\x16.coinlib.BrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12*\n\texchanges\x18\x0b \x03(\x0b\x32\x17.coinlib.BrokerExchange\x12\x45\n\x0b\x62rokerTypes\x18\x0c \x03(\x0e\x32\x30.coinlib.BrokerRegistration.SupportedBrokerTypes\"[\n\x14SupportedBrokerTypes\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"?\n\x0f\x42rokerPortfolio\x12,\n\x05\x61sset\x18\x01 \x03(\x0b\x32\x1d.coinlib.BrokerPortfolioAsset\"Z\n\x14\x42rokerPortfolioAsset\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x11\n\tlastPrice\x18\x04 \x01(\x02\"\x84\x03\n\x18\x42rokerSessionAccountInfo\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x44\n\x0c\x63ontractType\x18\x02 \x01(\x0e\x32..coinlib.BrokerSessionAccountInfo.ContractType\x12>\n\tassetType\x18\x03 \x01(\x0e\x32+.coinlib.BrokerSessionAccountInfo.AssetType\x12:\n\tloginInfo\x18\x04 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x0f\n\x07sandbox\x18\x05 \x01(\x08\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\x9b\x01\n\x1c\x42rokerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\"\xf4\x01\n\x14\x42rokerInfoTestConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\"g\n\x12\x42rokerWorkerConfig\x12\x43\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"@\n\x1a\x42rokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\",\n\x19\x42rokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"\x18\n\x16\x42rokerStartSessionInfo\"g\n\x0b\x42rokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"j\n\x0e\x42rokerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x15\n\rbrokerCommand\x18\x03 \x01(\t\x12\x1b\n\x13\x62rokerCommandParams\x18\x04 \x01(\t\".\n\x19\x42rokerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"P\n\x14\x42rokerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"d\n\x19\x42rokerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"e\n\x0f\x42rokerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\".\n\x19\x42rokerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"J\n\x16\x42rokerTestProtocolData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\x9c\x01\n\x0f\x41ppWorkerConfig\x12\x46\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32(.coinlib.AppWorkerInfoStartSessionConfigH\x00\x12\x33\n\ntestConfig\x18\x02 \x01(\x0b\x32\x1d.coinlib.BrokerInfoTestConfigH\x00\x42\x0c\n\ntest_oneof\"\xa9\x02\n\x1f\x41ppWorkerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x02 \x01(\t\x12,\n\tlogicInfo\x18\x03 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12;\n\x0c\x62rokerConfig\x18\x04 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfig\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x10\n\x08\x63odeType\x18\x07 \x01(\t\x12\x0e\n\x06\x63odeId\x18\x08 \x01(\t\x12\x13\n\x0b\x63odeVersion\x18\t \x01(\t\"1\n\x1c\x41ppWorkerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"W\n\x0e\x41ppWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"q\n\x11\x41ppWorkerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\x12\x0e\n\x06target\x18\x05 \x01(\t\"U\n\x1c\x41ppWorkerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"S\n\x17\x41ppWorkerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"g\n\x1c\x41ppWorkerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"h\n\x12\x41ppWorkerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x83\x01\n\x16\x41ppWorkerBrokerCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x0e\n\x06params\x18\x04 \x01(\t\x12\x11\n\tcommandId\x18\x05 \x01(\t\"\x9f\x01\n\x1c\x41ppWorkerBrokerCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tcommandId\x18\x03 \x01(\t\x12\x10\n\x08response\x18\x04 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12\r\n\x05\x65rror\x18\x06 \x01(\x08\"\x93\x01\n\x16\x41ppWorkerModuleCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\"\xd0\x01\n\x1c\x41ppWorkerModuleCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x07 \x01(\t\x12\r\n\x05\x65rror\x18\x08 \x01(\x08\x12\x10\n\x08response\x18\t \x01(\t\"g\n\x1a\x41ppWorkerFinishedStepInfos\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\"c\n\x19\x41ppWorkerRegistrationInfo\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07success\x18\x03 \x01(\x08\"\xad\x02\n\x1d\x46\x65\x61tureInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x14\n\x0coptionValues\x18\x03 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12\x1c\n\x14targetDatabaseServer\x18\x05 \x01(\t\x12\x18\n\x10targetDatabaseID\x18\x06 \x01(\t\x12\x13\n\x0bsessionData\x18\x07 \x01(\t\x12\x14\n\x0crabbitServer\x18\x08 \x01(\t\x12\x12\n\nrabbitUser\x18\t \x01(\t\x12\x11\n\trabbitPwd\x18\n \x01(\t\x12\x12\n\nrabbitPort\x18\x0b \x01(\t\x12\x19\n\x11rabbitQueuePrefix\x18\x0c \x01(\t\"i\n\x13\x46\x65\x61tureWorkerConfig\x12\x44\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32&.coinlib.FeatureInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"U\n\x0c\x46\x65\x61tureError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"_\n\x0f\x46\x65\x61tureCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\"Q\n\x15\x46\x65\x61tureCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"e\n\x1a\x46\x65\x61tureCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"/\n\x1a\x46\x65\x61tureSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"f\n\x10\x46\x65\x61tureEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\">\n\x17RegistrationInformation\x12\x12\n\nduplicated\x18\x01 \x01(\x08\x12\x0f\n\x07success\x18\x02 \x01(\x08\"I\n\x15SymbolDataRequestInfo\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x02 \x01(\t\"G\n\x12SymbolDataResponse\x12\x31\n\x07symbols\x18\x01 \x03(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\"\x19\n\x17\x45xchangeDataRequestInfo\"L\n\x13\x42rokerExchangeSmall\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04mode\x18\x04 \x01(\t\"G\n\x14\x45xchangeDataResponse\x12/\n\texchanges\x18\x02 \x03(\x0b\x32\x1c.coinlib.BrokerExchangeSmall\"\xae\x02\n\x17SymbolBrokerSymbolSmall\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x11\n\tsymbol_id\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\t\x12\x0c\n\x04\x62\x61se\x18\x05 \x01(\t\x12\r\n\x05quote\x18\x06 \x01(\t\x12\x16\n\x0epricePrecision\x18\x07 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12>\n\x07\x63olumns\x18\n \x03(\x0b\x32-.coinlib.SymbolBrokerSymbolSmall.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb2\x01\n\x11MarketDataRequest\x12\x30\n\x06symbol\x18\x01 \x01(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x05 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x06 \x01(\t\"h\n\x12MarketDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"i\n\x13\x46\x65\x61tureDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"\xa0\x01\n\x12\x46\x65\x61tureDataRequest\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x01 \x03(\t\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x15\n\rtarget_symbol\x18\x04 \x01(\t\x12\x17\n\x0ftarget_exchange\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05stage\x18\x07 \x01(\t\"\x1e\n\x1c\x41\x64\x64itionalDataFeatureRequest\"y\n\x19\x41\x64\x64itionalDataFeatureInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"Y\n\x1d\x41\x64\x64itionalDataFeatureResponse\x12\x38\n\x0c\x66\x65\x61tureInfos\x18\x01 \x03(\x0b\x32\".coinlib.AdditionalDataFeatureInfo\"\\\n\x13NotificationOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\x8f\x02\n\x18NotificationRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.coinlib.NotificationOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12\x15\n\risInteractive\x18\x0c \x01(\x08\"W\n\x0e\x46\x65\x61tureOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xc2\x02\n\x13\x46\x65\x61tureRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12(\n\x07options\x18\x04 \x03(\x0b\x32\x17.coinlib.FeatureOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\x15\n\rfeature_infos\x18\r \x01(\t\x12\x1d\n\x15\x65stimatedDataInterval\x18\x0e \x01(\x03\x12\r\n\x05group\x18\x0f \x01(\t\"5\n\x13SimulatorMethodCall\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\"`\n\x17StatisticFunctionInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"n\n\x15StatisticMethodInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x9d\x02\n\x1bStatisticMethodRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\trefreshOn\x18\x03 \x03(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x1c\n\x14targetPositionLayout\x18\x07 \x01(\t\x12.\n\x06inputs\x18\x08 \x03(\x0b\x32\x1e.coinlib.StatisticMethodInputs\x12\x0e\n\x06plugin\x18\t \x01(\t\x12\x15\n\rpluginVersion\x18\n \x01(\t\x12\x11\n\tcode_type\x18\x0b \x01(\t\x12\x0c\n\x04\x63ode\x18\x0c \x01(\t\"\x83\x02\n!StatisticRuleFunctionRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x30\n\x06inputs\x18\x07 \x03(\x0b\x32 .coinlib.StatisticFunctionInputs\x12\x0e\n\x06plugin\x18\x08 \x01(\t\x12\x15\n\rpluginVersion\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\"A\n\x15WorkerRegistryRequest\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x15\n\ractiveModules\x18\x02 \x03(\t\"D\n\x16WorkerRegistryResponse\x12\x16\n\x0etargetendpoint\x18\x01 \x01(\t\x12\x12\n\ntargetport\x18\x02 \x01(\t\"-\n\x06\x41piKey\x12\x12\n\napi_key_id\x18\x01 \x01(\t\x12\x0f\n\x07modules\x18\x02 \x01(\t\"0\n\x07\x41uthKey\x12\x10\n\x08\x61uth_key\x18\x01 \x01(\t\x12\x13\n\x0bvalid_until\x18\x02 \x01(\t2\xf6\x01\n\x0c\x43hartsWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.ChartsWorkerConfig\"\x00\x12L\n\x17OnIndicatorErrorOccured\x12\x17.coinlib.IndicatorError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnPartialChartLayout\x12&.coinlib.ChartsWorkerPartialDataLayout\x1a\x16.google.protobuf.Empty\"\x00\x32\x9d\x02\n\x16StatisticsMethodWorker\x12H\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a%.coinlib.StatisticsBulkedWorkerConfig\"\x00\x12[\n\x18OnStatisticPartiallyData\x12%.coinlib.StatisticBulkedPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x1fOnStatisticFunctionErrorOccured\x12\x1f.coinlib.StatisticFunctionError\x1a\x16.google.protobuf.Empty\"\x00\x32\xae\x06\n\x12SymbolBrokerWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.SymbolBrokerWorkerConfig\"\x00\x12l\n\x0fwaitForCommands\x12).coinlib.SymbolBrokerStopConsumerListener\x1a(.coinlib.SymbolBrokerStopConsumerCommand\"\x00(\x01\x30\x01\x12[\n\x1fonBrokerFetchSymbolDataReceived\x12\x1e.coinlib.SymbolBrokerFetchData\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x18onHistoricalDataReceived\x12).coinlib.SymbolBrokerHistoricalMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x1aonBrokerSymbolInfoReceived\x12\x19.coinlib.SymbolBrokerInfo\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x14onMarketDataReceived\x12\x1f.coinlib.SymbolBrokerMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x13onOrderbookReceived\x12\x1e.coinlib.SymbolBrokerOrderbook\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnSymbolBrokerErrorOccured\x12\x1a.coinlib.SymbolBrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12[\n\x1bonBrokerSymbolTickerCrashed\x12\".coinlib.SymbolBrokerConsumerError\x1a\x16.google.protobuf.Empty\"\x00\x32\x89\x02\n\x12NotificationWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.NotificationWorkerConfig\"\x00\x12Y\n\x17OnCallbackDataExtracted\x12$.coinlib.NotificationCallbackExtract\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnNotificationErrorOccured\x12\x1a.coinlib.NotificationError\x1a\x16.google.protobuf.Empty\"\x00\x32\xea\x03\n\x19LogicRunnerOfflineService\x12J\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12_\n\x1aGetLogicConfigForWorkspace\x12\x16.coinlib.WorkspaceInfo\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12\x61\n\x15OnRunnerPartiallyData\x12..coinlib.LogicRunnerOfflineWorkerPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnRunnerErrorOccured\x12&.coinlib.LogicRunnerOfflineWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x18OnRunnerFinishedComplete\x12-.coinlib.LogicRunnerOfflineWorkerFinishedData\x1a\x16.google.protobuf.Empty\"\x00\x32\xcd\x05\n\nDataWorker\x12?\n\x0f\x41\x63\x63\x65ptWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x10\x44\x65\x63lineWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\tFireEvent\x12\x15.coinlib.EventRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x14GetNodeForCollection\x12\x1e.coinlib.CollectionNodeRequest\x1a\x1f.coinlib.CollectionNodeResponse\"\x00\x12<\n\x0eRegisterWorker\x12\x0f.coinlib.Worker\x1a\x17.coinlib.WorkerSettings\"\x00\x12\x44\n\rGetAllPlugins\x12\x0f.coinlib.Worker\x1a .coinlib.WorkerPluginInformation\"\x00\x12K\n\x0fUpdateWorkerJob\x12\x1e.coinlib.WorkerJobDataResponse\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0fWatchWorkerJobs\x12\x1b.coinlib.WorkerRegistration\x1a\x12.coinlib.WorkerJob\"\x00(\x01\x30\x01\x12\x41\n\x11\x46inishedWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x10\x45rroredWorkerJob\x12\x17.coinlib.WorkerJobError\x1a\x16.google.protobuf.Empty\"\x00\x32\x9f\x01\n\x0cPluginWorker\x12\x38\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x15.coinlib.PluginConfig\"\x00\x12U\n\x14OnInstallationOutput\x12!.coinlib.PluginInstallationOutput\x1a\x16.google.protobuf.Empty\"\x00(\x01\x32\x9f\x05\n\tSimulator\x12X\n\x0fsimulateFeature\x12 .coinlib.FeatureSimulatorRequest\x1a!.coinlib.FeatureSimulatorResponse\"\x00\x12L\n\rsimulateChart\x12\x1d.coinlib.SimulatorChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12^\n\x16simulateStatisticsRule\x12&.coinlib.SimulatorStatisticChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12\x61\n\x18simulateStatisticsMethod\x12\'.coinlib.SimulatorMethodCallChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12g\n\x14simulateSymbolBroker\x12%.coinlib.SymbolBrokerSimulatorRequest\x1a&.coinlib.SymbolBrokerSimulatorResponse\"\x00\x12U\n\x0esimulateBroker\x12\x1f.coinlib.BrokerSimulatorRequest\x1a .coinlib.BrokerSimulatorResponse\"\x00\x12g\n\x14simulateNotification\x12%.coinlib.NotificationSimulatorRequest\x1a&.coinlib.NotificationSimulatorResponse\"\x00\x32m\n\tFunctions\x12`\n\x19registerIndicatorFunction\x12).coinlib.ChartWorkerIndicatorRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xbc\x05\n\x05Logic\x12\x46\n\x11registerDataUsage\x12\x17.coinlib.LogicDataUsage\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x14registerMonitorEvent\x12\x1a.coinlib.LogicMonitorEvent\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x12registerEventUsage\x12\x18.coinlib.LogicEventUsage\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x17registerCollectionUsage\x12\x1d.coinlib.LogicCollectionUsage\x1a\x16.google.protobuf.Empty\"\x00\x12:\n\x08runLogic\x12\x14.coinlib.LogicRunJob\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x0eregisterTrader\x12 .coinlib.LogicTraderRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x10registerScreener\x12\".coinlib.LogicScreenerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x11registerDataLogic\x12\x1e.coinlib.LogicDataRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x13\x61\x64\x64LogicToWorkspace\x12#.coinlib.WorkspaceLogicRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32Q\n\x06\x42roker\x12G\n\x0eregisterBroker\x12\x1b.coinlib.BrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xb2\x04\n\x0c\x42rokerWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.BrokerWorkerConfig\"\x00\x12\x46\n\x14OnBrokerErrorOccured\x12\x14.coinlib.BrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13WatchBrokerCommands\x12\".coinlib.BrokerCommandRegistration\x1a\x17.coinlib.BrokerCommands\"\x00(\x01\x30\x01\x12L\n\x11SendCommandAnswer\x12\x1d.coinlib.BrokerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x16SendCommandAnswerError\x12\".coinlib.BrokerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12U\n\x15RegisterBrokerSession\x12\".coinlib.BrokerSessionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rOnBrokerEvent\x12\x18.coinlib.BrokerEventData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa1\x08\n\tAppWorker\x12;\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x18.coinlib.AppWorkerConfig\"\x00\x12L\n\x17OnAppWorkerErrorOccured\x12\x17.coinlib.AppWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x13WatchBrokerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12\\\n\x10RunModuleCommand\x12\x1f.coinlib.AppWorkerModuleCommand\x1a%.coinlib.AppWorkerModuleCommandAnswer\"\x00\x12\\\n\x10RunBrokerCommand\x12\x1f.coinlib.AppWorkerBrokerCommand\x1a%.coinlib.AppWorkerBrokerCommandAnswer\"\x00\x12\x61\n\x16WatchAppWorkerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12O\n\x11SendCommandAnswer\x12 .coinlib.AppWorkerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x16SendCommandAnswerError\x12%.coinlib.AppWorkerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x18OnAppWorkerLogicFinished\x12#.coinlib.AppWorkerFinishedStepInfos\x1a\x16.google.protobuf.Empty\"\x00\x12g\n\x18RegisterAppWorkerSession\x12%.coinlib.AppWorkerSessionRegistration\x1a\".coinlib.AppWorkerRegistrationInfo\"\x00\x12I\n\x10OnAppWorkerEvent\x12\x1b.coinlib.AppWorkerEventData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x12OnBrokerTestResult\x12\x1f.coinlib.BrokerTestProtocolData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa2\x04\n\rFeatureWorker\x12?\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1c.coinlib.FeatureWorkerConfig\"\x00\x12\x41\n\x0eOnErrorOccured\x12\x15.coinlib.FeatureError\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\rWatchCommands\x12\x18.coinlib.FeatureCommands\x1a\x18.coinlib.FeatureCommands\"\x00(\x01\x30\x01\x12M\n\x11SendCommandAnswer\x12\x1e.coinlib.FeatureCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x16SendCommandAnswerError\x12#.coinlib.FeatureCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Z\n\x0fRegisterSession\x12#.coinlib.FeatureSessionRegistration\x1a .coinlib.RegistrationInformation\"\x00\x12>\n\x07OnEvent\x12\x19.coinlib.FeatureEventData\x1a\x16.google.protobuf.Empty\"\x00\x32]\n\x06Symbol\x12S\n\x14registerSymbolBroker\x12!.coinlib.SymbolBrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xc1\x03\n\x10\x44\x61taLoaderWorker\x12N\n\rgetAllSymbols\x12\x1e.coinlib.SymbolDataRequestInfo\x1a\x1b.coinlib.SymbolDataResponse\"\x00\x12T\n\x0fgetAllExchanges\x12 .coinlib.ExchangeDataRequestInfo\x1a\x1d.coinlib.ExchangeDataResponse\"\x00\x12J\n\rgetMarketData\x12\x1a.coinlib.MarketDataRequest\x1a\x1b.coinlib.MarketDataResponse\"\x00\x12M\n\x0egetFeatureData\x12\x1b.coinlib.FeatureDataRequest\x1a\x1c.coinlib.FeatureDataResponse\"\x00\x12l\n\x19getAdditionalDataFeatures\x12%.coinlib.AdditionalDataFeatureRequest\x1a&.coinlib.AdditionalDataFeatureResponse\"\x00\x32\x63\n\x0cNotification\x12S\n\x14registerNotification\x12!.coinlib.NotificationRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32U\n\x08\x46\x65\x61tures\x12I\n\x0fregisterFeature\x12\x1c.coinlib.FeatureRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xce\x01\n\nStatistics\x12\x65\n\x1dregisterStatisticRuleFunction\x12*.coinlib.StatisticRuleFunctionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x17registerStatisticMethod\x12$.coinlib.StatisticMethodRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xf5\x01\n\x12\x44\x61taWorkerRegistry\x12\x31\n\ngetAuthKey\x12\x0f.coinlib.ApiKey\x1a\x10.coinlib.AuthKey\"\x00\x12J\n\x16getAllDataWorkerServer\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x1bgetDataWorkerServerEndpoint\x12\x1e.coinlib.WorkerRegistryRequest\x1a\x1f.coinlib.WorkerRegistryResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61taWorker.proto\x12\x07\x63oinlib\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x19google/protobuf/any.proto\"P\n\tWorkerJob\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\"k\n\x0eWorkerJobError\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\x12\x14\n\x0c\x65rrorMessage\x18\x04 \x01(\t\"E\n\x16WorkerAvailablePlugins\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\xb7\x01\n\x06Worker\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x02 \x01(\t\x12\x13\n\x0bworker_mode\x18\x03 \x01(\t\x12\x39\n\x10\x61vailablePlugins\x18\x04 \x03(\x0b\x32\x1f.coinlib.WorkerAvailablePlugins\x12\n\n\x02os\x18\x05 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x06 \x01(\t\x12\x15\n\ractiveModules\x18\x07 \x03(\t\"\x1a\n\x07RowData\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\";\n\x15WorkerJobDataResponse\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x16\n\x14WorkerJobDataPartial\"\xfd\x01\n\x1a\x43hartWorkerPartialDataInfo\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x02\x12\x0f\n\x07opacity\x18\x05 \x01(\x02\x12\x15\n\rchartTypeIcon\x18\x06 \x01(\t\x12\x0f\n\x07tooltip\x18\x07 \x01(\x08\x12\r\n\x05\x63hart\x18\x08 \x01(\t\x12\x13\n\x0b\x63onnectGaps\x18\t \x01(\x08\x12\x11\n\tfill_from\x18\n \x01(\x02\x12\x0c\n\x04\x66ill\x18\x0b \x01(\t\x12\x12\n\nadditional\x18\x0c \x01(\t\x12\x0f\n\x07\x66ill_to\x18\r \x01(\t\"\xad\x01\n\x1d\x43hartsWorkerPartialDataLayout\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x02 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x36\n\tchartInfo\x18\x03 \x01(\x0b\x32#.coinlib.ChartWorkerPartialDataInfo\"\xdd\x01\n\x14\x43hartWorkerIndicator\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07\x66\x65\x61ture\x18\x03 \x01(\t\x12\x12\n\nsubfeature\x18\x04 \x01(\t\x12\r\n\x05short\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\x11\n\telementId\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tid_output\x18\n \x01(\t\x12\x10\n\x08\x66inished\x18\x0b \x01(\x08\x12\x0f\n\x07\x63hartId\x18\x0c \x01(\t\"\xdc\x02\n ChartWorkerIndicatorRegistration\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x11\n\tid_output\x18\x06 \x01(\t\x12\x0e\n\x06inputs\x18\x07 \x01(\x0c\x12\x0c\n\x04mode\x18\x08 \x01(\t\x12\x19\n\x11short_description\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07process\x18\x0b \x01(\t\x12\x16\n\x0eunstablePeriod\x18\x0c \x01(\x08\x12\x19\n\x11\x64ynamicTimeseries\x18\r \x01(\x08\x12\x0e\n\x06plugin\x18\x0e \x01(\t\x12\x15\n\rpluginVersion\x18\x0f \x01(\t\x12\x11\n\tcode_type\x18\x10 \x01(\t\x12\x0c\n\x04\x63ode\x18\x11 \x01(\t\"n\n!ChartWorkerIndicatorConfigElement\x12\x30\n\tindicator\x18\x01 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x17\n\x0findicatorConfig\x18\x02 \x01(\x0c\"\xac\x01\n\x12\x43hartsWorkerConfig\x12<\n\x08\x65lements\x18\x01 \x03(\x0b\x32*.coinlib.ChartWorkerIndicatorConfigElement\x12-\n\x08\x63hildren\x18\x02 \x01(\x0b\x32\x1b.coinlib.ChartsWorkerConfig\x12)\n\tchartData\x18\x03 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\"-\n\x0eStatisticInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"A\n\tDataError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x11\n\terrorCode\x18\x02 \x01(\x03\x12\x10\n\x08\x63ritical\x18\x03 \x01(\x08\"\x89\x01\n\x0eIndicatorError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x03 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\"\xa3\x01\n\x1aStatisticRuleFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa5\x01\n\x1cStatisticMethodFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xb2\x01\n\"StatisticsMethodWorkerWindowConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\x10\n\x08windowId\x18\x03 \x01(\t\x12)\n\tchartData\x18\x04 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x05 \x01(\x0b\x32\x17.coinlib.ParameterTable\"R\n\x13ParameterTableEntry\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08required\x18\x04 \x01(\x08\"B\n\x0eParameterTable\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.coinlib.ParameterTableEntry\"z\n\rChartDataInfo\x12\x10\n\x08\x63hart_id\x18\x01 \x01(\t\x12\x14\n\x0c\x63hart_prefix\x18\x02 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\t\x12\x13\n\x0b\x61\x63tivity_id\x18\x04 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x05 \x01(\t\"\xf6\x02\n\x1aStatisticsRuleWorkerConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x05rules\x18\x02 \x03(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x19\n\x11statisticFunction\x18\x03 \x01(\t\x12?\n\x06inputs\x18\x04 \x03(\x0b\x32/.coinlib.StatisticsRuleWorkerConfig.InputsEntry\x12\x12\n\ncombinator\x18\x05 \x01(\t\x12\x16\n\x0e\x63ombinator_not\x18\x06 \x01(\x08\x12\x0c\n\x04type\x18\x07 \x01(\t\x12)\n\tchartData\x18\x08 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x1a\x46\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.coinlib.StatisticInput:\x02\x38\x01\"\xa8\x01\n\x1eStatisticsRuleWorkerConfigType\x12\x33\n\x04rule\x18\x01 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfigH\x00\x12\x43\n\x0cmethodWindow\x18\x02 \x01(\x0b\x32+.coinlib.StatisticsMethodWorkerWindowConfigH\x00\x42\x0c\n\ntest_oneof\"\xb4\x01\n\x1cStatisticsBulkedWorkerConfig\x12\x38\n\x07\x63onfigs\x18\x01 \x03(\x0b\x32\'.coinlib.StatisticsRuleWorkerConfigType\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x03 \x01(\x0b\x32\x17.coinlib.ParameterTable\"\x9f\x01\n\x16StatisticFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa7\x01\n\x1cStatisticMethodPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x12\n\ndocumentId\x18\x03 \x01(\t\x12\r\n\x05width\x18\x04 \x01(\t\x12\x0e\n\x06height\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x10\n\x08windowId\x18\x07 \x01(\t\"\xa6\x01\n\x1aStatisticRulePartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12:\n\rstatisticRule\x18\x02 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x14\n\x0c\x63ollectionid\x18\x03 \x01(\t\x12\x12\n\nresultName\x18\x05 \x01(\t\"\xa2\x01\n\x1cStatisticBulkedPartiallyData\x12;\n\nmethodData\x18\x01 \x01(\x0b\x32%.coinlib.StatisticMethodPartiallyDataH\x00\x12\x37\n\x08ruleData\x18\x02 \x01(\x0b\x32#.coinlib.StatisticRulePartiallyDataH\x00\x42\x0c\n\ntest_oneof\"m\n\x11SymbolBrokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"U\n\x19SymbolBrokerConsumerError\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\"\x95\x02\n\x16SymbolBrokerMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04open\x18\x02 \x01(\x02\x12\r\n\x05\x63lose\x18\x03 \x01(\x02\x12\x0c\n\x04high\x18\x04 \x01(\x02\x12\x0b\n\x03low\x18\x05 \x01(\x02\x12\x0e\n\x06volume\x18\x06 \x01(\x02\x12\r\n\x05trade\x18\x07 \x01(\x02\x12\x10\n\x08\x64\x61tetime\x18\x08 \x01(\t\x12\x11\n\tsymbol_id\x18\t \x01(\t\x12\x0e\n\x06symbol\x18\n \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x0b \x01(\t\x12\x12\n\nevent_time\x18\x0c \x01(\t\x12\x0f\n\x07isfinal\x18\r \x01(\x08\x12\x11\n\tcloseTime\x18\x0e \x01(\t\"\x96\x01\n\x10SymbolBrokerInfo\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\texchanges\x18\x02 \x03(\x0b\x32\x1d.coinlib.SymbolBrokerExchange\x12,\n\x07symbols\x18\x03 \x03(\x0b\x32\x1b.coinlib.SymbolBrokerSymbol\";\n\x15SymbolBrokerOrderbook\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"F\n SymbolBrokerHistoricalMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\xba\x01\n\x14SymbolBrokerExchange\x12\x0c\n\x04icon\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07website\x18\x04 \x01(\t\x12\x15\n\rsymbols_count\x18\x05 \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x06 \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\x07 \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x08 \x01(\x02\"\x8c\x04\n\x12SymbolBrokerSymbol\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x38\n\tassetType\x18\x04 \x01(\x0e\x32%.coinlib.SymbolBrokerSymbol.AssetType\x12>\n\x0c\x63ontractType\x18\x05 \x01(\x0e\x32(.coinlib.SymbolBrokerSymbol.ContractType\x12\x0c\n\x04\x62\x61se\x18\x06 \x01(\t\x12\r\n\x05quote\x18\x07 \x01(\t\x12\x1a\n\x12\x65xchange_symbol_id\x18\x08 \x01(\t\x12\x16\n\x0esize_precision\x18\t \x01(\x02\x12\x17\n\x0fprice_precision\x18\n \x01(\x02\x12\r\n\x05price\x18\x0b \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x0c \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\r \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x0e \x01(\x02\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"O\n\x1cSymbolBrokerBrokerInfoConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\"\xdd\x03\n#SymbolBrokerConsumeMarketdataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12O\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x39.coinlib.SymbolBrokerConsumeMarketdataConfig.ContractType\x12I\n\tassetType\x18\t \x01(\x0e\x32\x36.coinlib.SymbolBrokerConsumeMarketdataConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xda\x03\n\"SymbolBrokerConsumeOrderbookConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12N\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x38.coinlib.SymbolBrokerConsumeOrderbookConfig.ContractType\x12H\n\tassetType\x18\t \x01(\x0e\x32\x35.coinlib.SymbolBrokerConsumeOrderbookConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xb8\x04\n#SymbolBrokerGetHistoricalDataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\t\x12\x0b\n\x03\x65nd\x18\x08 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\t \x01(\t\x12)\n\tchartData\x18\n \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12O\n\x0c\x63ontractType\x18\x0b \x01(\x0e\x32\x39.coinlib.SymbolBrokerGetHistoricalDataConfig.ContractType\x12I\n\tassetType\x18\x0c \x01(\x0e\x32\x36.coinlib.SymbolBrokerGetHistoricalDataConfig.AssetType\x12\x12\n\nreturnData\x18\r \x01(\x08\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xc5\x02\n\x18SymbolBrokerWorkerConfig\x12;\n\ninfoConfig\x18\x01 \x01(\x0b\x32%.coinlib.SymbolBrokerBrokerInfoConfigH\x00\x12\x45\n\rconsumeConfig\x18\x02 \x01(\x0b\x32,.coinlib.SymbolBrokerConsumeMarketdataConfigH\x00\x12M\n\x16\x63onsumeOrderbookConfig\x18\x03 \x01(\x0b\x32+.coinlib.SymbolBrokerConsumeOrderbookConfigH\x00\x12H\n\x10historicalConfig\x18\x04 \x01(\x0b\x32,.coinlib.SymbolBrokerGetHistoricalDataConfigH\x00\x42\x0c\n\ntest_oneof\"F\n SymbolBrokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"2\n\x1fSymbolBrokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"j\n\x15SymbolBrokerFetchData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12-\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x1f.coinlib.SymbolBrokerMarketData\"u\n$NotificationExtractMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\t\x12\x0f\n\x07options\x18\x04 \x01(\t\"\xd3\x01\n!NotificationSendMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0e\n\x06images\x18\x04 \x01(\t\x12\x0f\n\x07\x62uttons\x18\x05 \x01(\t\x12\x0f\n\x07options\x18\x06 \x01(\t\x12\x13\n\x0b\x63\x61llback_id\x18\x07 \x01(\t\x12\x14\n\x0c\x63\x61llback_url\x18\x08 \x01(\t\x12\x10\n\x08\x63hannels\x18\t \x01(\t\"\xbd\x01\n\x18NotificationWorkerConfig\x12G\n\x11sendMessageConfig\x18\x01 \x01(\x0b\x32*.coinlib.NotificationSendMessageDataConfigH\x00\x12J\n\x11\x65xtractDataConfig\x18\x02 \x01(\x0b\x32-.coinlib.NotificationExtractMessageDataConfigH\x00\x42\x0c\n\ntest_oneof\"Z\n\x11NotificationError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"b\n\x1bNotificationCallbackExtract\x12\x11\n\tbutton_id\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x98\x01\n\x0eLogicComponent\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x18\n\x10logicComponentId\x18\x03 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\x0c\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x14\n\x0clogicDetails\x18\x07 \x01(\t\"\xde\x03\n\x12\x42rokerAccountModel\x12:\n\nbrokerType\x18\x01 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerType\x12\x34\n\x04mode\x18\x02 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerMode\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x10\n\x08makerFee\x18\x04 \x01(\x02\x12\x10\n\x08takerFee\x18\x05 \x01(\x02\x12\x39\n\x0cmakerFeeMode\x18\x06 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\x12\x39\n\x0ctakerFeeMode\x18\x07 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\"Q\n\nBrokerType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"1\n\nBrokerMode\x12\x0e\n\nBACKTRADER\x10\x00\x12\t\n\x05PAPER\x10\x01\x12\x08\n\x04LIVE\x10\x02\"$\n\x07\x46\x65\x65Mode\x12\x0e\n\nPERCENTAGE\x10\x00\x12\t\n\x05\x46IXED\x10\x01\"~\n\x0ePortfolioAsset\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x03 \x01(\x02\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\x0e\n\x06locked\x18\x05 \x01(\x02\x12\x11\n\tlastPrice\x18\x06 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x07 \x01(\t\"o\n\x13\x43\x61lculatedBaseMoney\x12\r\n\x05total\x18\x01 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x0f\n\x07summary\x18\x04 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\"\xc0\x01\n\x0ePortfolioModel\x12\'\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x17.coinlib.PortfolioAsset\x12@\n\x1a\x63urrentCalculatedBaseMoney\x18\x02 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\x43\n\x1dhistoricalCalculatedBaseMoney\x18\x03 \x03(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\"\x82\x03\n\x10LogicRunnerLogic\x12)\n\tchartData\x18\x01 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x30\n\x0flogicComponents\x18\x02 \x03(\x0b\x32\x17.coinlib.LogicComponent\x12\x11\n\tstartDate\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x04 \x01(\t\x12*\n\tportfolio\x18\x05 \x01(\x0b\x32\x17.coinlib.PortfolioModel\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\x12/\n\x0eparameterTable\x18\x07 \x01(\x0b\x32\x17.coinlib.ParameterTable\x12\x11\n\tlogicMode\x18\x08 \x01(\t\x12\x15\n\rapp_worker_id\x18\t \x01(\t\x12\x1c\n\x14\x61pp_worker_runner_id\x18\n \x01(\t\x12\x14\n\x0coptions_json\x18\x0b \x01(\t\"\xd5\x01\n\x1eLogicRunnerOfflineWorkerConfig\x12,\n\tlogicInfo\x18\x01 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12+\n\tportfolio\x18\x03 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x18\n\x10\x61\x64vancedDataInfo\x18\x04 \x01(\t\x12\x13\n\x0bonlySignals\x18\x05 \x01(\x08\"\xcf\x04\n\x15LogicRunnerStatistics\x12\x1f\n\x17highestProfitPercentage\x18\x01 \x01(\x02\x12\x1d\n\x15highestLossPercentage\x18\x02 \x01(\x02\x12\x11\n\tsinceDate\x18\x03 \x01(\t\x12\x0e\n\x06\x61tDate\x18\x04 \x01(\t\x12\x11\n\ttradesCnt\x18\x05 \x01(\x02\x12\x35\n\x0f\x63\x61lculatedMoney\x18\x06 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\"\n\x1aunrealizedProfitPercentage\x18\x07 \x01(\x02\x12\x0c\n\x04\x66\x65\x65s\x18\x08 \x01(\x02\x12 \n\x18profitCompletePercentage\x18\t \x01(\x02\x12\x1d\n\x15highestProfitPerGroup\x18\n \x01(\x02\x12\x1b\n\x13highestLossPerGroup\x18\x0b \x01(\x02\x12\x18\n\x10slippagePerGroup\x18\x0c \x01(\x02\x12\x1a\n\x12\x61verageAmountQuote\x18\r \x01(\x02\x12\'\n\x1f\x61verageProfitPercentagePergroup\x18\x0e \x01(\x02\x12\x19\n\x11portfolioTimeline\x18\x0f \x01(\t\x12\x14\n\x0cwinLossRatio\x18\x10 \x01(\x02\x12\x0e\n\x06winCnt\x18\x11 \x01(\x02\x12\x0f\n\x07lossCnt\x18\x12 \x01(\x02\x12\x17\n\x0fsecondsInMarket\x18\x13 \x01(\x02\x12\x1d\n\x15\x61verageSecondsInTrade\x18\x14 \x01(\x02\x12\x10\n\x08\x64rawDown\x18\x15 \x01(\x02\"\xa6\x01\n%LogicRunnerOfflineWorkerPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\npercentage\x18\x02 \x01(\x02\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x05 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"w\n\x1dLogicRunnerOfflineWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xb4\x01\n$LogicRunnerOfflineWorkerFinishedData\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x04 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"K\n\rWorkspaceInfo\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x11\n\tdataSetId\x18\x02 \x01(\t\x12\x12\n\nactivityId\x18\x03 \x01(\t\"@\n\x17WorkerPluginInformation\x12%\n\x06plugin\x18\x01 \x03(\x0b\x32\x15.coinlib.PluginConfig\"<\n\x0eWorkerSettings\x12\x15\n\ractiveModules\x18\x01 \x03(\t\x12\x13\n\x0bworker_mode\x18\x02 \x01(\t\"\'\n\x12WorkerRegistration\x12\x11\n\tworker_id\x18\x01 \x01(\t\"b\n\x15\x43ollectionNodeRequest\x12\x16\n\x0e\x63ollectionName\x18\x01 \x01(\t\x12\r\n\x05stage\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\":\n\x16\x43ollectionNodeResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsize_in_mb\x18\x02 \x01(\t\"`\n\x0c\x45ventRequest\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\r\n\x05stage\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"t\n\x0cPluginConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x13\n\x0b\x66ilecontent\x18\x04 \x01(\t\x12\x10\n\x08testOnly\x18\x05 \x01(\x08\x12\x10\n\x08\x66iletype\x18\x06 \x01(\t\"U\n\x18PluginInstallationOutput\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x15\n\routputMessage\x18\x02 \x01(\t\"\xcb\x01\n\x1dSimulatorChartConfigIndicator\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nsubfeature\x18\x02 \x01(\t\x12\x42\n\x06inputs\x18\x03 \x03(\x0b\x32\x32.coinlib.SimulatorChartConfigIndicator.InputsEntry\x12\x12\n\nchartIndex\x18\x04 \x01(\t\x1a-\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x14SimulatorChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62roker\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\x97\x01\n\x1dSimulatorStatisticChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\xc7\x01\n\x1eSimulatorMethodCallChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\x12-\n\x07methods\x18\x07 \x03(\x0b\x32\x1c.coinlib.SimulatorMethodCall\"@\n\x11SimulatorResponse\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"\x83\x01\n\x1cSymbolBrokerSimulatorRequest\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x13\n\x0btestSymbol1\x18\x04 \x01(\t\x12\x13\n\x0btestSymbol2\x18\x05 \x01(\t\"g\n\x1dSymbolBrokerSimulatorResponse\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"@\n\x1e\x42rokerSimulatorBrokerLoginData\x12\x0e\n\x06\x61pikey\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"\x95\x01\n\x19\x42rokerSimulatorBrokerData\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12:\n\tloginInfo\x18\x02 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x11\n\tassetType\x18\x03 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x04 \x01(\t\"\x98\x01\n\x16\x42rokerSimulatorRequest\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x36\n\nbrokerInfo\x18\x04 \x01(\x0b\x32\".coinlib.BrokerSimulatorBrokerData\x12\x11\n\tpaperMode\x18\x05 \x01(\x08\"\xb2\x01\n\x17\x42rokerSimulatorResponse\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\x12\x11\n\tsessionId\x18\x04 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x05 \x01(\t\x12\x15\n\rtargetdepotId\x18\x06 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"f\n\x1cNotificationSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0e\n\x06inputs\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x10\n\x08\x63hannels\x18\x04 \x01(\t\"c\n\x1dNotificationSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"P\n\x17\x46\x65\x61tureSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\"^\n\x18\x46\x65\x61tureSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"c\n\nLogicInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x85\x02\n\x17LogicTraderRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x84\x02\n\x16LogicAlertRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x83\x02\n\x15LogicDataRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x87\x02\n\x19LogicScreenerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x91\x02\n\x1aWorkspaceLogicRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x18\n\x10logicComponentId\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\x0c\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0e\n\x06plugin\x18\x05 \x01(\t\x12\x15\n\rpluginVersion\x18\x06 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x07 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x10\n\x08workerId\x18\x0b \x01(\t\x12\x11\n\tautostart\x18\x0c \x01(\x08\x12\x16\n\x0e\x61utostartLogic\x18\r \x01(\x08\"\"\n\x0bLogicRunJob\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\"\xb3\x02\n\x0eLogicDataUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05group\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06symbol\x18\x06 \x01(\x08\x12\x10\n\x08\x65xchange\x18\x07 \x01(\x08\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf3\x01\n\x11LogicMonitorEvent\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf6\x01\n\x14LogicCollectionUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xe2\x01\n\x0fLogicEventUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\\\n\x13SymbolBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xe4\x01\n\x18SymbolBrokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12-\n\x07options\x18\x04 \x03(\x0b\x32\x1c.coinlib.SymbolBrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\"V\n\rBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xda\x03\n\x0e\x42rokerExchange\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x34\n\tloginMode\x18\x04 \x01(\x0e\x32!.coinlib.BrokerExchange.LoginMode\x12;\n\rcontractTypes\x18\x05 \x03(\x0e\x32$.coinlib.BrokerExchange.ContractType\x12\x35\n\nassetTypes\x18\x06 \x03(\x0e\x32!.coinlib.BrokerExchange.AssetType\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0bsupportDemo\x18\x08 \x01(\x08\x12\x13\n\x0bsupportLive\x18\t \x01(\x08\x12\x1a\n\x12positionModeFuture\x18\n \x01(\t\"\x18\n\tLoginMode\x12\x0b\n\x07\x41PI_KEY\x10\x00\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\xa8\x03\n\x12\x42rokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\'\n\x07options\x18\x04 \x03(\x0b\x32\x16.coinlib.BrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12*\n\texchanges\x18\x0b \x03(\x0b\x32\x17.coinlib.BrokerExchange\x12\x45\n\x0b\x62rokerTypes\x18\x0c \x03(\x0e\x32\x30.coinlib.BrokerRegistration.SupportedBrokerTypes\"[\n\x14SupportedBrokerTypes\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"?\n\x0f\x42rokerPortfolio\x12,\n\x05\x61sset\x18\x01 \x03(\x0b\x32\x1d.coinlib.BrokerPortfolioAsset\"Z\n\x14\x42rokerPortfolioAsset\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x11\n\tlastPrice\x18\x04 \x01(\x02\"\x84\x03\n\x18\x42rokerSessionAccountInfo\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x44\n\x0c\x63ontractType\x18\x02 \x01(\x0e\x32..coinlib.BrokerSessionAccountInfo.ContractType\x12>\n\tassetType\x18\x03 \x01(\x0e\x32+.coinlib.BrokerSessionAccountInfo.AssetType\x12:\n\tloginInfo\x18\x04 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x0f\n\x07sandbox\x18\x05 \x01(\x08\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\x9b\x01\n\x1c\x42rokerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\"\xf4\x01\n\x14\x42rokerInfoTestConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\"g\n\x12\x42rokerWorkerConfig\x12\x43\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"@\n\x1a\x42rokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\",\n\x19\x42rokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"\x18\n\x16\x42rokerStartSessionInfo\"g\n\x0b\x42rokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"j\n\x0e\x42rokerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x15\n\rbrokerCommand\x18\x03 \x01(\t\x12\x1b\n\x13\x62rokerCommandParams\x18\x04 \x01(\t\".\n\x19\x42rokerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"P\n\x14\x42rokerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"d\n\x19\x42rokerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"e\n\x0f\x42rokerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\".\n\x19\x42rokerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"J\n\x16\x42rokerTestProtocolData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\x9c\x01\n\x0f\x41ppWorkerConfig\x12\x46\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32(.coinlib.AppWorkerInfoStartSessionConfigH\x00\x12\x33\n\ntestConfig\x18\x02 \x01(\x0b\x32\x1d.coinlib.BrokerInfoTestConfigH\x00\x42\x0c\n\ntest_oneof\"\xa9\x02\n\x1f\x41ppWorkerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x02 \x01(\t\x12,\n\tlogicInfo\x18\x03 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12;\n\x0c\x62rokerConfig\x18\x04 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfig\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x10\n\x08\x63odeType\x18\x07 \x01(\t\x12\x0e\n\x06\x63odeId\x18\x08 \x01(\t\x12\x13\n\x0b\x63odeVersion\x18\t \x01(\t\"1\n\x1c\x41ppWorkerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"W\n\x0e\x41ppWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"q\n\x11\x41ppWorkerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\x12\x0e\n\x06target\x18\x05 \x01(\t\"U\n\x1c\x41ppWorkerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"S\n\x17\x41ppWorkerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"g\n\x1c\x41ppWorkerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"h\n\x12\x41ppWorkerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x83\x01\n\x16\x41ppWorkerBrokerCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x0e\n\x06params\x18\x04 \x01(\t\x12\x11\n\tcommandId\x18\x05 \x01(\t\"\x9f\x01\n\x1c\x41ppWorkerBrokerCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tcommandId\x18\x03 \x01(\t\x12\x10\n\x08response\x18\x04 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12\r\n\x05\x65rror\x18\x06 \x01(\x08\"\x93\x01\n\x16\x41ppWorkerModuleCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\"\xd0\x01\n\x1c\x41ppWorkerModuleCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x07 \x01(\t\x12\r\n\x05\x65rror\x18\x08 \x01(\x08\x12\x10\n\x08response\x18\t \x01(\t\"g\n\x1a\x41ppWorkerFinishedStepInfos\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\"c\n\x19\x41ppWorkerRegistrationInfo\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07success\x18\x03 \x01(\x08\"\xad\x02\n\x1d\x46\x65\x61tureInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x14\n\x0coptionValues\x18\x03 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12\x1c\n\x14targetDatabaseServer\x18\x05 \x01(\t\x12\x18\n\x10targetDatabaseID\x18\x06 \x01(\t\x12\x13\n\x0bsessionData\x18\x07 \x01(\t\x12\x14\n\x0crabbitServer\x18\x08 \x01(\t\x12\x12\n\nrabbitUser\x18\t \x01(\t\x12\x11\n\trabbitPwd\x18\n \x01(\t\x12\x12\n\nrabbitPort\x18\x0b \x01(\t\x12\x19\n\x11rabbitQueuePrefix\x18\x0c \x01(\t\"i\n\x13\x46\x65\x61tureWorkerConfig\x12\x44\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32&.coinlib.FeatureInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"U\n\x0c\x46\x65\x61tureError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"_\n\x0f\x46\x65\x61tureCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\"Q\n\x15\x46\x65\x61tureCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"e\n\x1a\x46\x65\x61tureCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"/\n\x1a\x46\x65\x61tureSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"f\n\x10\x46\x65\x61tureEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\">\n\x17RegistrationInformation\x12\x12\n\nduplicated\x18\x01 \x01(\x08\x12\x0f\n\x07success\x18\x02 \x01(\x08\"I\n\x15SymbolDataRequestInfo\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x02 \x01(\t\"G\n\x12SymbolDataResponse\x12\x31\n\x07symbols\x18\x01 \x03(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\"\x19\n\x17\x45xchangeDataRequestInfo\"L\n\x13\x42rokerExchangeSmall\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04mode\x18\x04 \x01(\t\"G\n\x14\x45xchangeDataResponse\x12/\n\texchanges\x18\x02 \x03(\x0b\x32\x1c.coinlib.BrokerExchangeSmall\"\xae\x02\n\x17SymbolBrokerSymbolSmall\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x11\n\tsymbol_id\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\t\x12\x0c\n\x04\x62\x61se\x18\x05 \x01(\t\x12\r\n\x05quote\x18\x06 \x01(\t\x12\x16\n\x0epricePrecision\x18\x07 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12>\n\x07\x63olumns\x18\n \x03(\x0b\x32-.coinlib.SymbolBrokerSymbolSmall.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb2\x01\n\x11MarketDataRequest\x12\x30\n\x06symbol\x18\x01 \x01(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x05 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x06 \x01(\t\"h\n\x12MarketDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"i\n\x13\x46\x65\x61tureDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"\xa0\x01\n\x12\x46\x65\x61tureDataRequest\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x01 \x03(\t\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x15\n\rtarget_symbol\x18\x04 \x01(\t\x12\x17\n\x0ftarget_exchange\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05stage\x18\x07 \x01(\t\"\x1e\n\x1c\x41\x64\x64itionalDataFeatureRequest\"y\n\x19\x41\x64\x64itionalDataFeatureInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"Y\n\x1d\x41\x64\x64itionalDataFeatureResponse\x12\x38\n\x0c\x66\x65\x61tureInfos\x18\x01 \x03(\x0b\x32\".coinlib.AdditionalDataFeatureInfo\"\\\n\x13NotificationOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\x8f\x02\n\x18NotificationRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.coinlib.NotificationOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12\x15\n\risInteractive\x18\x0c \x01(\x08\"W\n\x0e\x46\x65\x61tureOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xc2\x02\n\x13\x46\x65\x61tureRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12(\n\x07options\x18\x04 \x03(\x0b\x32\x17.coinlib.FeatureOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\x15\n\rfeature_infos\x18\r \x01(\t\x12\x1d\n\x15\x65stimatedDataInterval\x18\x0e \x01(\x03\x12\r\n\x05group\x18\x0f \x01(\t\"5\n\x13SimulatorMethodCall\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\"`\n\x17StatisticFunctionInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"n\n\x15StatisticMethodInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x9d\x02\n\x1bStatisticMethodRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\trefreshOn\x18\x03 \x03(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x1c\n\x14targetPositionLayout\x18\x07 \x01(\t\x12.\n\x06inputs\x18\x08 \x03(\x0b\x32\x1e.coinlib.StatisticMethodInputs\x12\x0e\n\x06plugin\x18\t \x01(\t\x12\x15\n\rpluginVersion\x18\n \x01(\t\x12\x11\n\tcode_type\x18\x0b \x01(\t\x12\x0c\n\x04\x63ode\x18\x0c \x01(\t\"\x83\x02\n!StatisticRuleFunctionRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x30\n\x06inputs\x18\x07 \x03(\x0b\x32 .coinlib.StatisticFunctionInputs\x12\x0e\n\x06plugin\x18\x08 \x01(\t\x12\x15\n\rpluginVersion\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\"A\n\x15WorkerRegistryRequest\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x15\n\ractiveModules\x18\x02 \x03(\t\"D\n\x16WorkerRegistryResponse\x12\x16\n\x0etargetendpoint\x18\x01 \x01(\t\x12\x12\n\ntargetport\x18\x02 \x01(\t\"-\n\x06\x41piKey\x12\x12\n\napi_key_id\x18\x01 \x01(\t\x12\x0f\n\x07modules\x18\x02 \x01(\t\"0\n\x07\x41uthKey\x12\x10\n\x08\x61uth_key\x18\x01 \x01(\t\x12\x13\n\x0bvalid_until\x18\x02 \x01(\t2\xf6\x01\n\x0c\x43hartsWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.ChartsWorkerConfig\"\x00\x12L\n\x17OnIndicatorErrorOccured\x12\x17.coinlib.IndicatorError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnPartialChartLayout\x12&.coinlib.ChartsWorkerPartialDataLayout\x1a\x16.google.protobuf.Empty\"\x00\x32\x9d\x02\n\x16StatisticsMethodWorker\x12H\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a%.coinlib.StatisticsBulkedWorkerConfig\"\x00\x12[\n\x18OnStatisticPartiallyData\x12%.coinlib.StatisticBulkedPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x1fOnStatisticFunctionErrorOccured\x12\x1f.coinlib.StatisticFunctionError\x1a\x16.google.protobuf.Empty\"\x00\x32\xae\x06\n\x12SymbolBrokerWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.SymbolBrokerWorkerConfig\"\x00\x12l\n\x0fwaitForCommands\x12).coinlib.SymbolBrokerStopConsumerListener\x1a(.coinlib.SymbolBrokerStopConsumerCommand\"\x00(\x01\x30\x01\x12[\n\x1fonBrokerFetchSymbolDataReceived\x12\x1e.coinlib.SymbolBrokerFetchData\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x18onHistoricalDataReceived\x12).coinlib.SymbolBrokerHistoricalMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x1aonBrokerSymbolInfoReceived\x12\x19.coinlib.SymbolBrokerInfo\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x14onMarketDataReceived\x12\x1f.coinlib.SymbolBrokerMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x13onOrderbookReceived\x12\x1e.coinlib.SymbolBrokerOrderbook\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnSymbolBrokerErrorOccured\x12\x1a.coinlib.SymbolBrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12[\n\x1bonBrokerSymbolTickerCrashed\x12\".coinlib.SymbolBrokerConsumerError\x1a\x16.google.protobuf.Empty\"\x00\x32\x89\x02\n\x12NotificationWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.NotificationWorkerConfig\"\x00\x12Y\n\x17OnCallbackDataExtracted\x12$.coinlib.NotificationCallbackExtract\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnNotificationErrorOccured\x12\x1a.coinlib.NotificationError\x1a\x16.google.protobuf.Empty\"\x00\x32\xea\x03\n\x19LogicRunnerOfflineService\x12J\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12_\n\x1aGetLogicConfigForWorkspace\x12\x16.coinlib.WorkspaceInfo\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12\x61\n\x15OnRunnerPartiallyData\x12..coinlib.LogicRunnerOfflineWorkerPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnRunnerErrorOccured\x12&.coinlib.LogicRunnerOfflineWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x18OnRunnerFinishedComplete\x12-.coinlib.LogicRunnerOfflineWorkerFinishedData\x1a\x16.google.protobuf.Empty\"\x00\x32\xcd\x05\n\nDataWorker\x12?\n\x0f\x41\x63\x63\x65ptWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x10\x44\x65\x63lineWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\tFireEvent\x12\x15.coinlib.EventRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x14GetNodeForCollection\x12\x1e.coinlib.CollectionNodeRequest\x1a\x1f.coinlib.CollectionNodeResponse\"\x00\x12<\n\x0eRegisterWorker\x12\x0f.coinlib.Worker\x1a\x17.coinlib.WorkerSettings\"\x00\x12\x44\n\rGetAllPlugins\x12\x0f.coinlib.Worker\x1a .coinlib.WorkerPluginInformation\"\x00\x12K\n\x0fUpdateWorkerJob\x12\x1e.coinlib.WorkerJobDataResponse\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0fWatchWorkerJobs\x12\x1b.coinlib.WorkerRegistration\x1a\x12.coinlib.WorkerJob\"\x00(\x01\x30\x01\x12\x41\n\x11\x46inishedWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x10\x45rroredWorkerJob\x12\x17.coinlib.WorkerJobError\x1a\x16.google.protobuf.Empty\"\x00\x32\x9f\x01\n\x0cPluginWorker\x12\x38\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x15.coinlib.PluginConfig\"\x00\x12U\n\x14OnInstallationOutput\x12!.coinlib.PluginInstallationOutput\x1a\x16.google.protobuf.Empty\"\x00(\x01\x32\x9f\x05\n\tSimulator\x12X\n\x0fsimulateFeature\x12 .coinlib.FeatureSimulatorRequest\x1a!.coinlib.FeatureSimulatorResponse\"\x00\x12L\n\rsimulateChart\x12\x1d.coinlib.SimulatorChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12^\n\x16simulateStatisticsRule\x12&.coinlib.SimulatorStatisticChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12\x61\n\x18simulateStatisticsMethod\x12\'.coinlib.SimulatorMethodCallChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12g\n\x14simulateSymbolBroker\x12%.coinlib.SymbolBrokerSimulatorRequest\x1a&.coinlib.SymbolBrokerSimulatorResponse\"\x00\x12U\n\x0esimulateBroker\x12\x1f.coinlib.BrokerSimulatorRequest\x1a .coinlib.BrokerSimulatorResponse\"\x00\x12g\n\x14simulateNotification\x12%.coinlib.NotificationSimulatorRequest\x1a&.coinlib.NotificationSimulatorResponse\"\x00\x32m\n\tFunctions\x12`\n\x19registerIndicatorFunction\x12).coinlib.ChartWorkerIndicatorRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xbc\x05\n\x05Logic\x12\x46\n\x11registerDataUsage\x12\x17.coinlib.LogicDataUsage\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x14registerMonitorEvent\x12\x1a.coinlib.LogicMonitorEvent\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x12registerEventUsage\x12\x18.coinlib.LogicEventUsage\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x17registerCollectionUsage\x12\x1d.coinlib.LogicCollectionUsage\x1a\x16.google.protobuf.Empty\"\x00\x12:\n\x08runLogic\x12\x14.coinlib.LogicRunJob\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x0eregisterTrader\x12 .coinlib.LogicTraderRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x10registerScreener\x12\".coinlib.LogicScreenerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x11registerDataLogic\x12\x1e.coinlib.LogicDataRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x13\x61\x64\x64LogicToWorkspace\x12#.coinlib.WorkspaceLogicRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32Q\n\x06\x42roker\x12G\n\x0eregisterBroker\x12\x1b.coinlib.BrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xb2\x04\n\x0c\x42rokerWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.BrokerWorkerConfig\"\x00\x12\x46\n\x14OnBrokerErrorOccured\x12\x14.coinlib.BrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13WatchBrokerCommands\x12\".coinlib.BrokerCommandRegistration\x1a\x17.coinlib.BrokerCommands\"\x00(\x01\x30\x01\x12L\n\x11SendCommandAnswer\x12\x1d.coinlib.BrokerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x16SendCommandAnswerError\x12\".coinlib.BrokerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12U\n\x15RegisterBrokerSession\x12\".coinlib.BrokerSessionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rOnBrokerEvent\x12\x18.coinlib.BrokerEventData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa1\x08\n\tAppWorker\x12;\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x18.coinlib.AppWorkerConfig\"\x00\x12L\n\x17OnAppWorkerErrorOccured\x12\x17.coinlib.AppWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x13WatchBrokerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12\\\n\x10RunModuleCommand\x12\x1f.coinlib.AppWorkerModuleCommand\x1a%.coinlib.AppWorkerModuleCommandAnswer\"\x00\x12\\\n\x10RunBrokerCommand\x12\x1f.coinlib.AppWorkerBrokerCommand\x1a%.coinlib.AppWorkerBrokerCommandAnswer\"\x00\x12\x61\n\x16WatchAppWorkerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12O\n\x11SendCommandAnswer\x12 .coinlib.AppWorkerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x16SendCommandAnswerError\x12%.coinlib.AppWorkerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x18OnAppWorkerLogicFinished\x12#.coinlib.AppWorkerFinishedStepInfos\x1a\x16.google.protobuf.Empty\"\x00\x12g\n\x18RegisterAppWorkerSession\x12%.coinlib.AppWorkerSessionRegistration\x1a\".coinlib.AppWorkerRegistrationInfo\"\x00\x12I\n\x10OnAppWorkerEvent\x12\x1b.coinlib.AppWorkerEventData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x12OnBrokerTestResult\x12\x1f.coinlib.BrokerTestProtocolData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa2\x04\n\rFeatureWorker\x12?\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1c.coinlib.FeatureWorkerConfig\"\x00\x12\x41\n\x0eOnErrorOccured\x12\x15.coinlib.FeatureError\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\rWatchCommands\x12\x18.coinlib.FeatureCommands\x1a\x18.coinlib.FeatureCommands\"\x00(\x01\x30\x01\x12M\n\x11SendCommandAnswer\x12\x1e.coinlib.FeatureCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x16SendCommandAnswerError\x12#.coinlib.FeatureCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Z\n\x0fRegisterSession\x12#.coinlib.FeatureSessionRegistration\x1a .coinlib.RegistrationInformation\"\x00\x12>\n\x07OnEvent\x12\x19.coinlib.FeatureEventData\x1a\x16.google.protobuf.Empty\"\x00\x32]\n\x06Symbol\x12S\n\x14registerSymbolBroker\x12!.coinlib.SymbolBrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xc1\x03\n\x10\x44\x61taLoaderWorker\x12N\n\rgetAllSymbols\x12\x1e.coinlib.SymbolDataRequestInfo\x1a\x1b.coinlib.SymbolDataResponse\"\x00\x12T\n\x0fgetAllExchanges\x12 .coinlib.ExchangeDataRequestInfo\x1a\x1d.coinlib.ExchangeDataResponse\"\x00\x12J\n\rgetMarketData\x12\x1a.coinlib.MarketDataRequest\x1a\x1b.coinlib.MarketDataResponse\"\x00\x12M\n\x0egetFeatureData\x12\x1b.coinlib.FeatureDataRequest\x1a\x1c.coinlib.FeatureDataResponse\"\x00\x12l\n\x19getAdditionalDataFeatures\x12%.coinlib.AdditionalDataFeatureRequest\x1a&.coinlib.AdditionalDataFeatureResponse\"\x00\x32\x63\n\x0cNotification\x12S\n\x14registerNotification\x12!.coinlib.NotificationRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32U\n\x08\x46\x65\x61tures\x12I\n\x0fregisterFeature\x12\x1c.coinlib.FeatureRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xce\x01\n\nStatistics\x12\x65\n\x1dregisterStatisticRuleFunction\x12*.coinlib.StatisticRuleFunctionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x17registerStatisticMethod\x12$.coinlib.StatisticMethodRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xf5\x01\n\x12\x44\x61taWorkerRegistry\x12\x31\n\ngetAuthKey\x12\x0f.coinlib.ApiKey\x1a\x10.coinlib.AuthKey\"\x00\x12J\n\x16getAllDataWorkerServer\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x1bgetDataWorkerServerEndpoint\x12\x1e.coinlib.WorkerRegistryRequest\x1a\x1f.coinlib.WorkerRegistryResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dataWorker_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _STATISTICSRULEWORKERCONFIG_INPUTSENTRY._options = None
@@ -40,409 +40,409 @@
   _ROWDATA._serialized_start=563
   _ROWDATA._serialized_end=589
   _WORKERJOBDATARESPONSE._serialized_start=591
   _WORKERJOBDATARESPONSE._serialized_end=650
   _WORKERJOBDATAPARTIAL._serialized_start=652
   _WORKERJOBDATAPARTIAL._serialized_end=674
   _CHARTWORKERPARTIALDATAINFO._serialized_start=677
-  _CHARTWORKERPARTIALDATAINFO._serialized_end=913
-  _CHARTSWORKERPARTIALDATALAYOUT._serialized_start=916
-  _CHARTSWORKERPARTIALDATALAYOUT._serialized_end=1089
-  _CHARTWORKERINDICATOR._serialized_start=1092
-  _CHARTWORKERINDICATOR._serialized_end=1313
-  _CHARTWORKERINDICATORREGISTRATION._serialized_start=1316
-  _CHARTWORKERINDICATORREGISTRATION._serialized_end=1664
-  _CHARTWORKERINDICATORCONFIGELEMENT._serialized_start=1666
-  _CHARTWORKERINDICATORCONFIGELEMENT._serialized_end=1776
-  _CHARTSWORKERCONFIG._serialized_start=1779
-  _CHARTSWORKERCONFIG._serialized_end=1951
-  _STATISTICINPUT._serialized_start=1953
-  _STATISTICINPUT._serialized_end=1998
-  _DATAERROR._serialized_start=2000
-  _DATAERROR._serialized_end=2065
-  _INDICATORERROR._serialized_start=2068
-  _INDICATORERROR._serialized_end=2205
-  _STATISTICRULEFUNCTIONERROR._serialized_start=2208
-  _STATISTICRULEFUNCTIONERROR._serialized_end=2371
-  _STATISTICMETHODFUNCTIONERROR._serialized_start=2374
-  _STATISTICMETHODFUNCTIONERROR._serialized_end=2539
-  _STATISTICSMETHODWORKERWINDOWCONFIG._serialized_start=2542
-  _STATISTICSMETHODWORKERWINDOWCONFIG._serialized_end=2720
-  _PARAMETERTABLEENTRY._serialized_start=2722
-  _PARAMETERTABLEENTRY._serialized_end=2804
-  _PARAMETERTABLE._serialized_start=2806
-  _PARAMETERTABLE._serialized_end=2872
-  _CHARTDATAINFO._serialized_start=2874
-  _CHARTDATAINFO._serialized_end=2996
-  _STATISTICSRULEWORKERCONFIG._serialized_start=2999
-  _STATISTICSRULEWORKERCONFIG._serialized_end=3373
-  _STATISTICSRULEWORKERCONFIG_INPUTSENTRY._serialized_start=3303
-  _STATISTICSRULEWORKERCONFIG_INPUTSENTRY._serialized_end=3373
-  _STATISTICSRULEWORKERCONFIGTYPE._serialized_start=3376
-  _STATISTICSRULEWORKERCONFIGTYPE._serialized_end=3544
-  _STATISTICSBULKEDWORKERCONFIG._serialized_start=3547
-  _STATISTICSBULKEDWORKERCONFIG._serialized_end=3727
-  _STATISTICFUNCTIONERROR._serialized_start=3730
-  _STATISTICFUNCTIONERROR._serialized_end=3889
-  _STATISTICMETHODPARTIALLYDATA._serialized_start=3892
-  _STATISTICMETHODPARTIALLYDATA._serialized_end=4059
-  _STATISTICRULEPARTIALLYDATA._serialized_start=4062
-  _STATISTICRULEPARTIALLYDATA._serialized_end=4228
-  _STATISTICBULKEDPARTIALLYDATA._serialized_start=4231
-  _STATISTICBULKEDPARTIALLYDATA._serialized_end=4393
-  _SYMBOLBROKERERROR._serialized_start=4395
-  _SYMBOLBROKERERROR._serialized_end=4504
-  _SYMBOLBROKERCONSUMERERROR._serialized_start=4506
-  _SYMBOLBROKERCONSUMERERROR._serialized_end=4591
-  _SYMBOLBROKERMARKETDATA._serialized_start=4594
-  _SYMBOLBROKERMARKETDATA._serialized_end=4871
-  _SYMBOLBROKERINFO._serialized_start=4874
-  _SYMBOLBROKERINFO._serialized_end=5024
-  _SYMBOLBROKERORDERBOOK._serialized_start=5026
-  _SYMBOLBROKERORDERBOOK._serialized_end=5085
-  _SYMBOLBROKERHISTORICALMARKETDATA._serialized_start=5087
-  _SYMBOLBROKERHISTORICALMARKETDATA._serialized_end=5157
-  _SYMBOLBROKEREXCHANGE._serialized_start=5160
-  _SYMBOLBROKEREXCHANGE._serialized_end=5346
-  _SYMBOLBROKERSYMBOL._serialized_start=5349
-  _SYMBOLBROKERSYMBOL._serialized_end=5873
-  _SYMBOLBROKERSYMBOL_ASSETTYPE._serialized_start=5745
-  _SYMBOLBROKERSYMBOL_ASSETTYPE._serialized_end=5788
-  _SYMBOLBROKERSYMBOL_CONTRACTTYPE._serialized_start=5790
-  _SYMBOLBROKERSYMBOL_CONTRACTTYPE._serialized_end=5873
-  _SYMBOLBROKERBROKERINFOCONFIG._serialized_start=5875
-  _SYMBOLBROKERBROKERINFOCONFIG._serialized_end=5954
-  _SYMBOLBROKERCONSUMEMARKETDATACONFIG._serialized_start=5957
-  _SYMBOLBROKERCONSUMEMARKETDATACONFIG._serialized_end=6434
-  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_ASSETTYPE._serialized_start=5745
-  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_ASSETTYPE._serialized_end=5788
-  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_CONTRACTTYPE._serialized_start=5790
-  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_CONTRACTTYPE._serialized_end=5873
-  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG._serialized_start=6437
-  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG._serialized_end=6911
-  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_ASSETTYPE._serialized_start=5745
-  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_ASSETTYPE._serialized_end=5788
-  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_CONTRACTTYPE._serialized_start=5790
-  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_CONTRACTTYPE._serialized_end=5873
-  _SYMBOLBROKERGETHISTORICALDATACONFIG._serialized_start=6914
-  _SYMBOLBROKERGETHISTORICALDATACONFIG._serialized_end=7482
-  _SYMBOLBROKERGETHISTORICALDATACONFIG_ASSETTYPE._serialized_start=5745
-  _SYMBOLBROKERGETHISTORICALDATACONFIG_ASSETTYPE._serialized_end=5788
-  _SYMBOLBROKERGETHISTORICALDATACONFIG_CONTRACTTYPE._serialized_start=5790
-  _SYMBOLBROKERGETHISTORICALDATACONFIG_CONTRACTTYPE._serialized_end=5873
-  _SYMBOLBROKERWORKERCONFIG._serialized_start=7485
-  _SYMBOLBROKERWORKERCONFIG._serialized_end=7810
-  _SYMBOLBROKERSTOPCONSUMERLISTENER._serialized_start=7812
-  _SYMBOLBROKERSTOPCONSUMERLISTENER._serialized_end=7882
-  _SYMBOLBROKERSTOPCONSUMERCOMMAND._serialized_start=7884
-  _SYMBOLBROKERSTOPCONSUMERCOMMAND._serialized_end=7934
-  _SYMBOLBROKERFETCHDATA._serialized_start=7936
-  _SYMBOLBROKERFETCHDATA._serialized_end=8042
-  _NOTIFICATIONEXTRACTMESSAGEDATACONFIG._serialized_start=8044
-  _NOTIFICATIONEXTRACTMESSAGEDATACONFIG._serialized_end=8161
-  _NOTIFICATIONSENDMESSAGEDATACONFIG._serialized_start=8164
-  _NOTIFICATIONSENDMESSAGEDATACONFIG._serialized_end=8375
-  _NOTIFICATIONWORKERCONFIG._serialized_start=8378
-  _NOTIFICATIONWORKERCONFIG._serialized_end=8567
-  _NOTIFICATIONERROR._serialized_start=8569
-  _NOTIFICATIONERROR._serialized_end=8659
-  _NOTIFICATIONCALLBACKEXTRACT._serialized_start=8661
-  _NOTIFICATIONCALLBACKEXTRACT._serialized_end=8759
-  _LOGICCOMPONENT._serialized_start=8762
-  _LOGICCOMPONENT._serialized_end=8914
-  _BROKERACCOUNTMODEL._serialized_start=8917
-  _BROKERACCOUNTMODEL._serialized_end=9395
-  _BROKERACCOUNTMODEL_BROKERTYPE._serialized_start=9225
-  _BROKERACCOUNTMODEL_BROKERTYPE._serialized_end=9306
-  _BROKERACCOUNTMODEL_BROKERMODE._serialized_start=9308
-  _BROKERACCOUNTMODEL_BROKERMODE._serialized_end=9357
-  _BROKERACCOUNTMODEL_FEEMODE._serialized_start=9359
-  _BROKERACCOUNTMODEL_FEEMODE._serialized_end=9395
-  _PORTFOLIOASSET._serialized_start=9397
-  _PORTFOLIOASSET._serialized_end=9523
-  _CALCULATEDBASEMONEY._serialized_start=9525
-  _CALCULATEDBASEMONEY._serialized_end=9636
-  _PORTFOLIOMODEL._serialized_start=9639
-  _PORTFOLIOMODEL._serialized_end=9831
-  _LOGICRUNNERLOGIC._serialized_start=9834
-  _LOGICRUNNERLOGIC._serialized_end=10220
-  _LOGICRUNNEROFFLINEWORKERCONFIG._serialized_start=10223
-  _LOGICRUNNEROFFLINEWORKERCONFIG._serialized_end=10436
-  _LOGICRUNNERSTATISTICS._serialized_start=10439
-  _LOGICRUNNERSTATISTICS._serialized_end=11030
-  _LOGICRUNNEROFFLINEWORKERPARTIALLYDATA._serialized_start=11033
-  _LOGICRUNNEROFFLINEWORKERPARTIALLYDATA._serialized_end=11199
-  _LOGICRUNNEROFFLINEWORKERERROR._serialized_start=11201
-  _LOGICRUNNEROFFLINEWORKERERROR._serialized_end=11320
-  _LOGICRUNNEROFFLINEWORKERFINISHEDDATA._serialized_start=11323
-  _LOGICRUNNEROFFLINEWORKERFINISHEDDATA._serialized_end=11503
-  _WORKSPACEINFO._serialized_start=11505
-  _WORKSPACEINFO._serialized_end=11580
-  _WORKERPLUGININFORMATION._serialized_start=11582
-  _WORKERPLUGININFORMATION._serialized_end=11646
-  _WORKERSETTINGS._serialized_start=11648
-  _WORKERSETTINGS._serialized_end=11708
-  _WORKERREGISTRATION._serialized_start=11710
-  _WORKERREGISTRATION._serialized_end=11749
-  _COLLECTIONNODEREQUEST._serialized_start=11751
-  _COLLECTIONNODEREQUEST._serialized_end=11849
-  _COLLECTIONNODERESPONSE._serialized_start=11851
-  _COLLECTIONNODERESPONSE._serialized_end=11909
-  _EVENTREQUEST._serialized_start=11911
-  _EVENTREQUEST._serialized_end=12007
-  _PLUGINCONFIG._serialized_start=12009
-  _PLUGINCONFIG._serialized_end=12125
-  _PLUGININSTALLATIONOUTPUT._serialized_start=12127
-  _PLUGININSTALLATIONOUTPUT._serialized_end=12212
-  _SIMULATORCHARTCONFIGINDICATOR._serialized_start=12215
-  _SIMULATORCHARTCONFIGINDICATOR._serialized_end=12418
-  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_start=12373
-  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_end=12418
-  _SIMULATORCHARTCONFIG._serialized_start=12421
-  _SIMULATORCHARTCONFIG._serialized_end=12591
-  _SIMULATORSTATISTICCHARTCONFIG._serialized_start=12594
-  _SIMULATORSTATISTICCHARTCONFIG._serialized_end=12745
-  _SIMULATORMETHODCALLCHARTCONFIG._serialized_start=12748
-  _SIMULATORMETHODCALLCHARTCONFIG._serialized_end=12947
-  _SIMULATORRESPONSE._serialized_start=12949
-  _SIMULATORRESPONSE._serialized_end=13013
-  _SYMBOLBROKERSIMULATORREQUEST._serialized_start=13016
-  _SYMBOLBROKERSIMULATORREQUEST._serialized_end=13147
-  _SYMBOLBROKERSIMULATORRESPONSE._serialized_start=13149
-  _SYMBOLBROKERSIMULATORRESPONSE._serialized_end=13252
-  _BROKERSIMULATORBROKERLOGINDATA._serialized_start=13254
-  _BROKERSIMULATORBROKERLOGINDATA._serialized_end=13318
-  _BROKERSIMULATORBROKERDATA._serialized_start=13321
-  _BROKERSIMULATORBROKERDATA._serialized_end=13470
-  _BROKERSIMULATORREQUEST._serialized_start=13473
-  _BROKERSIMULATORREQUEST._serialized_end=13625
-  _BROKERSIMULATORRESPONSE._serialized_start=13628
-  _BROKERSIMULATORRESPONSE._serialized_end=13806
-  _NOTIFICATIONSIMULATORREQUEST._serialized_start=13808
-  _NOTIFICATIONSIMULATORREQUEST._serialized_end=13910
-  _NOTIFICATIONSIMULATORRESPONSE._serialized_start=13912
-  _NOTIFICATIONSIMULATORRESPONSE._serialized_end=14011
-  _FEATURESIMULATORREQUEST._serialized_start=14013
-  _FEATURESIMULATORREQUEST._serialized_end=14093
-  _FEATURESIMULATORRESPONSE._serialized_start=14095
-  _FEATURESIMULATORRESPONSE._serialized_end=14189
-  _LOGICINPUT._serialized_start=14191
-  _LOGICINPUT._serialized_end=14290
-  _LOGICTRADERREGISTRATION._serialized_start=14293
-  _LOGICTRADERREGISTRATION._serialized_end=14554
-  _LOGICALERTREGISTRATION._serialized_start=14557
-  _LOGICALERTREGISTRATION._serialized_end=14817
-  _LOGICDATAREGISTRATION._serialized_start=14820
-  _LOGICDATAREGISTRATION._serialized_end=15079
-  _LOGICSCREENERREGISTRATION._serialized_start=15082
-  _LOGICSCREENERREGISTRATION._serialized_end=15345
-  _WORKSPACELOGICREGISTRATION._serialized_start=15348
-  _WORKSPACELOGICREGISTRATION._serialized_end=15621
-  _LOGICRUNJOB._serialized_start=15623
-  _LOGICRUNJOB._serialized_end=15657
-  _LOGICDATAUSAGE._serialized_start=15660
-  _LOGICDATAUSAGE._serialized_end=15967
-  _LOGICMONITOREVENT._serialized_start=15970
-  _LOGICMONITOREVENT._serialized_end=16213
-  _LOGICCOLLECTIONUSAGE._serialized_start=16216
-  _LOGICCOLLECTIONUSAGE._serialized_end=16462
-  _LOGICEVENTUSAGE._serialized_start=16465
-  _LOGICEVENTUSAGE._serialized_end=16691
-  _SYMBOLBROKEROPTIONS._serialized_start=16693
-  _SYMBOLBROKEROPTIONS._serialized_end=16785
-  _SYMBOLBROKERREGISTRATION._serialized_start=16788
-  _SYMBOLBROKERREGISTRATION._serialized_end=17016
-  _BROKEROPTIONS._serialized_start=17018
-  _BROKEROPTIONS._serialized_end=17104
-  _BROKEREXCHANGE._serialized_start=17107
-  _BROKEREXCHANGE._serialized_end=17581
-  _BROKEREXCHANGE_LOGINMODE._serialized_start=17427
-  _BROKEREXCHANGE_LOGINMODE._serialized_end=17451
-  _BROKEREXCHANGE_CONTRACTTYPE._serialized_start=5790
-  _BROKEREXCHANGE_CONTRACTTYPE._serialized_end=5873
-  _BROKEREXCHANGE_ASSETTYPE._serialized_start=5745
-  _BROKEREXCHANGE_ASSETTYPE._serialized_end=5788
-  _BROKERREGISTRATION._serialized_start=17584
-  _BROKERREGISTRATION._serialized_end=18008
-  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_start=17917
-  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_end=18008
-  _BROKERPORTFOLIO._serialized_start=18010
-  _BROKERPORTFOLIO._serialized_end=18073
-  _BROKERPORTFOLIOASSET._serialized_start=18075
-  _BROKERPORTFOLIOASSET._serialized_end=18165
-  _BROKERSESSIONACCOUNTINFO._serialized_start=18168
-  _BROKERSESSIONACCOUNTINFO._serialized_end=18556
-  _BROKERSESSIONACCOUNTINFO_CONTRACTTYPE._serialized_start=5790
-  _BROKERSESSIONACCOUNTINFO_CONTRACTTYPE._serialized_end=5873
-  _BROKERSESSIONACCOUNTINFO_ASSETTYPE._serialized_start=5745
-  _BROKERSESSIONACCOUNTINFO_ASSETTYPE._serialized_end=5788
-  _BROKERINFOSTARTSESSIONCONFIG._serialized_start=18559
-  _BROKERINFOSTARTSESSIONCONFIG._serialized_end=18714
-  _BROKERINFOTESTCONFIG._serialized_start=18717
-  _BROKERINFOTESTCONFIG._serialized_end=18961
-  _BROKERWORKERCONFIG._serialized_start=18963
-  _BROKERWORKERCONFIG._serialized_end=19066
-  _BROKERSTOPCONSUMERLISTENER._serialized_start=19068
-  _BROKERSTOPCONSUMERLISTENER._serialized_end=19132
-  _BROKERSTOPCONSUMERCOMMAND._serialized_start=19134
-  _BROKERSTOPCONSUMERCOMMAND._serialized_end=19178
-  _BROKERSTARTSESSIONINFO._serialized_start=19180
-  _BROKERSTARTSESSIONINFO._serialized_end=19204
-  _BROKERERROR._serialized_start=19206
-  _BROKERERROR._serialized_end=19309
-  _BROKERCOMMANDS._serialized_start=19311
-  _BROKERCOMMANDS._serialized_end=19417
-  _BROKERSESSIONREGISTRATION._serialized_start=19419
-  _BROKERSESSIONREGISTRATION._serialized_end=19465
-  _BROKERCOMMANDSANSWER._serialized_start=19467
-  _BROKERCOMMANDSANSWER._serialized_end=19547
-  _BROKERCOMMANDSANSWERERROR._serialized_start=19549
-  _BROKERCOMMANDSANSWERERROR._serialized_end=19649
-  _BROKEREVENTDATA._serialized_start=19651
-  _BROKEREVENTDATA._serialized_end=19752
-  _BROKERCOMMANDREGISTRATION._serialized_start=19754
-  _BROKERCOMMANDREGISTRATION._serialized_end=19800
-  _BROKERTESTPROTOCOLDATA._serialized_start=19802
-  _BROKERTESTPROTOCOLDATA._serialized_end=19876
-  _APPWORKERCONFIG._serialized_start=19879
-  _APPWORKERCONFIG._serialized_end=20035
-  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_start=20038
-  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_end=20335
-  _APPWORKERCOMMANDREGISTRATION._serialized_start=20337
-  _APPWORKERCOMMANDREGISTRATION._serialized_end=20386
-  _APPWORKERERROR._serialized_start=20388
-  _APPWORKERERROR._serialized_end=20475
-  _APPWORKERCOMMANDS._serialized_start=20477
-  _APPWORKERCOMMANDS._serialized_end=20590
-  _APPWORKERSESSIONREGISTRATION._serialized_start=20592
-  _APPWORKERSESSIONREGISTRATION._serialized_end=20677
-  _APPWORKERCOMMANDSANSWER._serialized_start=20679
-  _APPWORKERCOMMANDSANSWER._serialized_end=20762
-  _APPWORKERCOMMANDSANSWERERROR._serialized_start=20764
-  _APPWORKERCOMMANDSANSWERERROR._serialized_end=20867
-  _APPWORKEREVENTDATA._serialized_start=20869
-  _APPWORKEREVENTDATA._serialized_end=20973
-  _APPWORKERBROKERCOMMAND._serialized_start=20976
-  _APPWORKERBROKERCOMMAND._serialized_end=21107
-  _APPWORKERBROKERCOMMANDANSWER._serialized_start=21110
-  _APPWORKERBROKERCOMMANDANSWER._serialized_end=21269
-  _APPWORKERMODULECOMMAND._serialized_start=21272
-  _APPWORKERMODULECOMMAND._serialized_end=21419
-  _APPWORKERMODULECOMMANDANSWER._serialized_start=21422
-  _APPWORKERMODULECOMMANDANSWER._serialized_end=21630
-  _APPWORKERFINISHEDSTEPINFOS._serialized_start=21632
-  _APPWORKERFINISHEDSTEPINFOS._serialized_end=21735
-  _APPWORKERREGISTRATIONINFO._serialized_start=21737
-  _APPWORKERREGISTRATIONINFO._serialized_end=21836
-  _FEATUREINFOSTARTSESSIONCONFIG._serialized_start=21839
-  _FEATUREINFOSTARTSESSIONCONFIG._serialized_end=22140
-  _FEATUREWORKERCONFIG._serialized_start=22142
-  _FEATUREWORKERCONFIG._serialized_end=22247
-  _FEATUREERROR._serialized_start=22249
-  _FEATUREERROR._serialized_end=22334
-  _FEATURECOMMANDS._serialized_start=22336
-  _FEATURECOMMANDS._serialized_end=22431
-  _FEATURECOMMANDSANSWER._serialized_start=22433
-  _FEATURECOMMANDSANSWER._serialized_end=22514
-  _FEATURECOMMANDSANSWERERROR._serialized_start=22516
-  _FEATURECOMMANDSANSWERERROR._serialized_end=22617
-  _FEATURESESSIONREGISTRATION._serialized_start=22619
-  _FEATURESESSIONREGISTRATION._serialized_end=22666
-  _FEATUREEVENTDATA._serialized_start=22668
-  _FEATUREEVENTDATA._serialized_end=22770
-  _REGISTRATIONINFORMATION._serialized_start=22772
-  _REGISTRATIONINFORMATION._serialized_end=22834
-  _SYMBOLDATAREQUESTINFO._serialized_start=22836
-  _SYMBOLDATAREQUESTINFO._serialized_end=22909
-  _SYMBOLDATARESPONSE._serialized_start=22911
-  _SYMBOLDATARESPONSE._serialized_end=22982
-  _EXCHANGEDATAREQUESTINFO._serialized_start=22984
-  _EXCHANGEDATAREQUESTINFO._serialized_end=23009
-  _BROKEREXCHANGESMALL._serialized_start=23011
-  _BROKEREXCHANGESMALL._serialized_end=23087
-  _EXCHANGEDATARESPONSE._serialized_start=23089
-  _EXCHANGEDATARESPONSE._serialized_end=23160
-  _SYMBOLBROKERSYMBOLSMALL._serialized_start=23163
-  _SYMBOLBROKERSYMBOLSMALL._serialized_end=23465
-  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_start=23419
-  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_end=23465
-  _MARKETDATAREQUEST._serialized_start=23468
-  _MARKETDATAREQUEST._serialized_end=23646
-  _MARKETDATARESPONSE._serialized_start=23648
-  _MARKETDATARESPONSE._serialized_end=23752
-  _FEATUREDATARESPONSE._serialized_start=23754
-  _FEATUREDATARESPONSE._serialized_end=23859
-  _FEATUREDATAREQUEST._serialized_start=23862
-  _FEATUREDATAREQUEST._serialized_end=24022
-  _ADDITIONALDATAFEATUREREQUEST._serialized_start=24024
-  _ADDITIONALDATAFEATUREREQUEST._serialized_end=24054
-  _ADDITIONALDATAFEATUREINFO._serialized_start=24056
-  _ADDITIONALDATAFEATUREINFO._serialized_end=24177
-  _ADDITIONALDATAFEATURERESPONSE._serialized_start=24179
-  _ADDITIONALDATAFEATURERESPONSE._serialized_end=24268
-  _NOTIFICATIONOPTIONS._serialized_start=24270
-  _NOTIFICATIONOPTIONS._serialized_end=24362
-  _NOTIFICATIONREGISTRATION._serialized_start=24365
-  _NOTIFICATIONREGISTRATION._serialized_end=24636
-  _FEATUREOPTIONS._serialized_start=24638
-  _FEATUREOPTIONS._serialized_end=24725
-  _FEATUREREGISTRATION._serialized_start=24728
-  _FEATUREREGISTRATION._serialized_end=25050
-  _SIMULATORMETHODCALL._serialized_start=25052
-  _SIMULATORMETHODCALL._serialized_end=25105
-  _STATISTICFUNCTIONINPUTS._serialized_start=25107
-  _STATISTICFUNCTIONINPUTS._serialized_end=25203
-  _STATISTICMETHODINPUTS._serialized_start=25205
-  _STATISTICMETHODINPUTS._serialized_end=25315
-  _STATISTICMETHODREGISTRATION._serialized_start=25318
-  _STATISTICMETHODREGISTRATION._serialized_end=25603
-  _STATISTICRULEFUNCTIONREGISTRATION._serialized_start=25606
-  _STATISTICRULEFUNCTIONREGISTRATION._serialized_end=25865
-  _WORKERREGISTRYREQUEST._serialized_start=25867
-  _WORKERREGISTRYREQUEST._serialized_end=25932
-  _WORKERREGISTRYRESPONSE._serialized_start=25934
-  _WORKERREGISTRYRESPONSE._serialized_end=26002
-  _APIKEY._serialized_start=26004
-  _APIKEY._serialized_end=26049
-  _AUTHKEY._serialized_start=26051
-  _AUTHKEY._serialized_end=26099
-  _CHARTSWORKER._serialized_start=26102
-  _CHARTSWORKER._serialized_end=26348
-  _STATISTICSMETHODWORKER._serialized_start=26351
-  _STATISTICSMETHODWORKER._serialized_end=26636
-  _SYMBOLBROKERWORKER._serialized_start=26639
-  _SYMBOLBROKERWORKER._serialized_end=27453
-  _NOTIFICATIONWORKER._serialized_start=27456
-  _NOTIFICATIONWORKER._serialized_end=27721
-  _LOGICRUNNEROFFLINESERVICE._serialized_start=27724
-  _LOGICRUNNEROFFLINESERVICE._serialized_end=28214
-  _DATAWORKER._serialized_start=28217
-  _DATAWORKER._serialized_end=28934
-  _PLUGINWORKER._serialized_start=28937
-  _PLUGINWORKER._serialized_end=29096
-  _SIMULATOR._serialized_start=29099
-  _SIMULATOR._serialized_end=29770
-  _FUNCTIONS._serialized_start=29772
-  _FUNCTIONS._serialized_end=29881
-  _LOGIC._serialized_start=29884
-  _LOGIC._serialized_end=30584
-  _BROKER._serialized_start=30586
-  _BROKER._serialized_end=30667
-  _BROKERWORKER._serialized_start=30670
-  _BROKERWORKER._serialized_end=31232
-  _APPWORKER._serialized_start=31235
-  _APPWORKER._serialized_end=32292
-  _FEATUREWORKER._serialized_start=32295
-  _FEATUREWORKER._serialized_end=32841
-  _SYMBOL._serialized_start=32843
-  _SYMBOL._serialized_end=32936
-  _DATALOADERWORKER._serialized_start=32939
-  _DATALOADERWORKER._serialized_end=33388
-  _NOTIFICATION._serialized_start=33390
-  _NOTIFICATION._serialized_end=33489
-  _FEATURES._serialized_start=33491
-  _FEATURES._serialized_end=33576
-  _STATISTICS._serialized_start=33579
-  _STATISTICS._serialized_end=33785
-  _DATAWORKERREGISTRY._serialized_start=33788
-  _DATAWORKERREGISTRY._serialized_end=34033
+  _CHARTWORKERPARTIALDATAINFO._serialized_end=930
+  _CHARTSWORKERPARTIALDATALAYOUT._serialized_start=933
+  _CHARTSWORKERPARTIALDATALAYOUT._serialized_end=1106
+  _CHARTWORKERINDICATOR._serialized_start=1109
+  _CHARTWORKERINDICATOR._serialized_end=1330
+  _CHARTWORKERINDICATORREGISTRATION._serialized_start=1333
+  _CHARTWORKERINDICATORREGISTRATION._serialized_end=1681
+  _CHARTWORKERINDICATORCONFIGELEMENT._serialized_start=1683
+  _CHARTWORKERINDICATORCONFIGELEMENT._serialized_end=1793
+  _CHARTSWORKERCONFIG._serialized_start=1796
+  _CHARTSWORKERCONFIG._serialized_end=1968
+  _STATISTICINPUT._serialized_start=1970
+  _STATISTICINPUT._serialized_end=2015
+  _DATAERROR._serialized_start=2017
+  _DATAERROR._serialized_end=2082
+  _INDICATORERROR._serialized_start=2085
+  _INDICATORERROR._serialized_end=2222
+  _STATISTICRULEFUNCTIONERROR._serialized_start=2225
+  _STATISTICRULEFUNCTIONERROR._serialized_end=2388
+  _STATISTICMETHODFUNCTIONERROR._serialized_start=2391
+  _STATISTICMETHODFUNCTIONERROR._serialized_end=2556
+  _STATISTICSMETHODWORKERWINDOWCONFIG._serialized_start=2559
+  _STATISTICSMETHODWORKERWINDOWCONFIG._serialized_end=2737
+  _PARAMETERTABLEENTRY._serialized_start=2739
+  _PARAMETERTABLEENTRY._serialized_end=2821
+  _PARAMETERTABLE._serialized_start=2823
+  _PARAMETERTABLE._serialized_end=2889
+  _CHARTDATAINFO._serialized_start=2891
+  _CHARTDATAINFO._serialized_end=3013
+  _STATISTICSRULEWORKERCONFIG._serialized_start=3016
+  _STATISTICSRULEWORKERCONFIG._serialized_end=3390
+  _STATISTICSRULEWORKERCONFIG_INPUTSENTRY._serialized_start=3320
+  _STATISTICSRULEWORKERCONFIG_INPUTSENTRY._serialized_end=3390
+  _STATISTICSRULEWORKERCONFIGTYPE._serialized_start=3393
+  _STATISTICSRULEWORKERCONFIGTYPE._serialized_end=3561
+  _STATISTICSBULKEDWORKERCONFIG._serialized_start=3564
+  _STATISTICSBULKEDWORKERCONFIG._serialized_end=3744
+  _STATISTICFUNCTIONERROR._serialized_start=3747
+  _STATISTICFUNCTIONERROR._serialized_end=3906
+  _STATISTICMETHODPARTIALLYDATA._serialized_start=3909
+  _STATISTICMETHODPARTIALLYDATA._serialized_end=4076
+  _STATISTICRULEPARTIALLYDATA._serialized_start=4079
+  _STATISTICRULEPARTIALLYDATA._serialized_end=4245
+  _STATISTICBULKEDPARTIALLYDATA._serialized_start=4248
+  _STATISTICBULKEDPARTIALLYDATA._serialized_end=4410
+  _SYMBOLBROKERERROR._serialized_start=4412
+  _SYMBOLBROKERERROR._serialized_end=4521
+  _SYMBOLBROKERCONSUMERERROR._serialized_start=4523
+  _SYMBOLBROKERCONSUMERERROR._serialized_end=4608
+  _SYMBOLBROKERMARKETDATA._serialized_start=4611
+  _SYMBOLBROKERMARKETDATA._serialized_end=4888
+  _SYMBOLBROKERINFO._serialized_start=4891
+  _SYMBOLBROKERINFO._serialized_end=5041
+  _SYMBOLBROKERORDERBOOK._serialized_start=5043
+  _SYMBOLBROKERORDERBOOK._serialized_end=5102
+  _SYMBOLBROKERHISTORICALMARKETDATA._serialized_start=5104
+  _SYMBOLBROKERHISTORICALMARKETDATA._serialized_end=5174
+  _SYMBOLBROKEREXCHANGE._serialized_start=5177
+  _SYMBOLBROKEREXCHANGE._serialized_end=5363
+  _SYMBOLBROKERSYMBOL._serialized_start=5366
+  _SYMBOLBROKERSYMBOL._serialized_end=5890
+  _SYMBOLBROKERSYMBOL_ASSETTYPE._serialized_start=5762
+  _SYMBOLBROKERSYMBOL_ASSETTYPE._serialized_end=5805
+  _SYMBOLBROKERSYMBOL_CONTRACTTYPE._serialized_start=5807
+  _SYMBOLBROKERSYMBOL_CONTRACTTYPE._serialized_end=5890
+  _SYMBOLBROKERBROKERINFOCONFIG._serialized_start=5892
+  _SYMBOLBROKERBROKERINFOCONFIG._serialized_end=5971
+  _SYMBOLBROKERCONSUMEMARKETDATACONFIG._serialized_start=5974
+  _SYMBOLBROKERCONSUMEMARKETDATACONFIG._serialized_end=6451
+  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_ASSETTYPE._serialized_start=5762
+  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_ASSETTYPE._serialized_end=5805
+  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_CONTRACTTYPE._serialized_start=5807
+  _SYMBOLBROKERCONSUMEMARKETDATACONFIG_CONTRACTTYPE._serialized_end=5890
+  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG._serialized_start=6454
+  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG._serialized_end=6928
+  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_ASSETTYPE._serialized_start=5762
+  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_ASSETTYPE._serialized_end=5805
+  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_CONTRACTTYPE._serialized_start=5807
+  _SYMBOLBROKERCONSUMEORDERBOOKCONFIG_CONTRACTTYPE._serialized_end=5890
+  _SYMBOLBROKERGETHISTORICALDATACONFIG._serialized_start=6931
+  _SYMBOLBROKERGETHISTORICALDATACONFIG._serialized_end=7499
+  _SYMBOLBROKERGETHISTORICALDATACONFIG_ASSETTYPE._serialized_start=5762
+  _SYMBOLBROKERGETHISTORICALDATACONFIG_ASSETTYPE._serialized_end=5805
+  _SYMBOLBROKERGETHISTORICALDATACONFIG_CONTRACTTYPE._serialized_start=5807
+  _SYMBOLBROKERGETHISTORICALDATACONFIG_CONTRACTTYPE._serialized_end=5890
+  _SYMBOLBROKERWORKERCONFIG._serialized_start=7502
+  _SYMBOLBROKERWORKERCONFIG._serialized_end=7827
+  _SYMBOLBROKERSTOPCONSUMERLISTENER._serialized_start=7829
+  _SYMBOLBROKERSTOPCONSUMERLISTENER._serialized_end=7899
+  _SYMBOLBROKERSTOPCONSUMERCOMMAND._serialized_start=7901
+  _SYMBOLBROKERSTOPCONSUMERCOMMAND._serialized_end=7951
+  _SYMBOLBROKERFETCHDATA._serialized_start=7953
+  _SYMBOLBROKERFETCHDATA._serialized_end=8059
+  _NOTIFICATIONEXTRACTMESSAGEDATACONFIG._serialized_start=8061
+  _NOTIFICATIONEXTRACTMESSAGEDATACONFIG._serialized_end=8178
+  _NOTIFICATIONSENDMESSAGEDATACONFIG._serialized_start=8181
+  _NOTIFICATIONSENDMESSAGEDATACONFIG._serialized_end=8392
+  _NOTIFICATIONWORKERCONFIG._serialized_start=8395
+  _NOTIFICATIONWORKERCONFIG._serialized_end=8584
+  _NOTIFICATIONERROR._serialized_start=8586
+  _NOTIFICATIONERROR._serialized_end=8676
+  _NOTIFICATIONCALLBACKEXTRACT._serialized_start=8678
+  _NOTIFICATIONCALLBACKEXTRACT._serialized_end=8776
+  _LOGICCOMPONENT._serialized_start=8779
+  _LOGICCOMPONENT._serialized_end=8931
+  _BROKERACCOUNTMODEL._serialized_start=8934
+  _BROKERACCOUNTMODEL._serialized_end=9412
+  _BROKERACCOUNTMODEL_BROKERTYPE._serialized_start=9242
+  _BROKERACCOUNTMODEL_BROKERTYPE._serialized_end=9323
+  _BROKERACCOUNTMODEL_BROKERMODE._serialized_start=9325
+  _BROKERACCOUNTMODEL_BROKERMODE._serialized_end=9374
+  _BROKERACCOUNTMODEL_FEEMODE._serialized_start=9376
+  _BROKERACCOUNTMODEL_FEEMODE._serialized_end=9412
+  _PORTFOLIOASSET._serialized_start=9414
+  _PORTFOLIOASSET._serialized_end=9540
+  _CALCULATEDBASEMONEY._serialized_start=9542
+  _CALCULATEDBASEMONEY._serialized_end=9653
+  _PORTFOLIOMODEL._serialized_start=9656
+  _PORTFOLIOMODEL._serialized_end=9848
+  _LOGICRUNNERLOGIC._serialized_start=9851
+  _LOGICRUNNERLOGIC._serialized_end=10237
+  _LOGICRUNNEROFFLINEWORKERCONFIG._serialized_start=10240
+  _LOGICRUNNEROFFLINEWORKERCONFIG._serialized_end=10453
+  _LOGICRUNNERSTATISTICS._serialized_start=10456
+  _LOGICRUNNERSTATISTICS._serialized_end=11047
+  _LOGICRUNNEROFFLINEWORKERPARTIALLYDATA._serialized_start=11050
+  _LOGICRUNNEROFFLINEWORKERPARTIALLYDATA._serialized_end=11216
+  _LOGICRUNNEROFFLINEWORKERERROR._serialized_start=11218
+  _LOGICRUNNEROFFLINEWORKERERROR._serialized_end=11337
+  _LOGICRUNNEROFFLINEWORKERFINISHEDDATA._serialized_start=11340
+  _LOGICRUNNEROFFLINEWORKERFINISHEDDATA._serialized_end=11520
+  _WORKSPACEINFO._serialized_start=11522
+  _WORKSPACEINFO._serialized_end=11597
+  _WORKERPLUGININFORMATION._serialized_start=11599
+  _WORKERPLUGININFORMATION._serialized_end=11663
+  _WORKERSETTINGS._serialized_start=11665
+  _WORKERSETTINGS._serialized_end=11725
+  _WORKERREGISTRATION._serialized_start=11727
+  _WORKERREGISTRATION._serialized_end=11766
+  _COLLECTIONNODEREQUEST._serialized_start=11768
+  _COLLECTIONNODEREQUEST._serialized_end=11866
+  _COLLECTIONNODERESPONSE._serialized_start=11868
+  _COLLECTIONNODERESPONSE._serialized_end=11926
+  _EVENTREQUEST._serialized_start=11928
+  _EVENTREQUEST._serialized_end=12024
+  _PLUGINCONFIG._serialized_start=12026
+  _PLUGINCONFIG._serialized_end=12142
+  _PLUGININSTALLATIONOUTPUT._serialized_start=12144
+  _PLUGININSTALLATIONOUTPUT._serialized_end=12229
+  _SIMULATORCHARTCONFIGINDICATOR._serialized_start=12232
+  _SIMULATORCHARTCONFIGINDICATOR._serialized_end=12435
+  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_start=12390
+  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_end=12435
+  _SIMULATORCHARTCONFIG._serialized_start=12438
+  _SIMULATORCHARTCONFIG._serialized_end=12608
+  _SIMULATORSTATISTICCHARTCONFIG._serialized_start=12611
+  _SIMULATORSTATISTICCHARTCONFIG._serialized_end=12762
+  _SIMULATORMETHODCALLCHARTCONFIG._serialized_start=12765
+  _SIMULATORMETHODCALLCHARTCONFIG._serialized_end=12964
+  _SIMULATORRESPONSE._serialized_start=12966
+  _SIMULATORRESPONSE._serialized_end=13030
+  _SYMBOLBROKERSIMULATORREQUEST._serialized_start=13033
+  _SYMBOLBROKERSIMULATORREQUEST._serialized_end=13164
+  _SYMBOLBROKERSIMULATORRESPONSE._serialized_start=13166
+  _SYMBOLBROKERSIMULATORRESPONSE._serialized_end=13269
+  _BROKERSIMULATORBROKERLOGINDATA._serialized_start=13271
+  _BROKERSIMULATORBROKERLOGINDATA._serialized_end=13335
+  _BROKERSIMULATORBROKERDATA._serialized_start=13338
+  _BROKERSIMULATORBROKERDATA._serialized_end=13487
+  _BROKERSIMULATORREQUEST._serialized_start=13490
+  _BROKERSIMULATORREQUEST._serialized_end=13642
+  _BROKERSIMULATORRESPONSE._serialized_start=13645
+  _BROKERSIMULATORRESPONSE._serialized_end=13823
+  _NOTIFICATIONSIMULATORREQUEST._serialized_start=13825
+  _NOTIFICATIONSIMULATORREQUEST._serialized_end=13927
+  _NOTIFICATIONSIMULATORRESPONSE._serialized_start=13929
+  _NOTIFICATIONSIMULATORRESPONSE._serialized_end=14028
+  _FEATURESIMULATORREQUEST._serialized_start=14030
+  _FEATURESIMULATORREQUEST._serialized_end=14110
+  _FEATURESIMULATORRESPONSE._serialized_start=14112
+  _FEATURESIMULATORRESPONSE._serialized_end=14206
+  _LOGICINPUT._serialized_start=14208
+  _LOGICINPUT._serialized_end=14307
+  _LOGICTRADERREGISTRATION._serialized_start=14310
+  _LOGICTRADERREGISTRATION._serialized_end=14571
+  _LOGICALERTREGISTRATION._serialized_start=14574
+  _LOGICALERTREGISTRATION._serialized_end=14834
+  _LOGICDATAREGISTRATION._serialized_start=14837
+  _LOGICDATAREGISTRATION._serialized_end=15096
+  _LOGICSCREENERREGISTRATION._serialized_start=15099
+  _LOGICSCREENERREGISTRATION._serialized_end=15362
+  _WORKSPACELOGICREGISTRATION._serialized_start=15365
+  _WORKSPACELOGICREGISTRATION._serialized_end=15638
+  _LOGICRUNJOB._serialized_start=15640
+  _LOGICRUNJOB._serialized_end=15674
+  _LOGICDATAUSAGE._serialized_start=15677
+  _LOGICDATAUSAGE._serialized_end=15984
+  _LOGICMONITOREVENT._serialized_start=15987
+  _LOGICMONITOREVENT._serialized_end=16230
+  _LOGICCOLLECTIONUSAGE._serialized_start=16233
+  _LOGICCOLLECTIONUSAGE._serialized_end=16479
+  _LOGICEVENTUSAGE._serialized_start=16482
+  _LOGICEVENTUSAGE._serialized_end=16708
+  _SYMBOLBROKEROPTIONS._serialized_start=16710
+  _SYMBOLBROKEROPTIONS._serialized_end=16802
+  _SYMBOLBROKERREGISTRATION._serialized_start=16805
+  _SYMBOLBROKERREGISTRATION._serialized_end=17033
+  _BROKEROPTIONS._serialized_start=17035
+  _BROKEROPTIONS._serialized_end=17121
+  _BROKEREXCHANGE._serialized_start=17124
+  _BROKEREXCHANGE._serialized_end=17598
+  _BROKEREXCHANGE_LOGINMODE._serialized_start=17444
+  _BROKEREXCHANGE_LOGINMODE._serialized_end=17468
+  _BROKEREXCHANGE_CONTRACTTYPE._serialized_start=5807
+  _BROKEREXCHANGE_CONTRACTTYPE._serialized_end=5890
+  _BROKEREXCHANGE_ASSETTYPE._serialized_start=5762
+  _BROKEREXCHANGE_ASSETTYPE._serialized_end=5805
+  _BROKERREGISTRATION._serialized_start=17601
+  _BROKERREGISTRATION._serialized_end=18025
+  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_start=17934
+  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_end=18025
+  _BROKERPORTFOLIO._serialized_start=18027
+  _BROKERPORTFOLIO._serialized_end=18090
+  _BROKERPORTFOLIOASSET._serialized_start=18092
+  _BROKERPORTFOLIOASSET._serialized_end=18182
+  _BROKERSESSIONACCOUNTINFO._serialized_start=18185
+  _BROKERSESSIONACCOUNTINFO._serialized_end=18573
+  _BROKERSESSIONACCOUNTINFO_CONTRACTTYPE._serialized_start=5807
+  _BROKERSESSIONACCOUNTINFO_CONTRACTTYPE._serialized_end=5890
+  _BROKERSESSIONACCOUNTINFO_ASSETTYPE._serialized_start=5762
+  _BROKERSESSIONACCOUNTINFO_ASSETTYPE._serialized_end=5805
+  _BROKERINFOSTARTSESSIONCONFIG._serialized_start=18576
+  _BROKERINFOSTARTSESSIONCONFIG._serialized_end=18731
+  _BROKERINFOTESTCONFIG._serialized_start=18734
+  _BROKERINFOTESTCONFIG._serialized_end=18978
+  _BROKERWORKERCONFIG._serialized_start=18980
+  _BROKERWORKERCONFIG._serialized_end=19083
+  _BROKERSTOPCONSUMERLISTENER._serialized_start=19085
+  _BROKERSTOPCONSUMERLISTENER._serialized_end=19149
+  _BROKERSTOPCONSUMERCOMMAND._serialized_start=19151
+  _BROKERSTOPCONSUMERCOMMAND._serialized_end=19195
+  _BROKERSTARTSESSIONINFO._serialized_start=19197
+  _BROKERSTARTSESSIONINFO._serialized_end=19221
+  _BROKERERROR._serialized_start=19223
+  _BROKERERROR._serialized_end=19326
+  _BROKERCOMMANDS._serialized_start=19328
+  _BROKERCOMMANDS._serialized_end=19434
+  _BROKERSESSIONREGISTRATION._serialized_start=19436
+  _BROKERSESSIONREGISTRATION._serialized_end=19482
+  _BROKERCOMMANDSANSWER._serialized_start=19484
+  _BROKERCOMMANDSANSWER._serialized_end=19564
+  _BROKERCOMMANDSANSWERERROR._serialized_start=19566
+  _BROKERCOMMANDSANSWERERROR._serialized_end=19666
+  _BROKEREVENTDATA._serialized_start=19668
+  _BROKEREVENTDATA._serialized_end=19769
+  _BROKERCOMMANDREGISTRATION._serialized_start=19771
+  _BROKERCOMMANDREGISTRATION._serialized_end=19817
+  _BROKERTESTPROTOCOLDATA._serialized_start=19819
+  _BROKERTESTPROTOCOLDATA._serialized_end=19893
+  _APPWORKERCONFIG._serialized_start=19896
+  _APPWORKERCONFIG._serialized_end=20052
+  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_start=20055
+  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_end=20352
+  _APPWORKERCOMMANDREGISTRATION._serialized_start=20354
+  _APPWORKERCOMMANDREGISTRATION._serialized_end=20403
+  _APPWORKERERROR._serialized_start=20405
+  _APPWORKERERROR._serialized_end=20492
+  _APPWORKERCOMMANDS._serialized_start=20494
+  _APPWORKERCOMMANDS._serialized_end=20607
+  _APPWORKERSESSIONREGISTRATION._serialized_start=20609
+  _APPWORKERSESSIONREGISTRATION._serialized_end=20694
+  _APPWORKERCOMMANDSANSWER._serialized_start=20696
+  _APPWORKERCOMMANDSANSWER._serialized_end=20779
+  _APPWORKERCOMMANDSANSWERERROR._serialized_start=20781
+  _APPWORKERCOMMANDSANSWERERROR._serialized_end=20884
+  _APPWORKEREVENTDATA._serialized_start=20886
+  _APPWORKEREVENTDATA._serialized_end=20990
+  _APPWORKERBROKERCOMMAND._serialized_start=20993
+  _APPWORKERBROKERCOMMAND._serialized_end=21124
+  _APPWORKERBROKERCOMMANDANSWER._serialized_start=21127
+  _APPWORKERBROKERCOMMANDANSWER._serialized_end=21286
+  _APPWORKERMODULECOMMAND._serialized_start=21289
+  _APPWORKERMODULECOMMAND._serialized_end=21436
+  _APPWORKERMODULECOMMANDANSWER._serialized_start=21439
+  _APPWORKERMODULECOMMANDANSWER._serialized_end=21647
+  _APPWORKERFINISHEDSTEPINFOS._serialized_start=21649
+  _APPWORKERFINISHEDSTEPINFOS._serialized_end=21752
+  _APPWORKERREGISTRATIONINFO._serialized_start=21754
+  _APPWORKERREGISTRATIONINFO._serialized_end=21853
+  _FEATUREINFOSTARTSESSIONCONFIG._serialized_start=21856
+  _FEATUREINFOSTARTSESSIONCONFIG._serialized_end=22157
+  _FEATUREWORKERCONFIG._serialized_start=22159
+  _FEATUREWORKERCONFIG._serialized_end=22264
+  _FEATUREERROR._serialized_start=22266
+  _FEATUREERROR._serialized_end=22351
+  _FEATURECOMMANDS._serialized_start=22353
+  _FEATURECOMMANDS._serialized_end=22448
+  _FEATURECOMMANDSANSWER._serialized_start=22450
+  _FEATURECOMMANDSANSWER._serialized_end=22531
+  _FEATURECOMMANDSANSWERERROR._serialized_start=22533
+  _FEATURECOMMANDSANSWERERROR._serialized_end=22634
+  _FEATURESESSIONREGISTRATION._serialized_start=22636
+  _FEATURESESSIONREGISTRATION._serialized_end=22683
+  _FEATUREEVENTDATA._serialized_start=22685
+  _FEATUREEVENTDATA._serialized_end=22787
+  _REGISTRATIONINFORMATION._serialized_start=22789
+  _REGISTRATIONINFORMATION._serialized_end=22851
+  _SYMBOLDATAREQUESTINFO._serialized_start=22853
+  _SYMBOLDATAREQUESTINFO._serialized_end=22926
+  _SYMBOLDATARESPONSE._serialized_start=22928
+  _SYMBOLDATARESPONSE._serialized_end=22999
+  _EXCHANGEDATAREQUESTINFO._serialized_start=23001
+  _EXCHANGEDATAREQUESTINFO._serialized_end=23026
+  _BROKEREXCHANGESMALL._serialized_start=23028
+  _BROKEREXCHANGESMALL._serialized_end=23104
+  _EXCHANGEDATARESPONSE._serialized_start=23106
+  _EXCHANGEDATARESPONSE._serialized_end=23177
+  _SYMBOLBROKERSYMBOLSMALL._serialized_start=23180
+  _SYMBOLBROKERSYMBOLSMALL._serialized_end=23482
+  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_start=23436
+  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_end=23482
+  _MARKETDATAREQUEST._serialized_start=23485
+  _MARKETDATAREQUEST._serialized_end=23663
+  _MARKETDATARESPONSE._serialized_start=23665
+  _MARKETDATARESPONSE._serialized_end=23769
+  _FEATUREDATARESPONSE._serialized_start=23771
+  _FEATUREDATARESPONSE._serialized_end=23876
+  _FEATUREDATAREQUEST._serialized_start=23879
+  _FEATUREDATAREQUEST._serialized_end=24039
+  _ADDITIONALDATAFEATUREREQUEST._serialized_start=24041
+  _ADDITIONALDATAFEATUREREQUEST._serialized_end=24071
+  _ADDITIONALDATAFEATUREINFO._serialized_start=24073
+  _ADDITIONALDATAFEATUREINFO._serialized_end=24194
+  _ADDITIONALDATAFEATURERESPONSE._serialized_start=24196
+  _ADDITIONALDATAFEATURERESPONSE._serialized_end=24285
+  _NOTIFICATIONOPTIONS._serialized_start=24287
+  _NOTIFICATIONOPTIONS._serialized_end=24379
+  _NOTIFICATIONREGISTRATION._serialized_start=24382
+  _NOTIFICATIONREGISTRATION._serialized_end=24653
+  _FEATUREOPTIONS._serialized_start=24655
+  _FEATUREOPTIONS._serialized_end=24742
+  _FEATUREREGISTRATION._serialized_start=24745
+  _FEATUREREGISTRATION._serialized_end=25067
+  _SIMULATORMETHODCALL._serialized_start=25069
+  _SIMULATORMETHODCALL._serialized_end=25122
+  _STATISTICFUNCTIONINPUTS._serialized_start=25124
+  _STATISTICFUNCTIONINPUTS._serialized_end=25220
+  _STATISTICMETHODINPUTS._serialized_start=25222
+  _STATISTICMETHODINPUTS._serialized_end=25332
+  _STATISTICMETHODREGISTRATION._serialized_start=25335
+  _STATISTICMETHODREGISTRATION._serialized_end=25620
+  _STATISTICRULEFUNCTIONREGISTRATION._serialized_start=25623
+  _STATISTICRULEFUNCTIONREGISTRATION._serialized_end=25882
+  _WORKERREGISTRYREQUEST._serialized_start=25884
+  _WORKERREGISTRYREQUEST._serialized_end=25949
+  _WORKERREGISTRYRESPONSE._serialized_start=25951
+  _WORKERREGISTRYRESPONSE._serialized_end=26019
+  _APIKEY._serialized_start=26021
+  _APIKEY._serialized_end=26066
+  _AUTHKEY._serialized_start=26068
+  _AUTHKEY._serialized_end=26116
+  _CHARTSWORKER._serialized_start=26119
+  _CHARTSWORKER._serialized_end=26365
+  _STATISTICSMETHODWORKER._serialized_start=26368
+  _STATISTICSMETHODWORKER._serialized_end=26653
+  _SYMBOLBROKERWORKER._serialized_start=26656
+  _SYMBOLBROKERWORKER._serialized_end=27470
+  _NOTIFICATIONWORKER._serialized_start=27473
+  _NOTIFICATIONWORKER._serialized_end=27738
+  _LOGICRUNNEROFFLINESERVICE._serialized_start=27741
+  _LOGICRUNNEROFFLINESERVICE._serialized_end=28231
+  _DATAWORKER._serialized_start=28234
+  _DATAWORKER._serialized_end=28951
+  _PLUGINWORKER._serialized_start=28954
+  _PLUGINWORKER._serialized_end=29113
+  _SIMULATOR._serialized_start=29116
+  _SIMULATOR._serialized_end=29787
+  _FUNCTIONS._serialized_start=29789
+  _FUNCTIONS._serialized_end=29898
+  _LOGIC._serialized_start=29901
+  _LOGIC._serialized_end=30601
+  _BROKER._serialized_start=30603
+  _BROKER._serialized_end=30684
+  _BROKERWORKER._serialized_start=30687
+  _BROKERWORKER._serialized_end=31249
+  _APPWORKER._serialized_start=31252
+  _APPWORKER._serialized_end=32309
+  _FEATUREWORKER._serialized_start=32312
+  _FEATUREWORKER._serialized_end=32858
+  _SYMBOL._serialized_start=32860
+  _SYMBOL._serialized_end=32953
+  _DATALOADERWORKER._serialized_start=32956
+  _DATALOADERWORKER._serialized_end=33405
+  _NOTIFICATION._serialized_start=33407
+  _NOTIFICATION._serialized_end=33506
+  _FEATURES._serialized_start=33508
+  _FEATURES._serialized_end=33593
+  _STATISTICS._serialized_start=33596
+  _STATISTICS._serialized_end=33802
+  _DATAWORKERREGISTRY._serialized_start=33805
+  _DATAWORKERREGISTRY._serialized_end=34050
 # @@protoc_insertion_point(module_scope)
```

### Comparing `coinlib-2.2.3/coinlib/dataWorker_pb2_grpc.py` & `coinlib-2.2.5/coinlib/dataWorker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/drawable/CoinlibDrawable.py` & `coinlib-2.2.5/coinlib/drawable/CoinlibDrawable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/drawable/WindowGrid.py` & `coinlib-2.2.5/coinlib/drawable/WindowGrid.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/event/EventConsumer.py` & `coinlib-2.2.5/coinlib/event/EventConsumer.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/event/EventInterface.py` & `coinlib-2.2.5/coinlib/event/EventInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/feature/CoinlibFeature.py` & `coinlib-2.2.5/coinlib/feature/CoinlibFeature.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,14 +56,48 @@
                 "interval": self.defaultInterval,
                 "datetime": None
             }
         }
 
         pass
 
+    def isLiveEnvironment(self):
+        return self.registrar.isLiveEnvironment()
+
+    def alarm(self, *params):
+
+        message = ""
+        for param in params:
+            message += str(param) + "\r\n "
+        try:
+            data_server_target = self.databaseInfo.server
+
+            backend = self.registrar.coinlib_backend_host
+            if backend is None:
+                backend = "http://" + self.registrar.workerEndpoint + ":9001"
+            if backend is None:
+                backend = 'http://localhost:9001'
+            url = backend + "/api/v1/historicalfeatures/alarm/" + data_server_target
+
+            data = requests.post(url,
+                                 json={
+                                     "feature": self.databaseInfo.id,
+                                     "message": message
+                                 },
+                                 headers={'Content-type': 'application/json',
+                                          'Accept': 'text/plain'})
+
+            if data.status_code == 200:
+                return data.json()
+
+        except Exception as e:
+            print("Can not send alarm to " + data_server_target + " " + self.databaseInfo.id + " " + str(e))
+            pass
+        return None
+
     def logger(self):
         return self.registrar.logger
 
     def set_worker(self, worker):
         self.worker = worker
 
     @staticmethod
@@ -224,43 +258,80 @@
                 pass
 
             self.save_statistics(columns, df2.shape[0])
         except Exception as e:
             print(e)
         return True
 
-    def get_data(self, identifier=None, group=None, symbol=None, limit=10):
+
+
+    def get_data_range(self, identifier=None):
         try:
-            chipmunkDb = ChipmunkDb(self.registrar.get_chipmunkdb_host(self.databaseInfo.server))
-            #list = chipmunkDb.query("SELECT * FROM "+self.databaseInfo.id+" LIMIT "+str(limit))
-            #df = pd.DataFrame(list)
-            df = chipmunkDb.collection_as_pandas(self.databaseInfo.id)
+            data_server_target = self.databaseInfo.server
 
-            if symbol is not None:
-                df = df.query("symbol == '"+symbol+"'")
+            backend = self.registrar.coinlib_backend_host
+            if backend is None:
+                backend = "http://" + self.registrar.workerEndpoint + ":9001"
+            if backend is None:
+                backend = 'http://localhost:9001'
+            url = backend + "/api/v1/historicalfeatures/range/" + data_server_target
+
+            data = requests.post(url,
+                                 json={
+                                        "id": identifier,
+                                        "stage": "dev" if not self.registrar.isLiveEnvironment() else "live"
+                                       },
+                                 headers={'Content-type': 'application/json',
+                                          'Accept': 'text/plain'})
 
-            if identifier is not None:
-                id = identifier
-                if group is not None:
-                    id = group + "." + identifier
-                cols = []
-                if "datetime" in df.columns.to_list():
-                    cols.append("datetime")
-                if "symbol" in df.columns.to_list():
-                    cols.append("symbol")
-                if "exchange" in df.columns.to_list():
-                    cols.append("exchange")
-                if id in df.columns.to_list():
-                    cols.append(id)
-                return df[cols]
+            if data.status_code == 200:
+                return data.json()
 
-            return df
+        except Exception as e:
+            print("Can not read data from " + data_server_target + " " + self.databaseInfo.id + " " + str(e))
+            pass
+        return None
+
+    def get_data(self, identifier=None, start=None, end=None, query=None, limit=-1):
+        try:
+            data_server_target = self.databaseInfo.server
+
+            backend = self.registrar.coinlib_backend_host
+            if backend is None:
+                backend = "http://" + self.registrar.workerEndpoint + ":9001"
+            if backend is None:
+                backend = 'http://localhost:9001'
+            url = backend + "/api/v1/historicalfeatures/read/" + data_server_target
+
+            if query is None:
+                query = {
+                        "datetime": {
+                            "$gte": start.strftime("%Y-%m-%dT%H:%M:%S.%fZ"),
+                            "$lte": end.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+
+                    }
+
+                }
+
+            data = requests.post(url,
+                                 json={
+                                        "id": identifier,
+                                        "query": query,
+                                         "limit": limit,
+                                        "stage": "dev" if not self.registrar.isLiveEnvironment() else "live"
+                                       },
+                                 headers={'Content-type': 'application/json',
+                                          'Accept': 'text/plain'})
+
+            if data.status_code == 200:
+                return data.json()
 
         except Exception as e:
-            raise e
+            print("Can not read data from " + data_server_target + " " + self.databaseInfo.id + " " + str(e))
+            pass
         return None
 
     def delete_data(self, identifier=None, group=None):
         try:
 
             chipmunkDb = ChipmunkDb(self.registrar.get_chipmunkdb_host(self.databaseInfo.server))
             if identifier is not None:
@@ -281,15 +352,16 @@
             self.transactions["default"] = {
                 "data": [],
                 "interval": self.defaultInterval,
                 "datetime": None
             }
 
 
-    def write_data(self, identifier, value, symbol=None, exchange=None, interval=None, dt=None, group=None, transaction=None):
+    def write_data(self, identifier, value, symbol=None, exchange=None, interval=None,
+                   dt=None, group=None, transaction=None, additonalData=None):
 
         if transaction is None:
 
             if interval is None:
                 self.transactions["default"]["interval"] = self.defaultInterval
                 interval = self.defaultInterval
 
@@ -298,22 +370,26 @@
                 self.transactions["default"]["datetime"] = dt
             elif dt is None:
                 dt = self.transactions["default"]["datetime"]
             else:
                 dt = CoinlibFeature.formatInterval(dt, interval)
 
 
-            self.transactions["default"]["data"].append({
+
+            row = {
                 "identifier": identifier,
                 "value": value,
                 "symbol": symbol,
                 "exchange": exchange,
                 "datetime": dt,
                 "group": group
-            })
+            }
+            if additonalData is not None:
+                row.update(additonalData)
+            self.transactions["default"]["data"].append(row)
 
             # start a timer interval to write data when x seconds are gone
             if self.saveTimer is not None:
                 self.saveTimer.cancel()
                 self.saveTimer = None
             self.saveTimer = threading.Timer(2.0, self.saveDataAfterWriteTimeout)
             self.saveTimer.start()
@@ -322,24 +398,26 @@
             if interval is None:
                 interval = self.transactions[transaction]["interval"]
 
             if dt is None:
                 dt = self.transactions[transaction]["datetime"]
             else:
                 dt = CoinlibFeature.formatInterval(dt, interval)
-
-            if transaction in self.transactions:
-                self.transactions[transaction]["data"].append({
+            row = {
                     "identifier": identifier,
                     "value": value,
                     "symbol": symbol,
                     "exchange": exchange,
                     "datetime": dt,
                     "group": group
-                })
+                }
+            if additonalData is not None:
+                row.update(additonalData)
+            if transaction in self.transactions:
+                self.transactions[transaction]["data"].append()
             else:
                 self.logger().error("Transactionn does not exist")
                 return False
 
         return True
 
     def finish_transaction_sync(self, transaction_id):
@@ -358,14 +436,20 @@
         for name in self.timer_list:
             self.cancel_timer(name)
 
     def stop(self):
         self._stopped = True
         self.cancelAllTimer()
 
+    def isRunning(self):
+        return not self._stopped
+
+    def isStopped(self):
+        return self._stopped
+
     def cancel_timer(self, name: str):
         if name in self.timer_list:
             self.timer_list[name].cancel()
             return True
         return False
 
     def timer_was_called(self, interval, name, process):
```

### Comparing `coinlib-2.2.3/coinlib/feature/CoinlibFeatureFetcher.py` & `coinlib-2.2.5/coinlib/feature/CoinlibFeatureFetcher.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/feature/CoinlibFeatureLake.py` & `coinlib-2.2.5/coinlib/feature/CoinlibFeatureLake.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/feature/FeatureDTO.py` & `coinlib-2.2.5/coinlib/feature/FeatureDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/feature/FeatureWorker.py` & `coinlib-2.2.5/coinlib/feature/FeatureWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/feature/Features.py` & `coinlib-2.2.5/coinlib/feature/Features.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/helper.py` & `coinlib-2.2.5/coinlib/helper.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logger.py` & `coinlib-2.2.5/coinlib/logger.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/Logic.py` & `coinlib-2.2.5/coinlib/logics/Logic.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicBasicWorker.py` & `coinlib-2.2.5/coinlib/logics/LogicBasicWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicJob.py` & `coinlib-2.2.5/coinlib/logics/LogicJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicLoader.py` & `coinlib-2.2.5/coinlib/logics/LogicLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicOfflineJob.py` & `coinlib-2.2.5/coinlib/logics/LogicOfflineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicOfflineWorker.py` & `coinlib-2.2.5/coinlib/logics/LogicOfflineWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerTrader.py` & `coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerTrader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicOnlineJob.py` & `coinlib-2.2.5/coinlib/logics/LogicOnlineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicOnlineWorker.py` & `coinlib-2.2.5/coinlib/logics/LogicOnlineWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicRegistrationInstance.py` & `coinlib-2.2.5/coinlib/logics/LogicRegistrationInstance.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/LogicTestBrokerWorker.py` & `coinlib-2.2.5/coinlib/logics/LogicTestBrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/broker/LogicBrokerInterface.py` & `coinlib-2.2.5/coinlib/logics/broker/LogicBrokerInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/manager/LogicJobBroker.py` & `coinlib-2.2.5/coinlib/logics/manager/LogicJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/manager/LogicManager.py` & `coinlib-2.2.5/coinlib/logics/manager/LogicManager.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/manager/PortfolioModel.py` & `coinlib-2.2.5/coinlib/logics/manager/PortfolioModel.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py` & `coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py` & `coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py` & `coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/logics/onlineManager/LogicOnlineJobBroker.py` & `coinlib-2.2.5/coinlib/logics/onlineManager/LogicOnlineJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/notification/Notification.py` & `coinlib-2.2.5/coinlib/notification/Notification.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/notification/NotificationWorker.py` & `coinlib-2.2.5/coinlib/notification/NotificationWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/statistics/StatisticMethodJob.py` & `coinlib-2.2.5/coinlib/statistics/StatisticMethodJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/statistics/StatisticRuleJob.py` & `coinlib-2.2.5/coinlib/statistics/StatisticRuleJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/statistics/Statistics.py` & `coinlib-2.2.5/coinlib/statistics/Statistics.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/statistics/StatisticsMethodWorker.py` & `coinlib-2.2.5/coinlib/statistics/StatisticsMethodWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/statistics/StatisticsRuleWorker.py` & `coinlib-2.2.5/coinlib/statistics/StatisticsRuleWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/symbols/SymbolWorker.py` & `coinlib-2.2.5/coinlib/symbols/SymbolWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib/symbols/Symbols.py` & `coinlib-2.2.5/coinlib/symbols/Symbols.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/coinlib.egg-info/PKG-INFO` & `coinlib-2.2.5/coinlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.3
+Version: 2.2.5
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.3/coinlib.egg-info/SOURCES.txt` & `coinlib-2.2.5/coinlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/setup.py` & `coinlib-2.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README_pip.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="coinlib",
-    version="2.2.3",
+    version="2.2.5",
     description="Develop new code for your coindeck environment",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/coindeck/coinlib",
     author="coindeck",
     author_email="donnercody86@gmail.com",
     license="MIT",
```

### Comparing `coinlib-2.2.3/test/testchartworker.py` & `coinlib-2.2.5/test/testchartworker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/test/testcross.py` & `coinlib-2.2.5/test/testcross.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.3/test/testplot.py` & `coinlib-2.2.5/test/testplot.py`

 * *Files identical despite different names*

